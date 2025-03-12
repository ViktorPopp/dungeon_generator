# Isaac Floor Generator

This is a simple room generation project using [Phaser.js](https://phaser.io/). The script generates a dungeon-like floor plan inspired by *The Binding of Isaac*, placing rooms dynamically while ensuring connectivity and structure.

## Features
* Generates a random dungeon layout.
* Places special rooms like the boss room, reward room, coin room, and secret room.
* Uses a queue-based algorithm to ensure a connected and structured dungeon.
* Click to start the generation process.

## Installation & Setup
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/isaac-floor-generator.git
   ```
2. Open `index.html` in a browser.
3. Click on the canvas to start the generation.

## Dependencies
- [Phaser.js](https://phaser.io/)

## Project Structure
```bash
/project-root
│-- index.html        # Main HTML file
│-- main.js           # Contains the dungeon generation logic
│-- images/           # Folder containing assets (cell, boss, reward, coin, secret)
│-- README.md         # This file
```

## How It Works
* The game initializes with a `Click to Start` prompt.
* On click, the script starts generating a dungeon layout.
* A floor grid is created, and rooms are placed dynamically.
* Special rooms (Boss, Reward, Coin, Secret) are added after basic room generation.
* The generation process follows constraints to ensure connectivity and fairness.

## Configuration
Modify these values to tweak the generation:
```js
var maxrooms = 15; // Maximum number of rooms
var minrooms = 7;  // Minimum number of rooms
var cellw = 50;    // Cell width
var cellh = 44;    // Cell height
```

## License
This project is open-source and licenced under the MIT-License. Feel free to modify and use it in your own projects!

## Learn more
* [boristhebrave.com](https://www.boristhebrave.com/2020/09/12/dungeon-generation-in-binding-of-isaac/)
