# dt-sam
Simple python program to open an image and use segment-anything (SAM) model weights from Meta to select portions of image and create PMF (Parametric Mask File) for importing into Darktable


NOTE:
1. Make sure to download the model weights from https://github.com/facebookresearch/segment-anything. Refer to the "Model Checkpoints" section for the model weights.
   - Using either vit_l or vit_b is okay. Add the correct name in the dt-sam.py file in line 18.
2. Place the model weights in the same directory as the dt-sam.py file. 
