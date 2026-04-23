<!-- HERO -->

<h1 align="center">🧙‍♂️ A HEALTH GAME</h1>

<h3 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=00FFAA&center=true&vCenter=true&width=600&lines=Turn+Your+Life+Into+An+RPG;Gain+XP+For+Healthy+Habits;Level+Up+Your+Discipline;Built+With+Python+⚡"/>
</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Game-RPG-purple?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Health-System-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Python-Project-blue?style=for-the-badge&logo=python"/>
  <img src="https://img.shields.io/badge/Status-Learning-orange?style=for-the-badge"/>
</p>

<p align="center">
  <img src="https://media.giphy.com/media/f3iwJFOVOwuy7K6FFw/giphy.gif" width="500"/>
</p>

<p align="center">
  <b>⚔️ Train your habits like a game character ⚔️</b><br>
  Stop being lazy. Start gaining XP.
</p>

---

## 🧠 About The Project

**A Health Game** is a Python-based RPG-style system that turns real-life actions into **experience points (XP)**.

Instead of just tracking habits, you:

* 🏃 Gain XP for actions
* 🧙 Level up your character
* 🏆 Unlock ranks

Inspired by RPG mechanics, this system makes **self-discipline feel like a game**.

---

## 🚀 Features

<div align="center">

| ⚡ System        | 💡 Description          |
| --------------- | ----------------------- |
| 🎯 XP Engine    | Gain XP from activities |
| 🆙 Level System | Auto level-up logic     |
| 📈 Scaling      | Non-linear XP growth    |
| 🏆 Rank System  | Titles based on level   |
| 🔁 XP Carry     | Extra XP preserved      |
| 📊 Progress Bar | Visual console output   |

</div>

---

## 🧮 XP Formula

XP = 100 \cdot level^{1.5}

This ensures:

* Fast early progress ⚡
* Balanced mid-game 📊
* Challenging high levels 🔥

---

## 🏆 Rank System

| Level Range | Rank              |
| ----------- | ----------------- |
| 1 – 4       | Novice Mage       |
| 5 – 9       | Intermediate Mage |
| 10 – 14     | Main Sorcerer     |
| 15+         | Archmage          |

---

## 🧠 How It Works

```text
Do activity → Gain XP → Level Up → Rank Up → Repeat 🔁
```

---

## 📂 Project Structure

```bash
project/
│
├── player.py        # Core logic
├── main.py          # Execution
└── README.md
```

---

## ▶️ Usage

### 🧙 Create Player

```python
player = Player("Yeager")
```

---

### ⚡ Gain XP

```python
player.gain_xp(120, "Completed Workout")
player.gain_xp(500, "Finished Study Session")
```

---

## 📊 Example Output

```
--- ⚔️ Yeager performed Completed Workout! ---
Received 120 XP.

✨ LEVEL UP! You are now Level 2 (Novice Mage)! ✨

[████------] 20/282 XP
Level: 2 | Rank: Novice Mage
```

---

## 🎯 Learning Outcomes

✔ Object-Oriented Programming
✔ Game System Design
✔ Algorithmic Thinking
✔ State Management

---

## 🔮 Future Improvements

* 💾 Save/Load system
* ⚔️ Combat system
* 👾 Enemy AI
* 🌳 Skill tree
* 🖥 GUI (Tkinter / Pygame)
* ☁️ Database integration

---

## 🛠 Requirements

* Python 3.x
* No external libraries

---

## 👨‍💻 Author

**Akash**

<p align="center">
  <img src="https://img.shields.io/badge/Made%20With-🔥-black?style=for-the-badge"/>
</p>

---
