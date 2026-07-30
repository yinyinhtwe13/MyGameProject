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
