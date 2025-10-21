<h1 align="center">🐍 Snake AI with Q-Learning and Pygame</h1>

<p align="center">
An intelligent Snake game where the AI learns to play using <strong>Q-learning</strong>, with <strong>body awareness</strong> and <strong>gradient visualization</strong>. The AI navigates the grid, eats fruits, and avoids collisions with walls and itself.
</p>

---

<h2>📖 Project Overview</h2>
<p>This project implements the classic Snake game in Python using Pygame, enhanced with an AI agent that learns to play using <strong>Q-learning</strong>. The AI can make intelligent decisions by understanding the environment, tracking its own body, and avoiding obstacles. The game features a visually appealing gradient-colored snake and directional indicators for the head.</p>

<h2>🎯 Motivation</h2>
<ul>
  <li>Learn and demonstrate <strong>Reinforcement Learning (RL)</strong> concepts.</li>
  <li>Create a fun AI agent that can autonomously play the Snake game.</li>
  <li>Visualize AI decision-making and game dynamics in real-time.</li>
</ul>

---

<h2>🧠 How the AI Works</h2>
<p>The AI uses a <strong>Q-learning</strong> algorithm to learn the optimal policy for collecting fruits and avoiding collisions. The key concepts are:</p>
<ul>
  <li><strong>State Representation:</strong> Each state consists of:
    <ul>
      <li>Head coordinates</li>
      <li>Fruit coordinates</li>
      <li>Blocked directions (up, down, left, right) to avoid collisions with walls or its own body</li>
    </ul>
  </li>
  <li><strong>Actions:</strong> Four possible moves: UP, DOWN, LEFT, RIGHT</li>
  <li><strong>Reward System:</strong>
    <ul>
      <li>+10 for eating a fruit</li>
      <li>-10 for hitting a wall or own body</li>
      <li>-0.1 for each step to encourage efficient movement</li>
    </ul>
  </li>
  <li><strong>Q-table:</strong> Stores the expected reward for each state-action pair. AI chooses the action with the highest Q-value at each step.</li>
</ul>

---

<h2>✨ Features</h2>
<ul>
  <li><strong>Q-learning AI:</strong> Learns optimal moves autonomously.</li>
  <li><strong>Body awareness:</strong> AI tracks its own body to prevent self-collisions.</li>
  <li><strong>Gradient visualization:</strong> Dark green head gradually fades to light green tail.</li>
  <li><strong>Head direction indicator:</strong> Arrow on the head shows current movement direction.</li>
  <li><strong>Game-over notifications:</strong> Terminal shows the reason for game over (hit boundary or self-collision).</li>
  <li><strong>Customizable grid size & speed:</strong> Easily modify GRID_SIZE and FPS.</li>
  <li><strong>Expandable AI:</strong> Can be upgraded to Deep Q-Networks for larger grids.</li>
</ul>

---

<h2>📂 File Structure</h2>
<pre>
Snake-AI-Pygame/
│
├─ train_snake.py         # Q-learning training script
├─ play_snake.py          # Pygame AI play script
├─ q_table.pkl            # Saved Q-table after training
├─ README.md              # Project description
└─ requirements.txt       # Required Python packages
</pre>

---

<h2>⚙️ Installation & Usage</h2>
<ol>
  <li><strong>Clone the repository:</strong>
<pre>git clone https://github.com/&lt;username&gt;/Snake-AI-Pygame.git
cd Snake-AI-Pygame</pre>
  </li>
  <li><strong>Install dependencies:</strong>
<pre>pip install pygame</pre>
  </li>
  <li><strong>Train the AI (optional):</strong>
<pre>python train_snake.py</pre>
  </li>
  <li><strong>Play using AI:</strong>
<pre>python play_snake.py</pre>
  </li>
</ol>

---

<h2>📷 Screenshots / GIFs</h2>
<p>Add screenshots or GIFs here showing the AI snake in action:</p>
<img src="snake_preview.gif" alt="Snake AI Preview" width="600">

---

<h2>🛠 Optional Enhancements</h2>
<ul>
  <li>Implement Deep Q-Network (DQN) for larger grids and faster learning.</li>
  <li>Allow multiple fruits or obstacles on the grid.</li>
  <li>Visualize Q-values as heatmaps for each move.</li>
  <li>Add continuous AI play with automatic resets after game over.</li>
</ul>

---

<h2>📄 License</h2>
<p>This project is open-source and free to use under the <strong>MIT License</strong>.</p>

<h2>🤝 Contribution</h2>
<p>Contributions, issues, and feature requests are welcome! Feel free to fork the repository and submit a pull request.</p>
