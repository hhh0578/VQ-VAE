# CVAE and VQ-VAE

This is an implementation of the VQ-VAE (Vector Quantized Variational Autoencoder) and Convolutional Varational Autoencoder.
 from [Neural Discrete representation learning](https://arxiv.org/pdf/1711.00937.pdf) for compressing MNIST and Cifar10.
The code is based upon [pytorch/examples/vae](https://github.com/pytorch/examples/tree/master/vae).

```bash
pip install -r requirements.txt
python main.py
```

## requirements
 - Python 3.6 (maybe 3.5 will work as well)
 - PyTorch 3.1
 - Additional requirements in requirements.txt

# Results

 - MNIST (k=10, d=64)
 ![mnist](/images/mnist.png)
 -CIFAR10 (k=128, d=256)
 ![CIFAR10](/images/cifar10.png)
 -Imagenet (k=512, d=128)
 ![imagenet](/images/imagenet.png)


# TODO:

- [ ] Implement [Continuous Relaxation Training of Discrete Latent Variable Image Models](http://bayesiandeeplearning.org/2017/papers/54.pdf) 

- [ ] Sample using PixelCNN prior

- [X] Improve results on cifar

- [X] Merge VAE and VQ-VAE for MNIST and Cifar to one script

# Acknowledgement
[tf-vaevae](https://github.com/hiwonjoon/tf-vqvae) for a good reference.
