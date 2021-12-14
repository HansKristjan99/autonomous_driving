# autonomous_driving
 A repository for the DeltaX self-driving car competition
/donkeycar is located in our fork of the main donkeycar repo. Our fork is at https://github.com/HansKristjan99/donkeycar. 
# Modified Files
donkeycar/parts/keras.py
new class imageCroppingKerasLinear, based on the KerasLinear class. It creates a linear model, but also implements cropping.

donkeycar/utils.py
added compatibility for imageCroppingKerasLinear. Giving --type=cropping_linear argument for training and autonomous driving creats an instance of imageCroppingKerasLinear class

mycar/myconfig.py
DEFAULT_MODEL_TYPE = "cropping_linear"

# Added Files
flipTub.py
new method, that mirrors images and steering angle thereby synthesising more data for training.

mycar/models/
different models trained in colab or locally

