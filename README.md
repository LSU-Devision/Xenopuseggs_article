Xenopus laevis Egg Counting using Deep Learning (StarDist)
===========================================================

Overview
--------
This project uses deep learning to automatically count frog eggs (Xenopus laevis) in images.
Developed through LSU’s Capstone Course in partnership with the Aquatic Germplasm and Genetic 
Resources Center (AGGRC), this tool replaces manual counting with an efficient, high-accuracy 
instance segmentation model using StarDist.

GitHub Repository: https://github.com/LSU-Devision/Xenopuseggs_article  
GUI Tool Repository: https://github.com/LSU-Devision/GUI

Key Features
------------
- Instance segmentation using StarDist (U-Net backbone)
- Trained and evaluated on 180+ annotated frog egg images
- Achieved 93% accuracy (120 training images, 150 epochs)
- Alternate model using only 114 annotated images with rotation-based augmentation

Folder Structure
----------------
- data/         : Input images and image masks
- models/       : Trained model weights
- scripts/      : Python scripts for training and testing
- figures/      : Graphs and visualizations of model performance

Installation
------------
1. Requires Python 3.8 or higher
2. Install dependencies:
   pip install -r requirements.txt

3. For the GUI (hosted separately), visit:  
   https://github.com/LSU-Devision/GUI  
   and follow its instructions to run the application.

How to Annotate Images
----------------------
- Use Fiji (ImageJ v1.54) with the Labkit plugin
- Manually outline each egg using the pencil tool
- Save the resulting mask as a .tif file


Dependencies
------------
- StarDist 0.8.5
- TensorFlow 2.10.0
- NumPy, SciPy, Pillow, Matplotlib
- scikit-learn, openpyxl, tkinter-tooltip
- ImageJ (Fiji) with Labkit plugin for annotation

Credits
-------
Developed by LSU students and faculty as part of the Math Capstone course.
Supervisors: Prof. Peter R Wolenski (Mathematics) and Dr. Yue Liu (AGGRC)


