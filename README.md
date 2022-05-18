## BipedalWalkerDDPG

This project is my own implementation of DDPG [Paper](https://arxiv.org/pdf/1509.02971.pdf) for solving continuous control problem in the Bipedal Walker environment of OpenAI Gym.


![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/70597091/169095991-772f321e-d997-4f1e-8b5b-9b9b72156d02.gif)

## Overview

This project attempts to learn a walking gait for 2D Bipedal Walker in OpenAI Gym Environment. (Note: The reward function is already implemented in the gym environment). The original implementation requires Ornstein-Uhlenbeck process for exploration but in my experiment I've used a gaussian noise of 0.2 stddev. 

In the training process, first 1000 steps of data is collected by randomly sampling actions from action space. This data acts as pure exploration. After this 1000 steps, we use (Policy Network's prediction + Gaussian Noise) as our action.

## Requirements

This project requires following dependencies:
1) Python
2) Tensorflow
3) Numpy
4) OpenAI Gym
5) Jupyter Notebook (optional; code from each cell can be copied to create .py file)

## Trying Out

For trying out download the weights and the main file [BipedalDDPG.ipynb](https://github.com/HimGautam/BipedalWalkerDDPG/blob/main/BipedalDDPG.ipynb). Run all the cells except the one with #Training comment on it.
