# Face Morphing between Two Real Images using StyleGAN2 and JoJoGAN

| Architecture | Source Image | Reference Image | Final Morphed Frame |
|     :---:    |     :---:    |     :---:       |       :---:         |
| StyleGAN2   | <img src="https://github.com/patprem/FaceMorphing/blob/f371afea1d6d1836f833a6bf4798bb8f2a8b30bb/images/source1.jpeg" width="175" height ="225"> | <img src="https://github.com/patprem/FaceMorphing/blob/33670150e51806e30896f8da9b7cb0ef8da4a7f5/images/target2.jpg" width="175" height ="225"> | <img src="https://github.com/patprem/FaceMorphing/blob/f371afea1d6d1836f833a6bf4798bb8f2a8b30bb/images/MorphedFrame.jpg" width="200" height ="225">
| JoJoGAN     | <img src="https://github.com/patprem/FaceMorphing/blob/f371afea1d6d1836f833a6bf4798bb8f2a8b30bb/images/source1.jpeg" width="175" height ="225"> | <img src="https://github.com/patprem/FaceMorphing/blob/33670150e51806e30896f8da9b7cb0ef8da4a7f5/images/target2.jpg" width="175" height ="225"> | <img src="https://github.com/patprem/FaceMorphing/blob/37b3b4a12fd634c7f37e17d5e890b6f838731e48/images/MorphedJoJo.png" width="200" height ="225"> |










<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

![Face Morph](https://github.com/patprem/FaceMorphing/blob/8c16d28a59b005727dc196e9c856011795c30faf/images/facemorph.png)

Get high-accuracy, developer-friendly automatic face morphing tool within minutes!

The main objective of this project is to morph between two real images and then produce a morph/transition video between the two pictures. To be more specific, this project aims to face morph a selfie image of a person into a passport photo style image such that the user has easy access to their passport data.

Why is this important?
* To obtain access to passport photo data easily without facing any identification issues.
* There are very few highly accurate face morphing tools out there in contemporary AI industry.
* To transform one form into another seemingly seamlessly.
* To overcome identity thefts that uses morphed facial images in identification documents.

Pleas check the following sections to get started.

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

This section lists the major frameworks/libraries and deep learning architectures used to bootstrap this project. 
* [StyleGAN2](https://github.com/NVlabs/stylegan2#readme)
* [JoJoGAN](https://arxiv.org/pdf/2112.11641.pdf)
* [OpenCV](https://opencv.org/)
* [PyTorch](https://pytorch.org/)
* [TensorFlow](https://www.tensorflow.org/)
* [wandb](https://docs.wandb.ai/)
* [scikit](https://scikit-learn.org/stable/)
* [NumPy](https://numpy.org/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started
This project uses both StyleGAN2 and JoJoGAN to observe and analyze the differences between the two architectures. Results from both models are illustrated to draw a conclusion, where JoJoGAN proves to perform much better than StyleGAN2. To make things easier and to deliver this project accessible to everyone, Google Colab is the primary platform used in this project.

### Prerequisites

The following lists the prerequisites required to kickstart the project:
* Google Colab
* Samples of selfie images and passport photo style images

### Installation

_The instructions to start this project are simple. The two files named as StyleGAN2.ipynb and JoJoGAN.ipynb are the two main notebooks used in this project._
1. StyleGAN2.ipynb: Used to perform face morphing using StyleGAN2 architecture.
2. JoJoGAN.ipynb: Used to perform face morphing using JoJoGAN architecture.

Both notebooks will just need to be downloaded and imported into Google Colab on your local machine for uploading your desired source and target images.

Few software will have to be installed into Colab, for the notebook to work. 
* StyleGAN2
  ```sh
  git clone https://github.com/NVlabs/stylegan2-ada-pytorch.git
  ```
* JoJoGAN
  ```sh
  git clone https://github.com/patprem/JoJoGAN.git
  ```
* ninja
  ```sh
  pip install ninja
  ```
* Preprocessing Tools
  ```sh
  wget http://dlib.net/files/shape_predictor_5_face_landmarks.dat.bz2
  bzip2 -d shape_predictor_5_face_landmarks.dat.bz2
  ```
  
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

This section illustrates the results from both StyleGAN2 and JoJoGAN architectures for visualization and comparison purposes.





For instance, the below image is the source image that we wish to morph into passport photo style.
<img src="https://github.com/patprem/FaceMorphing/blob/f371afea1d6d1836f833a6bf4798bb8f2a8b30bb/images/source1.jpeg" width="200" height ="250">

And, the target image (passport photo style image) is shown below.
<img src="https://github.com/patprem/FaceMorphing/blob/f371afea1d6d1836f833a6bf4798bb8f2a8b30bb/images/target1.jpg" width="200" height ="250">

The final morphed frame is shown as:






<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
This code borrows snippets of code from [StyleGAN2 Morph Between Two Real Images, John Heaton](https://github.com/jeffheaton/stylegan2-toys) and [JoJoGAN: One Shot Face Stylization](https://github.com/mchong6/JoJoGAN) and rewritten to incorporate into my project.

<p align="right">(<a href="#top">back to top</a>)</p>
