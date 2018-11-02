# Tensor-Super-Resolution-Model
This repository is the implement of the following paper:<br>
>Tensor Sparse Coding for Generating High-granularity 3D Seismic Data      

In this paper, we propose a seismic trace interpolation method based on tensor sparse coding for 3D seismic data, that training a high-granularity dictionary and a low-granularity dictionary.<br>

## Ditionary training model
The training model for low- and high-granunarity dictionaries pair show in the figure.<br>
![model](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/0.png?raw=true)<br>
run `D_Training.m` in `SR` file for training the dictionaries pairs, get the low- and high-granularity dictionaries `Dh` and `Dl` in the file `Dictionary`. 

## Evaluation
run `Demo_seismic_SR.m` for generating high-granularity seismic data.
This figure is the Original Seismic Data<br>
![Original Seismic](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/ori.png?raw=true
)<br>
This figure is the low-granularity Seismic Data<br>
![low-granularity](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/smp.png?raw=true)<br>
This figure is the high-granularity Seismic Data generated by our method<br>
![high-granularity](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/gen.png?raw=true)<br>
This figure is the high-granularity Seismic Data generated by GAN, This is the implement of the following paper:<br>
>Ledig C, Wang Z, Shi W, et al. Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network[C]// Computer Vision and Pattern Recognition. IEEE, 2017:105-114.<br>
![high-granularity](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/gan.png?raw=true)





This is the two methods to generating high-granularity seismic dara for single trace.<br>
![SR Error](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/ERR.png?raw=true)<br>
![](https://github.com/hust512/Tensor-Super-Resolution-Model/blob/master/SR/Figures/final.png?raw=true)
