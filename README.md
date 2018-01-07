Connecting:
1. Open Terminal and type ssh -i certificate.pem -L 8157:127.0.0.1:8888 ec2-user@ec2-34-203-218-157.compute-1.amazonaws.com
    1. If times out, look at aws and see what the IP is. Each reboot gets a new one. 
2. Run jupyter notebook (cd mynotebooks, jupyter notebook)
3. Open notebook in browser (https://127.0.0.1:8157)
4. Type in password



You can change dtype to torch.FloatTensor at the top of each notebook to use CPU instead of GPU.

# Deep image prior

In this repository we provide *Jupyter Notebooks* to reproduce each figure from the paper:

> **Deep Image Prior**

>Dmitry Ulyanov, Andrea Vedaldi, Victor Lempitsky


[[paper]](http://sites.skoltech.ru/app/data/uploads/sites/25/2017/11/deep_image_prior.pdf) [[supmat]](https://box.skoltech.ru/index.php/s/ib52BOoV58ztuPM) [[project page]](https://dmitryulyanov.github.io/deep_image_prior)

![](data/teaser_compiled.png)

Here we provide hyperparameters and architectures, that were used to generate the figures. Most of them are far from optimal. Do not hesitate to change them and see the effect.

We will expand this README with a list of hyperparameters and options shortly.

# Install

Here is the list of libraries you need to install to execute the code:
- [pytorch](http://pytorch.org/) > 0.2
- numpy
- scipy
- matplotlib
- scikit-image
- jupyter

All of them can be installed via `conda` (`anaconda`), e.g.
```
conda install jupyter
```

# Citation
```
@article{UlyanovVL17,
    author    = {Ulyanov, Dmitry and Vedaldi, Andrea and Lempitsky, Victor},
    title     = {Deep Image Prior},
    journal   = {arXiv:1711.10925},
    year      = {2017}
}
```
