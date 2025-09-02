# Ants vs. SomeBees

## 1. Introduction

This project is a **tower defense** style game called *Ants vs. SomeBees*. As the ant queen, you must defend your colony with the bravest ants you can recruit. Ants protect the colony from invading bees that move through tunnels toward the queen. If bees make it through, the ants lose. If ants irritate the bees enough by throwing leaves at them, the bees are vanquished and the colony survives.  

The game is inspired by PopCap Games’ *Plants vs. Zombies* and is built with Python, emphasizing object-oriented programming, class hierarchies, and stateful simulation.

---

## 2. The Game

The game is turn-based. Each turn:

1. New bees may enter the colony from the hive.  
2. The player places ants to defend their colony.  
3. All insects act individually (ants first, then bees).  

Bees either move forward toward the queen or sting an ant in their way. Ants act based on their type: some collect food, some throw leaves at bees, others have unique defenses or abilities.  

The game ends when either:  
- A bee reaches the queen’s base (ants lose), or  
- All bees are defeated (ants win).  

---

## 3. Files

This repository contains the following files:

- **`ants.py`** — Main game logic for Ants vs. SomeBees.  
- **`ants_plans.py`** — Defines details for different difficulty levels.  
- **`gui.py`** — Provides the graphical interface to play the game in a browser.  
- **`ucb.py`** — Utility functions used throughout the project.  
- **`static/`** — Directory of images and supporting assets used by the GUI.  
- **`templates/`** — HTML templates for the GUI.  

---

## 4. Playing the Game

The game can be run in two modes:  

- **Text-based (debug mode)** — runs in the terminal.  
- **Graphical mode (recommended)** — runs with a web-based GUI.  

### Run the graphical game:
```bash
$ python3 gui.py
By default, the game runs at http://127.0.0.1:31415/.
If you change code, restart the server (Ctrl + C then run again).
Options
python3 gui.py [-h] [-d DIFFICULTY] [-w] [--food FOOD]

optional arguments:
  -h, --help     show this help message and exit
  -d DIFFICULTY  sets difficulty (test / easy / normal / hard / extra-hard)
  -w, --water    loads a layout with water places
  --food FOOD    number of food to start with when testing

5. Acknowledgments
This project is based on the classic Ants vs. SomeBees assignment from UC Berkeley, adapted here with custom files and GUI integration.



