# Face Morphing between Two Real Images using StyleGAN2 and JoJoGAN
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
    <li><a href="#contribute">Contribute</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a>
    
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

Please check the following sections to get started.

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

This section lists the major frameworks/libraries and deep learning architectures used to bootstrap this project. 
* [StyleGAN2](https://github.com/NVlabs/stylegan2#readme)
* [JoJoGAN](https://arxiv.org/pdf/2112.11641.pdf)
* [OpenCV](https://opencv.org/)
* [PyTorch](https://pytorch.org/)
* [TensorFlow](https://www.tensorflow.org/)
* [wandb](https://docs.wandb.ai/)
* [Matplotlib](https://matplotlib.org/)
* [scikit](https://scikit-learn.org/stable/)
* [NumPy](https://numpy.org/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started
This project uses both StyleGAN2 and JoJoGAN to observe and analyze the differences between the two architectures. Results from both models are illustrated to draw a conclusion, where JoJoGAN proves to perform much better than StyleGAN2. To make things easier and to deliver this project accessible to everyone, Google Colab is the primary platform used in this project.

**Everything to get started with this project are provided in these two Google Colab notebooks:**
1. Face Morphing using StyleGAN2: [FM StyleGAN2](https://github.com/patprem/FaceMorphingTool/blob/b39a13ceb85393e2b86850fcc82456f687bfca8f/StyleGAN2.ipynb)
2. Face Morphing using JoJoGAN: [FM JoJoGAN](https://github.com/patprem/FaceMorphingTool/blob/b39a13ceb85393e2b86850fcc82456f687bfca8f/JoJoGAN.ipynb)

### Prerequisites

The following lists the prerequisites required to kickstart the project:
* Google Colab account
* Samples of selfie images and passport photo style images

### Installation

_The instructions to start this project are simple. The two files named as StyleGAN2.ipynb and JoJoGAN.ipynb are the two main notebooks used in this project._
1. StyleGAN2.ipynb: Used to perform face morphing using StyleGAN2 architecture.
2. JoJoGAN.ipynb: Used to perform face morphing using JoJoGAN architecture.

_Both notebooks will just need to be downloaded and imported into Google Colab on your local machine for uploading your desired source and target images or simply click on the notebook links provided under Prerequisities section._

_Few software will have to be installed into Colab, for the notebook to work. 
**NOTE: The following commands are already pre-typed in the above Colab notebooks.**_
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
| Architecture | Source Image | Reference Image | Final Morphed Frame |
|     :---:    |     :---:    |     :---:       |       :---:         |
| StyleGAN2   | <img src="https://github.com/patprem/FaceMorphing/blob/633c647236458583bbe16c3be4282a3f9463fe3b/images/Selfie1.jpeg" width="150" height ="200"> | <img src="https://github.com/patprem/FaceMorphing/blob/33670150e51806e30896f8da9b7cb0ef8da4a7f5/images/target2.jpg" width="150" height ="200"> | <img src="https://github.com/patprem/FaceMorphing/blob/633c647236458583bbe16c3be4282a3f9463fe3b/images/MorphedStyleGAN.jpg" width="200" height ="200">
| JoJoGAN     | <img src="https://github.com/patprem/FaceMorphing/blob/633c647236458583bbe16c3be4282a3f9463fe3b/images/Selfie1.jpeg" width="150" height ="200"> | <img src="https://github.com/patprem/FaceMorphing/blob/633c647236458583bbe16c3be4282a3f9463fe3b/images/Target1.jpg" width="150" height ="200"> | <img src="https://github.com/patprem/FaceMorphingTool/blob/3a68a10a6fcccf707824c5bb89f10d19724ec9dd/images/MorphedJoJo.png" width="200" height ="200"> |

The below depicts the transition video for the same selfie image obtained using **StyleGAN2** model. The final morphed frame is the frame seen halfway through the video.
<p align="center">
  <img src="https://github.com/patprem/FaceMorphing/blob/fb48b08a97a0c36d9e9ec3b33d0c4c4379d2c86f/transition_videos/FaceMorph_Source1.gif" width="275" height="300" />
</p>

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTE -->
## Contribute

If you like this project and interested to contribute:
* Please show your support by ⭐ (star) the project.
* Submit pull requests and improve the repo overall quality.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
The codes used in this project borrows snippets of code from [StyleGAN2 Morph Between Two Real Images, John Heaton](https://github.com/jeffheaton/stylegan2-toys) and [JoJoGAN: One Shot Face Stylization](https://github.com/mchong6/JoJoGAN) and rewritten to incorporate into my project.

<p align="right">(<a href="#top">back to top</a>)</p>
