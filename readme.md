<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Snake AI with Q-Learning and Pygame</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f8f9fa;
            color: #333;
            padding: 20px;
            max-width: 900px;
            margin: auto;
        }

        h1, h2 {
            color: #2c3e50;
        }

        h1 {
            text-align: center;
        }

        pre {
            background-color: #272822;
            color: #f8f8f2;
            padding: 15px;
            overflow-x: auto;
        }

        code {
            font-family: monospace;
        }

        ul {
            margin-left: 20px;
        }

        .badge {
            display: inline-block;
            padding: 3px 8px;
            background-color: #3498db;
            color: white;
            border-radius: 5px;
            font-size: 0.8em;
            margin-right: 5px;
        }

        a {
            color: #2980b9;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        .section {
            margin-bottom: 40px;
        }
    </style>
</head>
<body>

    <h1>Snake AI with Q-Learning and Pygame</h1>

    <div class="section">
        <p>An intelligent Snake game where the AI learns to play using <span class="badge">Q-learning</span>, with <span class="badge">body awareness</span> and <span class="badge">gradient visualization</span>. The AI navigates the grid, eats fruits, and avoids collisions with walls and itself.</p>
    </div>

    <div class="section">
        <h2>Features</h2>
        <ul>
            <li><strong>Q-learning AI:</strong> Trains the snake to make optimal moves.</li>
            <li><strong>Body awareness:</strong> Snake tracks its own body to prevent self-collisions.</li>
            <li><strong>Gradient visualization:</strong> Dark green head gradually fades to lighter green tail.</li>
            <li><strong>Head direction indicator:</strong> Arrow on the head shows current movement direction.</li>
            <li><strong>Game-over notifications:</strong> Terminal shows the reason for game over (boundary or self-collision).</li>
            <li><strong>Customizable grid size and speed.</strong></li>
        </ul>
    </div>

    <div class="section">
        <h2>File Structure</h2>
        <pre>
Snake-AI-Pygame/
│
├─ train_snake.py         # Q-learning training script
├─ play_snake.py          # Pygame AI play script
├─ q_table.pkl            # Saved Q-table after training
├─ README.md              # Project description
└─ requirements.txt       # Required Python packages
        </pre>
    </div>

    <div class="section">
        <h2>Getting Started</h2>
        <p>Follow these steps to run the Snake AI:</p>
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
    </div>

    <div class="section">
        <h2>Screenshots / GIFs</h2>
        <p>Add screenshots or GIFs here showing the AI snake in action.</p>
    </div>

    <div class="section">
        <h2>License</h2>
        <p>This project is open-source and free to use under the <strong>MIT License</strong>.</p>
    </div>

</body>
</html>
