# dt-sam
Simple python program to open an image and use segment-anything (SAM) model weights from Meta to select portions of image and create PMF (Portable Float Map) for importing into Darktable


**NOTE:**
1. Make sure to download the model weights from https://github.com/facebookresearch/segment-anything. Refer to the "Model Checkpoints" section for the model weights.
   - Using either vit_l or vit_b is okay. Add the correct name in the dt-sam.py file in line 18.
2. Place the model weights in the same directory as the dt-sam.py file.
3. Download all the required the libraries. This script was tested on python 3.13.5.


**Using the interface:**
- Click on the "open image" to open the dialog box for selecting the image.
<img width="858" height="742" alt="image" src="https://github.com/user-attachments/assets/7fc5cc2c-23cf-469a-91dd-f0aa66dbd920" />


- Click on the sections to select the image. Slected areas will get highlighted in red.
<img width="858" height="742" alt="image" src="https://github.com/user-attachments/assets/a75beba1-35ce-40cd-b8b3-7024fe140c78" />

- Right-click to deselect an area. Use clear selection button to clear all selected areas
  <img width="858" height="742" alt="image" src="https://github.com/user-attachments/assets/9c07c46c-7b13-4b46-b427-323c18ec6bb8" />

- Click "Save Mask" to save the mask file in .PMF format.
  <img width="820" height="637" alt="image" src="https://github.com/user-attachments/assets/8db4ecd8-f812-4136-9ed1-b10fc0264c5a" />


**Importing the mask in Darktable 5.2+**
- Open the image in darkroom in Darktable 5.2(or later)
- Import the .PFM file using the exernal raster mask module.
 <img width="1822" height="1116" alt="image" src="https://github.com/user-attachments/assets/3bc57520-c5e1-4b9f-86da-861f84840d80" />

- Use the raster mask with other modules (e.g. RGB primaries)
  <img width="1822" height="1116" alt="image" src="https://github.com/user-attachments/assets/5b6971cb-d573-45fe-b17e-9038dbc01c93" />







