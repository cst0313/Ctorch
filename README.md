# Neural-network-in-C
## 📁  File structure
```
├── README.md                           // Readme
├── code
│   ├── Makefile                        // For easier compilation, type "make mnist" in cmd                    
│   ├── adam.c                          // code for Adam optimizer
│   ├── adam.h                          // header file for Adam optimizer                                                                            
│   ├── ann.c                           // code for neural network (create, predict, train)
│   ├── ann.h                           // header file for ann.c
│   ├── cnnlayer.c                      // code for Convolutional layers
│   ├── cnnlayer.h                      // header file for cnnlayer.c
│   ├── conv.c                          // operations for convolutional layers
│   ├── data.temp                       // temp file to store training data for graph plotting
│   ├── flattenlayer.c                  // flatten layer for CNN
│   ├── flattenlayer.h                  // header file for flatten layer
│   ├── helper.c                        // code for graph plotting
│   ├── helper.h                        // header file for helper.c
│   ├── layer.c                         // code for fully connected layers
│   ├── layer.h                         // header file for layer.c
│   ├── math_funcs.c                    // math functions, e.g. activation and loss functions
│   ├── math_funcs.h                    // header file for math_funcs.c
│   ├── math_r4t.c                      // operations on the r4t struct 
│   ├── math_r4t.h                      // header file for math_r4t.c
│   ├── math_structs.c                  // matrix operations
│   ├── math_structs.h                  // header file for math_structs.c
│   ├── mnist.c                         // Main program -- tests the DNN on the MNIST dataset
│   ├── tensor.c                        // implementation of Pytorch Tensors
│   ├── tensor.h                        // header file for tensor.c
│   ├── tensor_math.c                   // math operations on tensors
│   └── xor.c                           // testing program to test sigmoidal MLP to learn the XOR function. Use "make xor" to build.
├── data                                // Image data downloaded from official MNIST website
│   ├── test-images.idx3-ubyte          
│   ├── test-labels.idx1-ubyte
│   ├── train-images.idx3-ubyte
│   └── train-labels.idx1-ubyte
└── results
    ├── mnist_accuracy_100x100.png      // Accuracy graph for 2 hidden layers (100+100), both dropout 0.4, mini-batch GD
    ├── mnist_accuracy_100x100_adam.png // Accuracy graph for 2 hidden layers (100+100), only final hidden layer dropout 0.4, Adam optimizer (BEST)
    ├── mnist_accuracy_30x30.png        // Accuracy graph for 2 hidden layers (30+30), no dropout, mini-batch GD (INITIAL)
    ├── mnist_accuracy_60x60.png        // Accuracy graph for 2 hidden layers (60+60), both dropout 0.4, mini-batch GD
    ├── mnist_loss_100x100.png          // Same descriptions as above, but for loss graph (Mean Cross Entropy loss of the whole training set in each epoch)
    ├── mnist_loss_100x100_adam.png
    ├── mnist_loss_30x30.png
    ├── mnist_loss_60x60.png
    └── xor.png                         // Loss graph (MSE) for XOR network (1 hidden layer, 2 neurons)
```
## 🔢 Math and Logic

## 🔨 Build and Run

## 📊 Results

## 🚀 Future Improvements
 - Put more neurons in the hidden layers. I did not do that because my potato machine will probably explode.
 - Try to use GPU for matrix operations as it provides a significant speedup.
