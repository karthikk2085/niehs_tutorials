Deep Learning Tutorials for classification and segmentation in Medical Imaging
------------------------------------------------------------------------------

 This repository contains jupyter notebooks useful for model development for classification and segmentation


## Setup folders and google colaboratory:

Download this repository by clicking on 'Code' button and then on 'Download ZIP'. After downloading this repository in .zip format, unzip it using (7zip)[https://www.7-zip.org/download.html]. If you or on windows you can also right click on .zip file and click on 'Extract All' button to extract the contents of this repository to your local machine and if you or on mac you can also extract the contents of this repository by double clicking on the .zip file. After unzipping it, user needs to change the name of this repository from ('niehs_tutorials-master') to 'niehs_tutorials'. After signing in to your google account,please upload your unzipped folder into 'My Drive' in Google Drive. This should take couple of seconds to upload. After you upload the
this folder under you drive, go inside your folder in google drive and click on '+ New' button(![new](newbutton.PNG)) on top left corner > More > make sure you are able to see Google Colaboratory in the options, if you don't see it , click on 'Connect More Apps' > Search 'colaboratory' in the search bar and install it(After installing it, you should be able to see it in the installed  apps 'Google Colaboratory'). After installing google colaboratory to your drive, click on any of the jupyter notebooks(.ipynb files) and there you should be able to see that the jupyter notebook opened through google colaboratory.


## tb_not_tb_classification.ipynb:
This notebook serves as an example for binary classification  where we try to explore Chest X Rays(CXRs) and
develop prediction model to detect Tuberculosis or not.

In this notebook, we visualize the data, preprocess the CXRs (to contain **only the region of lungs** and remove  significant portions of the abdomen, neck, and head from standard CXRs), split the dataset to train/validation/test sets, develop a model using pretrained 'imagenet' weights and we will test them on their own test data to check the performance results.
We also check the robustness of the model  by testing the model on completely unseen variable data.

Description and setup about datasets used for this notebook are given in this notebook in a cell containing the heading as **Download the datasets (User can follow either of the options ).**

## lung_segmentation.ipynb:
This notebook serves as an example for  developing a deep learning segmentation model where we try to explore Chest X Rays(CXRs) and
develop segmentation model to segment lungs in the Chest X Rays.

In this notebook, we visualize the data, preprocess the CXRs (we combine right and left lung masks for a sample dataset, perform adaptive histogram equalization  ), split the dataset to train/validation/test sets, develop a model using basic UNet architecture and we will test them on their own test data to check the performance results.
We also check the robustness of the model  by testing the model on completely unseen variable data.

We use the Montgomery County dataset that is downloaded as part of step for previous notebook, for training the lung segmentation model.