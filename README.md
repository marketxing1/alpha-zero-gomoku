# AlphaZero Gomoku
A multi-threaded implementation of AlphaZero

## Features
* Free-style Gomoku
* parallel MCTS with virtual loss/libtorch(Tree Parallelization and Root Parallelization)
* Gomoku and MCTS are written in C++
* swig wrap python extension

## Args
Edit config.py

## Environment

* Python 3.6+
* PyGame 1.9+
* PyTorch 1.0+
* LibTorch 1.0+
* MSVC14.00+/GCC4.8.2+
* CMake 3.0+
* SWIG 3.0+

## Run
```
# Add LibTorch/SWIG to environment variable $PATH

# Compile Python extension
mkdir build
cd build
cmake .. -DCMAKE_PREFIX_PATH=path/to/libtorch -DCMAKE_BUILD_TYPE=Release
cmake --build

# Run
cd ../test
python learner_test.py train # train model
python learner_test.py play  # play with human
```

## Pre-trained models
> Trained 12 hours on GTX1070

Link: https://pan.baidu.com/s/1c2Otxdl7VWFEXul-FyXaJA Password: e5y4

## GUI
![](https://github.com/hijkzzz/alpha-zero-gomoku/blob/master/assets/gomoku_gui.png)

## References
1. Mastering the Game of Go without Human Knowledge
2. Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm
3. Parallel Monte-Carlo Tree Search
4. An Analysis of Virtual Loss in Parallel MCTS
5. A Lock-free Multithreaded Monte-Carlo Tree Search Algorithm
6. github.com/suragnair/alpha-zero-general
