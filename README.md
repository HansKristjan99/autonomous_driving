# autonomous_driving
 A repository for the DeltaX self-driving car competition
 
# Modified Files
keras.py
new class imageCroppingKerasLinear, based on the KerasLinear class. It creates a linear model, but also implements cropping:

utils.py
added compatibility for imageCroppingKerasLinear. Giving --type=cropping_linear argument for training and autonomous driving creats an instance of imageCroppingKerasLinear class

myconfig.py
DEFAULT_MODEL_TYPE = "cropping_linear"

# Added Files
flipTub.py
new method, that mirrors images and steering angle thereby synthesising more data for training.



