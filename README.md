# Predicting the Dyssynchrony with LSTMs

### Goal: 
Using VCG simulations generated from Continuity, classify the corresponding dyssynchrony index, using
a LSTM recurrent neural network implemented in TensorFlow

### Dataset:
* 608 Simulations (More to come)
* 120 timesteps 
* 3 values per timestep (spatial coordinates)

### Run:
The program runs one single training step, with a batch of 20, using an Adam optimizer. Actual loss and 
accuracy may vary. 
``` 
>>> git clone https://github.com/jonathanhchiu/dyssynchrony_predictions.git
>>> virtualenv env
>>> source env/bin/activate
>>> pip install -r requirements.txt
>>> python lstm.py

Loss (before training): 1.833138.
Training Accuracy: 0.050000
Loss (after training): 1.495084.
Training Accuracy: 0.400000
```