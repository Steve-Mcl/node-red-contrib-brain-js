# node-red-contrib-brain-js

This node provides neural networks.
It is based on [brain.js](https://github.com/harthur-org/brain.js)

### Install

From your node-red directory:

npm install node-red-contrib-brain-js

or

in the Node-red, Manage palette, Install node-red-contrib-brain-js

### Usage

This node provides neural networks.<br>
At first you need to see the [brain.js](https://github.com/harthur-org/brain.js) documentation<p>

The following neural networks are available :<p>

- Feedforward Neural Network with backpropagation.
- Recurrent Neural Network
- Long Short Term Memory Neural Network
- Gated Recurrent Unit

### Training

The training data need to be stored in **msg.trainData** and the format is described [here](https://github.com/harthur-org/brain.js#training).<br>
The network options can be provided in **msg.neuralNetworkOptions**.

When the training is done, the network is available in **msg.net** and can be stored to be imported next time.

### Run

The running data need to be stored in **msg.runData**.<p>

The result is available in **msg.decision**.

### Import network

When the input message contains **msg.netJSON**, the network is loaded from the JSON provided.

### License

MIT License
