🎰 Python Slot Machine Game

A simple command-line slot machine simulator built in Python.
Players can deposit money, choose the number of lines to bet on, place wagers, and spin the slot machine to test their luck!

🧩 Features

-> 💰 Deposit and track your balance

-> 🎯 Choose how many lines to bet on (1–3)

-> 💵 Place custom bets within set limits

-> 🎡 Randomized slot machine spins

-> 🏆 Calculates winnings based on matching symbols and payout values

-> 🔁 Continue playing until you choose to quit

🖥️ Gameplay Overview
1. Deposit an amount of money to start.
2. Choose the number of lines to bet on (up to 3).
3. Place your bet per line (between $1 and $100).
4. Spin the slot machine to reveal random symbols.
5. Win if matching symbols appear across a line!
6. Keep playing until you decide to quit.

⚙️ Game Rules

  Max Lines: 3
  
  Min Bet: $1
  
  Max Bet: $100
  
  Slot Machine Size: 3x3 grid
  
 The fewer times a symbol appears, the higher its value!

🧠 How Winnings Work

-> You win if all symbols in a row match across all columns.

-> Your payout is calculated as:

Winnings = Symbol Value × Bet Amount

Example:
If you bet $10 on one line and hit 3 A’s in a row, you win:
5 (value of A) × 10 = $50

🧾 Example Gameplay

What would you like to deposit? $100

Enter the number of lines to bet on (1-3)? 3

What would you like to bet on each line? $5

You are betting $5 on 3 lines. Total bet is equal to: $15

D | C | D

A | A | A

C | B | D

You won $25.

You won on lines: 2

Press enter to play (q to quit).


🛠️ Code Structure
Copy code


slot_machine.py

│
├── check_winnings()       # Checks for winning lines and calculates payout

├── get_slot_machine_spin()# Randomly generates slot results

├── print_slot_machine()   # Displays slot machine visually

├── deposit()              # Handles user deposit

├── get_number_of_lines()  # Prompts for number of bet lines

├── get_bet()              # Prompts for bet per line

├── spin()                 # Runs a single round of the game

└── main()                 # Main game loop


