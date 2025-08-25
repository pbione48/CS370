# CS370
# CS 370 Project Two – Pirate Intelligent Agent

This project implements a **Deep Q-Learning (DQN) agent** to solve a treasure-hunt maze game.  
The pirate agent learns a policy to navigate from random start positions to the treasure using reinforcement learning.

---

##  Work Completed
For this project, I implemented a reinforcement learning agent (the pirate) to navigate a maze and find treasure.  
- **Provided code:** `TreasureMaze.py` (maze environment), `GameExperience.py` (experience replay), and some skeleton helpers.  
- **My code:** Implemented the Deep Q-Learning components, including:
  - Training loop (`qtrain`)
  - Neural network model
  - Evaluation functions
  - Visualizations of the pirate’s path
  - Checkpoint saving/loading for long training  
- Trained the agent in chunks using checkpoints. While the agent showed progress, convergence to a consistently high win rate requires longer training runs beyond my current lab environment.

---

##  Connection to Computer Science
Computer scientists design, test, and refine solutions that apply computational thinking to real-world problems.  
This project demonstrates how reinforcement learning can solve sequential decision problems, which is a foundation for:
- Robotics  
- Gaming AI  
- Autonomous systems  

These same principles also power technologies like **self-driving cars, fraud detection, and recommendation systems.**

---

##  Problem-Solving Approach
I approached the problem like a computer scientist by:
1. Breaking it into smaller parts — environment setup, agent design, learning algorithm.  
2. Iterating through debugging and training in smaller chunks.  
3. Using systematic experimentation (adjusting epochs, replay buffer size, epsilon decay) rather than guessing.  

This mirrors **real-world engineering practice** where solutions are developed and tested incrementally.

---

##  Ethical Responsibilities
My responsibility is to ensure intelligent agents are used ethically:  
- AI must not create harm through bias or unsafe decisions.  
- Reinforcement learning agents deployed in real-world contexts must consider **human safety and transparency**.  
- As a developer, I must clearly communicate **limitations** (such as incomplete convergence in this project) and always prioritize the **end user’s well-being** while aligning solutions with organizational goals.  

---

##  How to Run
1. Clone this repository and open `TreasureHuntGame.ipynb` in Jupyter.  
2. Run all cells in order to:
   - Build and train the agent
   - Save/load checkpoints from the `checkpoints/` folder
   - Evaluate performance
   - Visualize the path taken by the agent  
3. If training disconnects, re-run from the last checkpoint and continue in chunks (e.g., `train_to(2000)`, `train_to(5000)`, etc.).

---

##  Results
- Training reached up to **epoch ~500+** with checkpoints saved.  
- The agent demonstrates the reinforcement learning process, though convergence to >80% win rate requires extended training.  
- Includes an evaluation cell to check win rate and a demo path from `(0,0)` to the treasure.  

---

##  References
- Russell, S., & Norvig, P. (2021). *Artificial Intelligence: A Modern Approach*.  
- Sutton, R. S., & Barto, A. G. (2018). *Reinforcement Learning: An Introduction*.  
- Silver, D., et al. (2016). *Mastering the game of Go with deep neural networks and tree search*. *Nature*.  

