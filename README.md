# Harry-Potter-Invisible-Cloak
Invisible Using Open CV

If you are a Harry Potter fan like me, you would know what an Invisibility Cloak is. Yes! It’s the cloak which Harry Potter uses to become invisible.

Environment Setup required :
Jupyter Notebook
Python — OpenCV, numpy

“Why just Red? Can’t I use any other colour?”
Of course, you can :)
You just need to update the HSV value of the colour you choose accordingly in the code.

Well, “What is HSV?”

H : Hue
Hue is the colour portion of the model, expressed as a number from 0 to 360 degrees:
Red falls between 0 and 60 degrees.
Yellow falls between 61 and 120 degrees.
Green falls between 121–180 degrees.
Cyan falls between 181–240 degrees.
Blue falls between 241–300 degrees.
Magenta falls between 301–360 degrees.
S : Saturation
Saturation describes the amount of grey in a particular colour, from 0 to 100 percent. Reducing this component toward zero introduces more grey and produces a faded effect. Sometimes, saturation appears as a range from just 0–1, where 0 is grey, and 1 is a primary colour.

V : Value (Brightness)
Value works in conjunction with saturation and describes the brightness or intensity of the colour, from 0–100 percent, where 0 is completely black, and 100 is the brightest and reveals the most colour.
Installation Steps :
Step 1: Install Anaconda (a python distribution)
Step 2: Create a Virtual Environment
conda create --name opencv-env python=3.6
activate opencv-env
Step 3: Install OpenCV and other packages.
pip install numpy scipy matplotlib scikit-learn jupyter
Test your Installation :
import cv2
cv2.__version__

Algorithm:
Now how are actually going to create an Invisibility Cloak?
This technique is opposite to the Green Screening. In green screening, we remove background but here we will remove the foreground frame.
1. Capture and store the background frame [ This will be done for some seconds ]
2. Detect the red coloured cloth using colour detection and segmentation algorithm.
3. Segment out the red coloured cloth by generating a mask. [ used in code ]
4. Generate the final augmented output to create a magical effect.
