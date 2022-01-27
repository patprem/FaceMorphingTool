# Face Morphing between Two Real Images using StyleGAN2 and JoJoGAN

<!-- TABLE OF CONTENTS -->
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
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>

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

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

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
  
1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#top">back to top</a>)</p>
