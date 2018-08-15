# Spikeduino
An event based neural network implementation for an arduino.

The C Program contains the code to be run on the chip. This code is 

(1) an implementation of a (small) balanced networks. I.e. synapses scale like 1/sqrt(K) where K is the indegree. The network is a random graph that is initialized with the build-in random number generator. The typical activity pattern is asynchronous and irregular.
(2) The Code generates Voltage-Pulses on the digital pins of the controller. Each pin corresponding to one neuron.
(3) The serial interface sends a continuous stream of numbers, corresponding to the index of the spiking cell. 


The Python Program allows to read the serial data stream, and plot it as an animation.
