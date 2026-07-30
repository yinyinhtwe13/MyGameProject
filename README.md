# Java Console Mini-Games Collection (MyGameProject)
A collection of classic text-based mini-games built in Java, showcasing fundamental programming concepts such as control flow, random number generation, input handling, and game loops.

## 🕹️ Included Games
- 🌲 **StoryAdventureGame** - A text-based RPG adventure game.
- 🎲 **DiceGame** - Classic dice rolling game.
- ❓ **JavaQuizGame** - Interactive quiz/trivia game.
- 🎰 **JavaSlotMachine** - Casino slot machine simulator.
- ✂️ **RockPaperScissorGame** - Classic Rock, Paper, Scissors game.

## 🌲 Story Adventure Game (Forest Adventure)
**StoryAdventureGame** is an interactive, text-based RPG where players explore a dark forest, make path choices, and engage in turn-based encounters with wild creatures.

### 🌟 Key Features & Gameplay Mechanics
1. **Player Personalization**: Takes the player's name via console input to personalize story messages.
2. **Branching Paths**: 
   - **Left Path**: Leads to a glowing cave.
   - **Right Path**: Leads down a dark forest trail.
3. **Randomized Combat System**:
   - Spawns a creature with random strength (1–10).
   - **Attack Option (1)**: Deals random damage (1–10). Victory occurs when creature strength drops to `0` or less.
   - **Run Option (2)**: 50% chance (`randomNumber >= 50`) to successfully escape to safety.
4. **Game Loop**: Employs a `do-while (chose1 != 0)` loop to continuously prompt action choices until the player either defeats the creature or escapes.

### 🎮 How to Play

1. **Enter Your Name**: Start your journey by entering your adventurer's name when prompted.
2. **Choose Your Path**:
   - Type `1` to go **Left** toward a glowing cave.
   - Type `2` to go **Right** down a dark forest trail.
3. **Face the Creature**: A wild creature with random strength (1–10) will block your way.
4. **Choose Your Combat Action**:
   - Type `1` (**Attack**): Deal random damage (1–10) to the creature. Keep attacking until its strength drops to `0` or less to win!
   - Type `2` (**Run**): Attempt to escape back to safety (50% chance of success).
5. **Win the Game**: Defeat the creature or successfully run away to survive the forest!
   
## ✂️ Rock Paper Scissors Game

A classic command-line implementation of the Rock-Paper-Scissors game where players play against a computer AI.

### 🌟 Key Features & Gameplay Mechanics

1. **Randomized AI Choice**: The computer randomly selects its move (`rock`, `paper`, or `scissors`) using Java's `Random` class and an array of available moves.
2. **Win / Tie / Lose Logic**: Compares player and computer inputs using `.equals()` combined with logical operators (`&&`, `||`) to evaluate outcomes accurately.
3. **Replay System**: Utilizes a `do-while` loop and `.equalsIgnoreCase("yes")` to allow seamless replay without restarting the program.
4. **Clean Exit & Resource Management**: Properly closes the `Scanner` stream upon user exit with a friendly farewell message.

### 🎮 How to Play

1. Enter your choice when prompted: `rock`, `paper`, or `scissors`.
2. View the computer's choice and the game result (`You win!`, `You lose!`, or `It's a tie!`).
3. Type `yes` to play another round, or `no` to exit the game.
