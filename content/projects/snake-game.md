---
title: "Snake game training using Deep Reinforcement learning"
description: "Can a snake game train by itself to improve?"
dateString: Mar 2023 - May 2023
draft: false
tags: ["Python", "Tensorflow", "Keras", "Gym", "OpenCV", "DQNAgents", "AI"]
showToc: false
weight: 203
cover:
    image: "projects/automated-image-captioning/cover.jpg"
--- 
### 🔗 [Github link](https://github.com/fam33/Final-Project-INFO-550/tree/main)

## Description
In this project, I implemented the paper **[Show, Attend and Tell: Neural Image Caption Generation with Visual Attention](https://arxiv.org/abs/1502.03044)**. The neural network, a combination of **CNN** and **LSTM**, was trained on the **MS COCO** dataset and it learns to generate captions from images.

The project consists of a snake game implementation with a Deep Q Learning Agent on a Reinforcement Learning environment and is trained on neural networks. The repository consists of four files consisting of Snake Environment, implementation of DQNAgent, Test_the_Environment for checking if the environment is working and a training file to train the model.

As the network generates the caption, word by word, the model’s gaze (attention) shifts across the image. This allows it to focus on those parts of the image which is more relevant for the next word to be generated. 
![Attention Mechanism](/projects/automated-image-captioning/img1.jpg)

Furthermore, beam search is used during inference to enhance the prediction result. The network was trained in **PyTorch** on an **Nvidia GTX 1060** graphics card for over 80 epochs.