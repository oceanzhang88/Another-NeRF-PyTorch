# Another **NeRF** PyTorch
This is a re-implementation of ECCV 2020 paper [NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis.](https://arxiv.org/abs/2003.08934) 

The auhtor also makes a Tensorflow version here: [NeRF Tensorflow](https://github.com/bmild/nerf)



## About
This project is a concise NeRF re-implementation that follows closely with the original implementation.

## Data

- The official NeRF data repository is here [link](https://drive.google.com/drive/folders/128yBriW1IG_3NJ5Rp7APSTZsJqdJdfc1) 
- download ```nerf_synthetic``` folder.
- Place the ```nerf_synthetic``` folder inside the main project directory.

## Result

Final rendered images from out project:

&nbsp; &nbsp; &nbsp; <img src="media/final_gif/chair.gif" height="250" width="250"> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<img src="media/final_gif/ship.gif" height="250" width="250"> &nbsp; &nbsp; &nbsp;


## How to Train

#### Run ```Train.py```.

Running ```Train.py``` you will see prompts to select a test image index.

After running  ```Train.py``` you will see 3 folders under the main  directory. 

1. ```noval_view/instance_xxx/```
  - novel view image by NeRF is stored here. 

2. ```models/instance_xxx/```
  - Models are saved in this directory. 

3. ```runtime/instance_xxx/```
  - Enter ```tensorboard --logdir PATH_TO_PROJECT_DIRECTORY/runtime``` to monitor the runtime logs during training.
  


## Inference

#### Run ```Inference.py```

After running ```Inference.py``` you will see prompts to specify instance name, rendering size, and latitude angle.




## Additional GIF

<img src="media/final_gif/lego_0angle.gif" height="250" width="250"> &nbsp; &nbsp; &nbsp;
<img src="media/final_gif/lego.gif" height="250" width="250"> &nbsp; &nbsp; &nbsp;
<img src="media/final_gif/lego_60angle.gif" height="250" width="250">

image1: 0 degree, image2: 30 degrees, image3: 60 degrees


