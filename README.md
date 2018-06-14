<p align="center"><img width="40%" src="./assests/logo.jpg" /></p>

--------------------------------------------------------------------------------

## Overview

This project is fork of TensorFlow implementation of [StarGAN](https://arxiv.org/abs/1711.09020). StarGAN is a unified Generative Adversarial Networks (GANs) for multi-domain image-to-image translation. What this means is, StarGAN can flexibly translate an input image to any desired target domain using only a single generator and a discriminator. You can take a look at the demo video for StarGAN [here](https://www.youtube.com/watch?v=EYjdLppmERE).

## Requirements
* Tensorflow 1.8
* Python 3.6

## Usage
### Downloading the dataset
```python
> python download.py celebA
```

```
├── dataset
   └── celebA
       ├── train
           ├── 000001.jpg 
           ├── 000002.jpg
           └── ...
       ├── test (It is not celebA)
           ├── a.jpg (The test image that you wanted)
           ├── b.png
           └── ...
       ├── list_attr_celeba.txt (For attribute information) 
```

### Train
* python main.py --phase train

### Test
* python main.py --phase test 
* The celebA test image and the image you wanted run simultaneously

### Pretrained model
* Download [checkpoint for 128x128](https://drive.google.com/open?id=1ezwtU1O_rxgNXgJaHcAynVX8KjMt0Ua-)

## Summary
![overview](./assests/overview.PNG)

## Results (128x128, wgan-gp)
### Women
![women](./assests/women.png)

### Men
![men](./assests/men.png)

## Reference
* [StarGAN paper](https://arxiv.org/abs/1711.09020)
* [Author pytorch code](https://github.com/yunjey/StarGAN)

## Author
Junho Kim
