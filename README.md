# Play Flappy Bird using a Genetic Algorithm

This project aims to build a neural network architecture from scratch and train it using a genetic algorithm. The challenge was to do the genetic algorithm using ideas that I knew from biology like cross-over and mutation before learning about genetic algorithms formally.

## The algorithm that I used:
* A generation of birds is initialized each with a randomly weighted neural network (input, hidden layer, and output). The inputs to the neural networks are Distance to next pipe, height from the center of the next pipe, the Y position of the bird, and the Y velocity of the bird.
* The game is run until all of them die.
* The top n are used as parents for the next generation.
* The weights are arranged in an array (like a gene) then cross-over between random parents is used to generate new birds.
* Mutation is added to the process to allow for new discoveries.
* The games running are displayed, but at a high speed (as much as your computer can handle).

## You can change the settings used in the algorithm:
* Number of birds in generation is self explanatory. It is the number of birds used for the initial generation and each one following it.
* Number of parents is the variable n described above
* Hidden layer size is the number of neurons in the hidden layer
* Activation function is the activation function used in the neurons in the birds. You can select the sigmoid, tanh, or relu
* Mutation probability is the probability that any gene is mutated to a random value (a gene is a weight in the network)
* Max number of mutated genes is a cap used if you want to mutate a max number of genes
