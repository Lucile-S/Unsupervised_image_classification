# Unsupervised_image_classification

## Project
I will explore how I can give the computer a group of retine OCT images, and it can cluster the ones with the same patalogy together.

## DATA 

### Context 

Retinal optical coherence tomography (OCT) is an imaging technique used to capture high-resolution cross sections of the retinas of living patients. Approximately 30 million OCT scans are performed each year, and the analysis and interpretation of these images takes up a significant amount of time (Swanson and Fujimoto, 2017).

The figure below Represents Optical Coherence Tomography Images and the Workflow Diagram [Kermany et. al. 2018] http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5

<p align="center"><img src="Helper/och.png" width="840"\></p>

(A) (Far left) choroidal neovascularization (CNV) with neovascular membrane (white arrowheads) and associated subretinal fluid (arrows). (Middle left) Diabetic macular edema (DME) with retinal-thickening-associated intraretinal fluid (arrows). (Middle right) Multiple drusen (arrowheads) present in early AMD. (Far right) Normal retina with preserved foveal contour and absence of any retinal fluid/edema.

Optical coherence tomography (OCT) images (Spectralis OCT, Heidelberg Engineering, Germany) were selected from retrospective cohorts of adult patients from the Shiley Eye Institute of the University of California San Diego, the California Retinal Research Foundation, Medical Center Ophthalmology Associates, the Shanghai First People’s Hospital, and Beijing Tongren Eye Center between July 1, 2013 and March 1, 2017.

### Content
The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (NORMAL,CNV,DME,DRUSEN). There are 84,495 X-Ray images (JPEG) and 4 categories (NORMAL,CNV,DME,DRUSEN).

Images are labeled as (disease)-(randomized patient ID)-(image number by this patient) and split into 4 directories: CNV, DME, DRUSEN, and NORMAL.

<p align="center"><img src="Helper/nb_images_all_dataset.jpg" width="200"\></p>
<p align="center"><img src="Helper/training_images_by_cat.png" width="640"\></p>

In this project, I created a smaller dataset consisting of **2000 images from each directories, giving a total of 8000 images.**  


#### Distribution of Images Sizes 
The stats of images sizes by category show that the images have vastly different shapes. 
<p align="left"><img src="Helper/size_description.jpg" width="800"\></p>

## Image pre-processing  : 
Images are reading  as grayscale and resizing to 150x150.
The amount of features is reduced  to (8000, 22500)

## Ressources
For additional information: see http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5

Data: https://data.mendeley.com/datasets/rscbjbr9sj/2

Citation: http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5
