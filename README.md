# Python Text-Based Block Mining Simulator

A modular, Object-Oriented Programming (OOP) CLI simulation in Python where players equip customizable tools, mine blocks with dynamically rendered emoji grids, collect resources, and manage inventory state with local file persistence.

## Key Features

* **Object-Oriented Architecture:** Clean class-based architecture separating game logic (`Block`, `Player`, `Tools`, `GameEngine`) from state persistence and UI formatting[cite: 3, 5, 7, 9, 10].
* **Dynamic Visual Rendering:** Renders real-time ASCII/Emoji brick grids (`🧱`) that visually scale based on block size and health[cite: 3].
* **Tool & Material Mechanics:** Custom tool classes (Wooden, Stone, Iron, Diamond, Netherite) with discrete damage values, wear mechanics, and durability loss[cite: 9].
* **Persistence & Save Management:** Features game state logging and parameter loading via `CSV` file I/O and preset resource management via `JSON` files[cite: 5, 6, 8].
* **Interactive CLI Engine:** Interactive menu system supporting custom parameter selection, game loops, inventory progression, and match history review.

## Tech Stack

* **Language:** Python 3.x
* **Data Persistence:** CSV, JSON[cite: 5, 6, 8]
* **Design Patterns:** Object-Oriented Programming (OOP), Model-View-Controller (MVC) decoupling[cite: 3, 5, 7, 9, 10]

## Project Structure

```text
├── block.py        # Block class handling size, damage, and rendering[cite: 3]
├── player.py       # Player class tracking inventory and stats[cite: 7]
├── tool.py         # Tool class handling damage, durability, and types[cite: 9]
├── gameengine.py   # Core game loop, menu management, and workflow
├── save.py         # CSV file persistence for saved games and parameters[cite: 8]
├── load.py         # JSON parameter loading and block management[cite: 6]
├── ui.py           # Text formatting and UI strings[cite: 10]
├── game.py         # Simplified game loop runner[cite: 4]
└── README.md       # Project documentation
