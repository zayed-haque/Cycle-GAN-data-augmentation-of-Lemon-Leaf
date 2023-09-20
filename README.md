# Cycle GAN Data Augmentation of Lemon Leaf


## Introduction

This repository contains the implementation of CycleGAN for data augmentation of lemon leaf images. CycleGAN is a powerful technique for domain-to-domain image translation without the need for paired training data. Here, we leverage CycleGAN to augment lemon leaf images, generating diverse variations that can be used for training machine learning models. This project is in association with Tamil Nadu Famers Welfare Department.

## CycleGAN Model

The CycleGAN model is implemented in the `CycleGan` class, which is a subclass of TensorFlow's `Model`. It takes four input parameters - two generators and two discriminators - along with other optional configurations. The `compile` method sets up the optimizers and loss functions for training. The `train_step` method performs a single training step using the given batch data.

## Generator Model

The generator model is defined in the `generator_fn` function, which creates a CycleGAN generator network using TensorFlow's Keras API. The generator contains multiple encoder and decoder blocks, as well as transformer blocks, to learn the mapping between the two domains (lemon leaf images and augmented lemon leaf images).

## Discriminator Model

The discriminator model is defined in the `discriminator_fn` function, which creates a discriminator network based on the MobileNetV2 architecture. The discriminator takes an input image and predicts whether it belongs to the real or generated domain.

## Cycle Generated Images
![output](https://github.com/zayed-haque/Cycle-GAN-data-augmentation-of-Lemon-Leaf/assets/48508566/3c5e537a-8e95-4399-ab2d-84e0586e9f89)

## Disease Leaf Generated 
![output](https://github.com/zayed-haque/Cycle-GAN-data-augmentation-of-Lemon-Leaf/assets/48508566/10a229a7-8b2d-4f92-9393-5c78b25b9b1b)
