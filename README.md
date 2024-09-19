# A3C for Alien Game
This is a  Asynchronous Advantage Actor Critic (A3C) Reinforcement Learning model developed for the Alien game in the Gymnasium library.
 Convolutional Neural layers are considered to capture the features in the photos and then Recurrent Neural Layers (LSTM) are considered to capture the temporal dynamics of the game.

## Score Table
You can find the scores table from here: https://atariage.com/manual_html_page.php?SoftwareID=815

## Results
The attached videod demonstrate typical examples of how the agent moves in the game environment. 
On average, the obtained score was about 250 to 350. 

## Insights
One of the issues with this game, also mentioned by others here: https://github.com/Maskime/convolutional-dqn/tree/master is the frames in the environments.
Sometimes the stars are not shown in the right hand side of the frame, sometimes the agent disappears.
However, by using LSTM, our results improved significantly. I believe that by increasing the sequence length and the number of blocks in the LSTM layer, results will also improve due to the temporal dynamics captured by the LSTM.
