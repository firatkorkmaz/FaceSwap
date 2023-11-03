# Face Swap with Delaunay Triangles
A program written in Jupyter Notebook to swap faces of people in multiple images by using Delaunay Triangles in Computer Vision.

## General Information
This is a step-by-step implementation of a Face Swap program by using Delaunay Triangles and 68 landmark detection functions of the **dlib** library. As a result, all the faces of people in multiple images in a destination folder are replaced with one single face chosen from a source image.

There are 5 Jupyter Notebook files which include 5 steps of the implementation to achieve the final program.

1. **1_Face_Detection.ipynb**: Simple face detection.
2. **2_GrayImage_Detector.ipynb**: Grayscale / Black & White image detection.
3. **3_Face_Colorization.ipynb**: Image colorization
4. **4_Single_Swapper[Explanation].ipynb**: Detailed explanation of the program by processing only two single files to swap one face in a source image with all the faces in a destination image.
5. **5_Multi_Swapper[Final_Program].ipynb**: FINAL program which swaps one face in a source image with all the faces in a folder of multiple destination images automatically.

* **./src/** folder will contain the model and wheel files, check: **./src/download.txt** 
* **./images/** folder contains the images which are used in the notebook files: 1-4.
* **./destination/** folder contains destination images where the source face will be swapped.
* **./destination_/** folder will be created to save the resulting images, it will be re-created on each run.

## Setup & Run
* Install the DLIB library by using the provided wheel (.whl) files in **./src/** folder:
```
For Python 3.9.x:
pip install ./src/dlib-19.22.99-cp39-cp39-win_amd64.whl

For Python 3.10.x:
pip install ./src/dlib-19.22.99-cp310-cp310-win_amd64.whl
```
* Then, install the libraries in **requirements.txt** file:
```
pip install -r requirements.txt
```
* Run Jupyter Notebook and open the Notebook files with it:
```
jupyter notebook
```