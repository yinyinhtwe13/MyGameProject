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

## 🎲 Dice Game

A fun console application that simulates rolling custom amounts of 6-sided dice, featuring ASCII art graphics for visual representation of each die face.

### 🌟 Key Features & Gameplay Mechanics

1. **ASCII Art Visualization**: Uses Java's multiline text blocks (`"""..."""`) to render clear ASCII art graphics for dice faces 1 through 6.
2. **Modern Switch Syntax**: Utilizes modern Java `switch` arrow expressions (`case 1 -> ...`) to map roll values to their corresponding ASCII graphic seamlessly.
3. **Dynamic Multi-Dice Rolling**: Allows players to roll multiple dice at once using a `for` loop based on user input.
4. **Input Validation & Total Calculation**: Validates that the number of dice requested is greater than `0`, keeps track of each individual roll, and computes the grand total.

### 🎮 How to Play

1. Enter the number of dice you wish to roll when prompted (must be greater than 0).
2. Watch the console print the visual ASCII die face and numeric value for each roll.
3. Review the combined sum/total score of all rolled dice!


## ❓ Java Quiz Game

An interactive console-based trivia quiz game testing knowledge on Computer Science, Networking, Cybersecurity, and Software Development concepts.

### 🌟 Key Features & Gameplay Mechanics

1. **2D Array Option Mapping**: Utilizes a 1D array for questions (`Questions[]`) and answer keys (`answers[]`), paired with a 2D array (`Options[][]`) to cleanly structure and render multiple-choice options.
2. **Computer Science Knowledge Test**: Features 10 tech-focused questions covering operating systems, networking (HTTP/HTTPS, IP masks), databases (SQL), and data structures.
3. **Real-Time Answer Evaluation**: Compares player input (`guess`) against stored answer keys in real time, giving instant visual feedback (`Correct!` or `Wrong!`).
4. **Score Tracking System**: Accurately tracks accumulated points throughout the quiz and displays the final score out of 10 upon completion.

### 🎮 How to Play

1. Read the Computer Science/IT question displayed on the console.
2. Enter your guess by typing a number from `1` to `4` corresponding to your choice.
3. Receive instant feedback after each response.
4. Complete all 10 questions to reveal your total score!

## 🎰 Java Slot Machine

A console-based slot machine game featuring customizable bets, interactive emoji reels, balance tracking, and dynamic payout multipliers for matching combinations.

### 🌟 Key Features & Gameplay Mechanics

1. **Emoji Reel Representation**: Uses an array of UTF-8 fruit and food emojis (`🍓`, `🍒`, `🍋`, `🍄`, `🥑`) to simulate visual slot machine reels in the terminal.
2. **Dynamic Payout Multipliers**:
   - **3 Matching Symbols**: Triggers a **3x payout** (`betAmount * 3`).
   - **2 Matching Symbols**: Triggers a **2x payout** (`betAmount * 2`).
   - **No Matches**: Forfeits the wagered bet.
3. **Smart Balance & Bet Validation**: Validates user bets against the active balance (`betAmount > currentBalance`), preventing invalid entries and auto-terminating the game when out of funds.
4. **Interactive Replay Loop**: Implements a `do-while` loop paired with user input sanitization (`toUpperCase().charAt(0)`) to allow seamless continuous rounds.

### 🎮 How to Play

1. Start with an initial virtual balance of **$100**.
2. Enter your wager amount for the spin (must not exceed your active balance).
3. Watch the 3 reels spin and display random emoji combinations.
4. Collect your payouts for matching 2 or 3 symbols, or keep spinning until you choose to quit or run out of money!
   
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
