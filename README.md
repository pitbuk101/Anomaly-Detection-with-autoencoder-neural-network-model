# Anomaly-Detection-with-autoencoder-neural-network-model
Anomaly Detection with autoencoder neural network model




MCSA involves analyzing the current signature of a motor to detect changes in its characteristics, which can indicate the presence of faults such as rotor bar breakage, bearing wear, and misalignment. The technique is based on the fact that the current drawn by a motor is affected by the condition of the rotor and stator windings, as well as the load on the motor. By analyzing the frequency spectrum of the current signal, it is possible to detect changes in the signature that are indicative of specific types of faults.
I have used an autoencoder deep learning neural network model to identify vibrational anomalies from the sensor readings. The goal is to predict future failures/diffrent activity before they happen.
Here, we will use Long Short-Term Memory (LSTM) neural network cells in our autoencoder model. LSTM networks are a sub-type of the more general recurrent neural networks (RNN). A key attribute of recurrent neural networks is their ability to persist information, or cell state, for use later in the network. This makes them particularly well suited for analysis of temporal data that evolves over time

Dataset: The dataset has observations of a 3-phase AC motor(3.2hp).

Approach:
We will use an autoencoder neural network architecture for our anomaly detection model. The autoencoder architecture essentially learns an “identity” function. It will take the input data, create a compressed representation of the core / primary driving features of that data and then learn to reconstruct it again. 

The rationale for using this architecture for anomaly detection is that we train the model on the “normal” data and determine the resulting reconstruction error. Then, when the model encounters data that is outside the norm and attempts to reconstruct it, we will see an increase in the reconstruction error as the model was never trained to accurately recreate items from outside the norm.

