<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/https://github.com/PointCloudSegementationOnALSandMLS">
    <img src="images/logo.PNG" alt="Logo">
  </a>

  <h3 align="center">Master Thesis - Point Cloud Segmentation of Urban Architectural Structures from Aerial and Mobile LiDAR Scans using Neural Networks
 </h3>

  <p align="center">
    This organization contains the main source code used and devloped for this master thesis. However, the scripts were often used in small deviations. Here we tired to adjust these to make them reusable by other persons. In any questions arise, please [contact](#contact) me. 
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



## Getting started



<!-- CONTACT -->
## Contact

GitHub: [Nick Jakuschona](https://github.com/NJaku01)  <br>
Mail:  <a href="mailto:nick.jakuschona@uni-muenster.de">nick.jakuschona@uni-muenster.de</a>



