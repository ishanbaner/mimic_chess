# mimic_chess
Train a neural network to play like a chess player.

# An overview of the idea

Using Reinforcement learning, the bot learns to play like a specific player. 
The dataset must be in the pgn format and can be accessed from "Opening tree". 
The state space is the set of board positions and upon taking an action which is a legal move for a specific board position, a reward of +1 is given if it matches the player's move, otherwise 0. The Q value Q(s,a), is approximated by an FFN, much like Deep Q learning except it uses a single neural network. 
