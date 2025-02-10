
---

# Guessing Game in Rust

Welcome to the **Guessing Game** implemented in Rust! This is a simple console-based game where the player guesses a randomly generated number between 1 and 100. The game provides feedback on whether the guess is too small, too big, or correct.

---

## Table of Contents
- [Guessing Game in Rust](#guessing-game-in-rust)
  - [Table of Contents](#table-of-contents)
  - [How to Play](#how-to-play)
  - [Installation](#installation)
  - [Running the Game](#running-the-game)
  - [Code Structure](#code-structure)
  - [Dependencies](#dependencies)
  - [License](#license)

---


## How to Play

1. The program generates a random number between 1 and 100 (the "secret number").
2. The player is prompted to input their guess.
3. The program compares the guess to the secret number and provides feedback:
   - **Too small!**: The guess is lower than the secret number.
   - **Too big!**: The guess is higher than the secret number.
   - **You win!**: The guess matches the secret number.
4. The game ends when the player guesses the correct number.

---

## Installation

To run this game, you need to have Rust installed on your system. If you don't have Rust installed, follow these steps:

1. Install Rust by following the official guide: [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install).
2. Verify the installation by running:
   ```bash
   rustc --version
   ```
3. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/wali-hu/Guessing-Game-in-Rust.git
   ```
4. Navigate to the project directory:
   ```bash
   cd guessing-game
   ```

---

## Running the Game

1. Build and run the game using Cargo:
   ```bash
   cargo run
   ```
2. Follow the on-screen instructions to play the game.

---

## Code Structure

The project consists of a single Rust file (`main.rs`) with the following structure:

- **Dependencies**:
  - `rand`: Used to generate a random number.
  - `std::cmp::Ordering`: Used to compare the player's guess with the secret number.
  - `std::io`: Used to handle user input.

- **Main Logic**:
  - The program generates a random number using `rand::thread_rng().gen_range(1..=100)`.
  - A loop continuously prompts the player for input until they guess the correct number.
  - The player's input is parsed and compared to the secret number using a `match` statement.

---

## Dependencies

This project uses the following external crate:

- **`rand`**: A Rust library for random number generation. It is included in the `Cargo.toml` file.

To add the `rand` crate to your project, include the following in your `Cargo.toml`:

```toml
[dependencies]
rand = "0.8"
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Enjoy playing the game, and happy coding! 🚀

---

