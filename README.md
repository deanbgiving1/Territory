Welcome to my program of the game Territory. This was written with Python 3.13, older versions might not work.
Don't change any folder or file names

To install the necessary libraries, run the following command in your command prompt: pip install -r requirements.txt

To run the game, open command prompt and locate the directory which you saved the "territory" folder on your computer. For example
C:\Users\yourname\Downloads\territory>
If command prompt opens in C:\Users\yourname>, use 'cd downloads/territory' to get there.

Once in the correct directory, run 'python main.py' and the game should start. It may be helpful to keep the command prompt open for the print statements that assist in playing the game

The AI uses Q-learning, a machine learning technique that evaluates previous game states to determine the best moves. The AI stores these evaluations in a Q-table and selects moves based on the highest Q-value. To get the q table I ran simulations and stored the game data from those. To train the AI yourself try 'python train_q_learning_ai.py' 

By default it will run 50 games, but you can change this by opening the .py file and finding

if __name__ == "__main__":
    train_q_learning_ai(episodes=50)   <-- change this number 

After each game finishes, the game data is logged and the q table is updated. As the Q-table grows with more simulations, it may be more intensive on your computer. It’s recommended to limit the number of simulations when training the AI, as the q table file will grow with each new boardstate logged.

UPDATE -- Added Improved UI!

Program created by Dean Carpenter. drcarpenter234@gmail.com
