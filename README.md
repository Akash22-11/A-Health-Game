# A-Health-Game
This is a health game foe a lazy user who want discipline in his life but he can't 
class AnimeHealthAvatar:
    def __init__(self, name):
        self.name = name
        self.level = 1
        self.current_xp = 0
        self.xp_to_next_level = 100                                                                          # Starting 
        self.rank = "Beginer Adventurer"                                                                      # Anime style rank

    def calculate_xp_threshold(self):
        """
        Algorithm: As level increases, it becomes harder to level up.
        Formula: Next Level XP = Current Level * 100
        """
        self.xp_to_next_level = self.level * 100

    def gain_xp(self, amount, activity_name):
        print(f"--- ⚔️ {self.name} performed {activity_name}! ---")
        self.current_xp += amount
        print(f"Received {amount} XP.")
        
        # Check if we leveled up (Loop handles multiple level ups at once)
        while self.current_xp >= self.xp_to_next_level:
            self.level_up()
        
        self.show_stats()

    def level_up(self):
        self.current_xp -= self.xp_to_next_level                                                                 # Carry over extra XP
        self.level += 1
        self.calculate_xp_threshold()                                                                            # Recalculate difficulty
        
        # Rank Up Logic (If statements)
        if self.level == 5:
            self.rank = "Intermediate Mage"
        elif self.level == 10:
            self.rank = "Main Sorcerer"
            
        print(f"\n✨  HURRY LEVEL UP! You are now Level {self.level} ({self.rank})! ✨\n")

    def show_stats(self):
        # Create a visual progress bar
        progress_percent = int((self.current_xp / self.xp_to_next_level) * 10)
        bar = "█" * progress_percent + "-" * (10 - progress_percent)
        print(f"[{bar}] {self.current_xp}/{self.xp_to_next_level} XP to next level")

# --- Simulation Code (How to use it) ---

# 1. Create your avatar
player = AnimeHealthAvatar("Eren Yeager")

# 2. Simulate health activities
player.gain_xp(20, "Drank 1 Liter Water")                                                                     # 520/100 XP
player.gain_xp(30, "Morning Jog")                                                                             # Level Up! (Total 110 XP)
player.gain_xp(100, "Hit Step Goal")                                                                          # XP boost
