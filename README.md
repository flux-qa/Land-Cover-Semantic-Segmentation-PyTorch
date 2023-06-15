<div align="center">
 
![logo](https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/assets/logo2.jpg)  

<h1 align="center"><strong>🛣 Land-Cover-Semantic-Segmentation-PyTorch:<h6 align="center">An end-to-end Image Segmentation (CV) project</h6></strong></h1>

![PyTorch - Version](https://img.shields.io/badge/PYTORCH-2.0+-red?style=for-the-badge&logo=pytorch)
![Python - Version](https://img.shields.io/badge/PYTHON-3.9+-blue?style=for-the-badge&logo=python&logoColor=white)
[![Generic badge](https://img.shields.io/badge/License-MIT-<COLOR>.svg?style=for-the-badge)](https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/LICENSE) 
[![GitHub Issues](https://img.shields.io/github/issues/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch.svg?style=for-the-badge)](https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/issues)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg?style=for-the-badge)

</div>

----
 
## 📚 Table of Contents
- [Overview](#overview)
- [Demo](#demo)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the project](#running-the-project)
- [Citing](#citing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

----

## 📌 Overview <a name="overview"></a>
An end-to-end Computer Vision project focused on the topic of <a href="https://en.wikipedia.org/wiki/Image_segmentation" target="_blank">Image Segmentation</a> (specifically Semantic Segmentation). Although this project has primarily been built with the <a href="https://landcover.ai.linuxpolska.com/" target="_blank">LandCover.ai</a> dataset, the project template can be applied to train a model on any semantic segmentation dataset and extract inference outputs from the model in a <b>promptable</b> fashion. Though this is not even close to actual promptable AI, the term is being used here because of a specific functionality that has been integrated here.

The model can be trained on any or all the classes present in the semantic segmentation dataset, thereafter the user can pass the prompt (in the form of the config variable '<b>test_classes</b>') of the selected classes that are expected to be present in the masks predicted by trained model.

The project has been built with the help of <a href="https://github.com/qubvel/segmentation_models.pytorch" target="_blank">Segmentation-Models-PyTorch</a>.

----

## 💫 Demo <a name="demo"></a>
 <p>
  1. Training the model on <a href="https://landcover.ai.linuxpolska.com/" target="_blank">LandCover.ai</a> dataset with '<b>train_classes</b>': <b>['background', 'building', 'woodland', 'water']</b>...
 </p>
 <p align="center">
  <img width="60%" src="https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/assets/training.png">
 </p>
 <p>
  2. Testing the trained model for all the classes used to train the model, i.e. '<b>test_classes</b>': <b>['background', 'building', 'woodland', 'water']</b>...
 </p>
 <p align="center">
  <img width="90%" src="https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/assets/all_classes.png">
 </p>
 <p>
  3. Testing the trained model for selective classes as per user input, i.e. '<b>test_classes</b>': <b>['background', 'building', 'water']</b>...
 </p>
 <p align="center">
  <img width="90%" src="https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/assets/select_classes.png">
 </p>

---

## 🚀 Getting Started <a name="getting-started"></a>

### ✅ Prerequisites <a name="prerequisites"></a>
 
 1. <b>Dataset prerequisite for training</b>:
 
 Before starting to train a model, make sure to download the dataset from <a href="https://landcover.ai.linuxpolska.com/" target="_blank">LandCover.ai</a> or from <a href="https://www.kaggle.com/datasets/adrianboguszewski/landcoverai" target="_blank">kaggle/LandCover.ai</a>, and copy/move over the downloaded directories 'images' and 'masks' to the 'train' directory of the project.
 
 2. <b>Programming environment prerequisite to run the project</b>:
 
 If using an installed <a hre="https://docs.conda.io/en/latest/">conda</a> package manager, i.e. either Anaconda or Miniconda, create the conda environment following the steps mentioned below:
 ```shell
 conda create --name <environment-name> python=3.9
 conda activate <environment-name>
 ```
 
 If using a directly installed python software, create the virtual environment following the steps mentioned below:
 ```shell
 python -m venv <environment-name>
 <environment-name>\Scripts\activate
 ```
 

### 💻 Installation <a name="installation"></a>
 
 1. Clone the repository:
 ```shell
 git clone https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch.git
 ```
 2. Change to the project directory:
 ```shell
 cd Land-Cover-Semantic-Segmentation-PyTorch
 ```
 3. Install the dependencies:
 ```shell
 pip install -r requirements.txt
 ```

### 🤖 Running the project <a name="running-the-project"></a>
 
 Running the model training and testing/inferencing scripts from the project directory. It is not necessary to train the model first mandatorily, as a simple trained model has been provided to run the test and check outputs before trying to fine-tune the model.
 
 1. Run the model training script:
 ```shell
 cd src
 python train.py
 ```
 2. Run the model testing/inferencing script:
 ```shell
 cd src
 python test.py
 ```

----

## 📝 Citing <a name="citing"></a>
```
@misc{Souvik2023,
  Author = {Souvik Majumder},
  Title = {Land Cover Semantic Segmentation PyTorch},
  Year = {2023},
  Publisher = {GitHub},
  Journal = {GitHub repository},
  Howpublished = {\url{https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch}}
}
```

----

## 🛡️ License <a name="license"></a>
Project is distributed under [MIT License](https://github.com/souvikmajumder26/Land-Cover-Semantic-Segmentation-PyTorch/blob/main/LICENSE)

---

## 👏 Acknowledgements <a name="acknowledgements"></a>
 - [qubvel/segmentation_models.pytorch](https://github.com/qubvel/segmentation_models.pytorch)
 ```
 @misc{Iakubovskii:2019,
  Author = {Pavel Iakubovskii},
  Title = {Segmentation Models Pytorch},
  Year = {2019},
  Publisher = {GitHub},
  Journal = {GitHub repository},
  Howpublished = {\url{https://github.com/qubvel/segmentation_models.pytorch}}
 }
 ```
 - [LandCover.ai](https://landcover.ai.linuxpolska.com/)
 - [bnsreenu/python_for_microscopists](https://github.com/bnsreenu/python_for_microscopists)
 - [leonardo.ai](https://leonardo.ai)

<p align="right">
 <a href="#top"><b>🔝 Return </b></a>
</p>

---
