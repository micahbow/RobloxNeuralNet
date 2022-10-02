# RobloxNeuralNet
A neural network ModuleScript and sample NEAT simulation application for training Roblox AI behavior via genetic mutation. 

The module code is within a single modulescript which can be called using `require` within other server scripts. Here are some highlighted features:
- `NNModule.NN.new` Construct a neural network by providing: 
  - A 2D array specifying layers and the number of nodes per layer
  - A 3D array specifying initial connection weights between layers
- `NNModule.NN.newRandom` Generate a random-topology neural network by providing:
  - The number of input and output nodes
  - The maximum number of layers and nodes per layer
- `NNModule.NN.newcopy` Create a copy of an existing neural network
- `NNModule.NN:Mutate` Mutate a neural network by randomly modifying a single weight
- `NNModule.NN:ForwardPropgate` Evaluate the output of the neural network given an input vector to map to input nodes
- `NNModule.NN:Render` Generate a physical model of the neural network with color coding and connection thicknesses to convey weights/values

Provided are some other scripts that were used to test the module in a NEAT application,  but you must first construct a simple testing rig:


![IMG_5309](https://user-images.githubusercontent.com/80184148/193438488-e83f70c3-4fab-47fb-9382-0489eb2e2023.gif)
