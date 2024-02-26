<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/PointCloudSegementationOnALSandMLS">
    <img src="https://github.com/PointCloudSegementationOnALSandMLS/.github/blob/main/profile/img/logo.png?raw=true" alt="Logo">
  </a>

  <h3 align="center">Master Thesis - Point Cloud Segmentation of Urban Architectural Structures from Aerial and Mobile LiDAR Scans using Neural Networks
 </h3>

  <p align="center">
    This organization contains the main source code used and devloped for this master thesis. However, the scripts were often used in small deviations. Here we tired to adjust these to make them reusable by other persons. In any questions arise, please contact me. 
The ALS and MLS datasets and pre-trained models on this datasets will be published shortly.
    <br/>
    
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
* [Implementation](#implementation)
* [Getting Started](#getting-started)
* [Contact](#contact)



<!-- ABOUT THE PROJECT -->
## About The Project
Digital Twins assist in urban planning decisions by enabling various analyses, such as assessing
noise pollution. As part of Digital Twins, three-dimensional representations of the real world
can be created using laser scanning. These scans can be conducted by airplanes, referred to
as aerial, or by vehicles, referred to as mobile. The result is an unstructured point cloud. In
order to utilize this data in different applications, it is essential to assign a semantic label to
each data point. Neural networks have shown considerable potential for semantically segment
point clouds. Nevertheless, this requires networks specifically designed for point clouds and
benchmark datasets to train and evaluate them. However, point clouds from aerial and mobile
laser scans are quite different for the same area due to different scanning angles and point
densities. Thus, there is a need to investigate whether aerial or mobile datasets are more
sufficient for the detection of specific classes, such as walls. We provide the first benchmark
dataset covering the same area by aerial and mobile laser scans to enable this research. Using
these datasets for network training has shown promising results in performing a segmentation
on them. Especially to assign points to the classes natural, buildings and cars. Identifying
vertical objects proved to be more challenging. When dealing with aerial data, it is beneficial
to group walls, fences, and hedges into a single class. However, for mobile data, it is more
advantageous to keep walls and fences as separate classes and include hedges in the natural
class. Further, segmentation on mobile scans allows the identification of road structures,
whereas on aerial scans it was useful to identify ground points.

<!-- Implementation -->
## Implementation
For the implementation we used the existing repositories [Open3D-ML](https://github.com/PointCloudSegementationOnALSandMLS/Open3D-ML) and [KPConv-Pytorch](https://github.com/PointCloudSegementationOnALSandMLS/KPConv-PyTorch). For both repositories we adapted the forks, reprsented in this organisation. Further we introduce the DataProcessingAndEvaluation repository, which contains, Data processing, visualization and evaluation scripts.

### Open3D
For the Open3D-ML package we added configurations and data loader scripts for the DALES dataset and our new intorduced Essen-ALS and Essen-MLS dataset. Further we did small adjustements in the weight calculations and the models itself.

The configurations can be found here: ml3d/configs/configs The data loader scripts are inside this folder: ml3d/datasets

Additionally we implemented two scipts: train_dataset.py and inference_dataset.py. These scripts were used for training and inferencing and we found that those scipts are missing in this repository.

### KPConv
For the KPConv dataset we implemented a data loader script for the DALES dataset and our new introduced Essen-ALS and MLS datasets. Further, we implemented training scripts for our Essen datasets. In these datasets also the configurations and parameter seettings are already included. In addition, we adapted the test scipt to also deal with our dataset.

### DataProcessingAndEvaluation
In this folder we provide different scripts we used during our thesis. For more information please stick to the Readme in this repository.
## Getting started
When you are generally interested in using point clouds and machine learning on these we suggest to orientate on the Open3D package. When interested in training the KPConv model please refer to the KPConv-Pytorch repository. When you are interested how we preprocessed our data and evaluated the results, have a look at our DataProcessingAndEvaluation repository. In general please gain further information on how to get started, from the Readmes of the different repositories.


<!-- CONTACT -->
## Contact

GitHub: [Nick Jakuschona](https://github.com/NJaku01)  <br>
Mail:  <a href="mailto:nick.jakuschona@uni-muenster.de">nick.jakuschona@uni-muenster.de</a>



