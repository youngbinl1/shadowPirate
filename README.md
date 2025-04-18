ShadowPirate - university project
ShadowPirate is a simple role-playing game built with Java and the Basic Academic Game Engine Library (Bagel). You play as a sailor trapped on a ship, trying to reach the exit while avoiding deadly obstacles. But beware—this sailor can’t swim!

🕹️ Gameplay
Your goal is to reach the ladder, located at the bottom-right corner of the screen. Along the way, you'll face immovable blocks that damage your health on contact. Keep an eye on your health bar—if it hits zero or you fall off the side of the ship, it's game over.

🎯 Objectives
- Navigate the sailor to the exit (the ladder).
- Avoid collisions with blocks (each hit reduces health).
- Stay onboard—falling off means instant death.
- Survive with at least 1 health point to win.

⚙️ How It Works
📍 Coordinates
- The game world is based on a 2D coordinate system:
  The top-left corner is (0,0).
  Coordinates increase toward the bottom-right.
  Positions are defined in pixels using Bagel's Point class.

🎞️ Frames
- Bagel updates the game in sync with your monitor’s refresh rate.
- Each update is called a frame.
- The update() method in the ShadowPirate class is called every frame to update game logic and redraw the screen.

💥 Collision Detection
- Collisions occur when the sailor's sprite overlaps with a block.

Bagel treats all images as rectangles and provides a Rectangle class to assist with collision detection.

🧰 Technologies Used
- Java
- Bagel Game Engine (Basic Academic Game Engine Library)

📁 Project Structure
plaintext
Copy
Edit
ShadowPirate/
├── src/
│   ├── ShadowPirate.java      // Main game logic and update loop
│   ├── Sailor.java            // Handles player movement, health, and collisions
│   └── Block.java             // Represents immovable obstacles
├── resources/                 // Game assets (images, sounds, etc.)
└── README.md                  // This file

🚀 How to Run
- Clone the repository.
- Open the project in your preferred IDE.
- Add the Bagel library to your classpath.
- Run ShadowPirate.java.

📝 Notes
- The sailor can’t swim, so falling off the ship ends the game.
- All obstacles are stationary.
- Collision logic assumes rectangular shapes for simplicity.

📬 Feedback
Feel free to fork this project and submit pull requests if you'd like to contribute or suggest improvements.

Happy sailing! ⛵
