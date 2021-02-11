# Image_Processing 
This is one of the assignment of Princeton University based on Image Processing

1) I try to process certain input images based on certain features and filters. As a reference follow this link:                
https://www.cs.princeton.edu/courses/archive/spring14/cos426/assignment1/examples.html

2) OS - Windows, IDE - Pycharm. One can use Anaconda Platforms (Spider, Jupiter notebook etc.) 

``` Pre-requirements for this project ```
1) Create a virtual environment {both for Anaconda, Pycharm}. 
  1.1) For anaconda using command line refer: 
       https://salishsea-meopar-docs.readthedocs.io/en/latest/work_env/python3_conda_environment.html
  1.2) For Pycharm IDE, please refer:
       https://arcade.academy/venv_install/index.html

2) Using command line, cd: to reach into virtual environment. Example = 'D:\Datasets\pythonProject\Princeton_IP\img_pro' {where img_pro is my vr name}. (Change path accordingly)
4) Manually install packages using PIP - NumPy, PILLOW, OpenCV 
   pip install opencv-python numpy PIL 
   'OR' 
   pip install -r requirment.txt
5) All the scripts lies here: 'D:\Datasets\pythonProject\Princeton_IP\img_pro'


```PYTHON CODE  File Structure```
1) output/ - Empty to start. Automatically writes the output images produced by the program into this folder with filter or option used. Do have a look before start
2) input/ - contains sample images for experimentation. 

Command Line Argument
```1. pmake.py - Python file to run the functions like {bright, contrast, blur, scale}
USAGE: python pmake.py -i<image_path>.<extention> -o <option> -f1<int_factor> -f2 <factor2>
Foe bright : python pmake.py --image princeton_small.jpg -o bright -f1 4
For contrast: python pmake.py --image c.jpg -o contrast -f1 -1.0 
Or
python pmake.py -i input.png


2. filter.py - Python file for convolution functions
USAGE: python filter.py --image <image name>.<extention> -k <kernelname> 
or 
#python filter.py --image <image name>.<extention>

Example to run Sharpen:
python filter.py --image princeton_small.jpg -k sharpen
Gaussian blur: python filter.py --image princeton_small.jpg -k gaussian blur
EDGE: python filter.py --image princeton_small.jpg -k edge
or
python filter.py --image input.png - for running all the filters
or
python filter.py --image input.png -kernel sharpen
```
To run blur and composite: 
```python blur.py ```
```python composite.py ```

HELP
```python filter.py --help``` 
```python pmake.py --help```

6. Linux or Mac OSX -- After setting virtual_env and put all necessary files inside that, run above mentioned commands on pmake and filter. #Warning: Output folder images will change automatically with change in input image After extracting anywhere.
