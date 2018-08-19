# fast_style_transfer
Implemented fast style transfer for ML/AI practice (based on already existing work)

After finishing up the Deep Learning course from Coursera, I wanted to explore more work that was done in the area of style transfer 
(Gatys et al), which was an assignment for us in that course.

Turns out that a faster, better method based on training a feedforward network existed so I was interested in seeing how it works. I came across the work of Logan Engstrom here: https://github.com/lengstrom/fast-style-transfer

I looked over the code and implemented it a version of it in Jupyter notebooks. One notebook contains the code for training the network
and the other is for generating images based on the trained network.

Code used: Tensorflow 1.9 for GPU along with the requisite CUDA and CuDNN libraries on a Win10 machine with Ryzen 1600, 
16GB RAM and NVIDIA 1070. 

Takes approximately 580s for 1 epoch across 10000 images of the MSCOCO dataset. Trained for 30 epochs to get the results shown below.

Styles used:

![1](https://github.com/varunvprabhu/fast_style_transfer/blob/master/data/style/1.jpg)

![2](https://github.com/varunvprabhu/fast_style_transfer/blob/master/data/style/3.jpg)

Content Image:

![3](https://github.com/varunvprabhu/fast_style_transfer/blob/master/data/content/liberty.jpg)

Output images:

![4](https://github.com/varunvprabhu/fast_style_transfer/blob/master/data/generated/liberty_star.jpg)

![5](https://github.com/varunvprabhu/fast_style_transfer/blob/master/data/generated/liberty_wave.jpg)

Other implementations have trained over the entire MSCOCO dataset which would give better results. As mentioned before, this was an exploratory work on a great application of AI.

Citation
  @misc{engstrom2016faststyletransfer,
    author = {Logan Engstrom},
    title = {Fast Style Transfer},
    year = {2016},
    howpublished = {\url{https://github.com/lengstrom/fast-style-transfer/}},
    note = {commit xxxxxxx}
  }
  
LICENSE: see Logan Engstrom's github.


