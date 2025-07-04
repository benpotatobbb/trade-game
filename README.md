Trader Adventure is a 2D top-down game made with Python and Pygame. You play as a character exploring a randomly generated world filled with grass, paths, and water. Along the way, you meet traders and can buy or sell items like Potions and Pokeballs. The goal is to manage your money and inventory wisely while moving around the map and interacting with different characters.

The map is made up of different tile types—mostly grass, with some paths and a bit of water. You can move using the arrow keys, but only across grass and path tiles. When trading, items cost more to buy and less to sell, so thinking strategically helps. A simple HUD shows your money, inventory, and trader details, and the game gives feedback messages when you do things like trade or try something that’s not allowed.

Requirements

Python 3.x
Pygame: Install via pip: pip install pygame



Installation

Ensure Python 3.x is installed on your system.
Install Pygame using the command above.
Download the trader game.py script.
Run the script:python trader_game.py



How to Play

Objective: Explore the map, interact with traders, and manage your inventory and money through trading.
Controls:
Arrow Keys: Move the player (Up, Down, Left, Right).
ESC Key: Exit trading mode when interacting with a trader.
Mouse Clicks: Click "Buy" or "Sell" buttons in the trading interface to trade items.


Gameplay:
Move the player to a trader's position to start trading.
During trading, view the trader's inventory and dialogue, and use buttons to buy or sell items.
Manage your money and inventory strategically to avoid running out of funds or items.
Avoid water tiles, as they are impassable.


Map:
Green Tiles: Grass (walkable).
Brown Tiles: Paths (walkable).
Blue Tiles: Water (impassable).


Player:
Starts with 200 money, 2 Potions, and 1 Pokeball.
Represented as a red circle.


Traders:
Represented as yellow triangles with names displayed above.
Each trader has unique inventory and dialogue.



Game Mechanics

Map: A 30x20 grid of tiles, with the player and traders placed on grass tiles for accessibility.
Items:
Potion: Base price $10 (Buy: $12, Sell: $8).
Pokeball: Base price $15 (Buy: $18, Sell: $12).


Trading:
Buy items from traders if you have enough money and the trader has stock.
Sell items to traders if you have the item in your inventory.
Messages display the outcome of trades or errors (e.g., insufficient funds).


Movement:
Player movement has a cooldown to prevent rapid inputs.
Movement is restricted to valid tiles (not water).



Technical Details

Language: Python 3 with Pygame.
Screen Resolution: 960x710 pixels (30x20 tile map with a 150-pixel HUD).
Frame Rate: 60 FPS.
Classes:
Item: Represents items with a name and base price.
Trader: Defines NPC traders with position, name, inventory, and dialogue.
Player: Manages player position, inventory, money, and movement cooldown.
TradeGame: Main game class handling map generation, rendering, input, and game loop.


Dependencies: Pygame for graphics and event handling.

Limitations

No save/load functionality; progress is reset on game close.
Limited item types (only Potions and Pokeballs).
No win/lose conditions or overarching objectives beyond trading.
Basic graphics using simple shapes (circles for player, triangles for traders).

Future Improvements

Add more item types and trader variety.
Implement quests or goals to give the game a clear objective.
Enhance visuals with sprites or textures.
Add sound effects and background music.
Include a save/load system for persistent progress.

Troubleshooting

Pygame not found: Ensure Pygame is installed (pip install pygame).
Game window closes immediately: Check for errors in the terminal and ensure Python and Pygame are correctly installed.
Player can't move: Ensure you're not on a water tile or in trading mode (press ESC to exit trading).

License
This project is unlicensed and provided as-is for educational purposes.
