# CS6910_Assignment3
Contains code for Assignment 3 based on RNNs,LSTMs,GRUs for CS6910 - taught by Dr. Mitesh M. Khapra, IIT MADRAS

In this project I implemented a sequence to sequence model for learning problems using Recurrent Neural Networks, compare different cells such as vanilla RNN, LSTM and GRU, implement attention networks to overcome the limitations of vanilla seq2seq model and visualise the interactions between different components in an RNN based model. I used wandb for hyper parameter configuration using the validation dataset and visualisation of test data.

The codes are implemented for both vanilla sequence to sequence and With attention. I have used Tamil Language for the model.

Questions 1 to 7 are in Main.ipynb
To test the model use
```python
model = besttest(emb_dimension=256, neuron=256, dropout=0.2, no_of_layers=3, layer="LSTM", att=False, teacher_forcing=1.0)
```

To train the model use
```python
wandb.agent(sweep_id, function=train)
```
Question 8 is iin song.ipynb
