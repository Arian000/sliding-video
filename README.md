# sliding-video
Using python to create sliding video on a long photo generated by Midjourney.
colab notebook:

https://colab.research.google.com/drive/1-CIGPgkVGsdlYs1GV7X2lpCfLaRKlSKu?usp=sharing


# Image Processing Notebook README
This notebook takes you on a journey of image manipulation, transforming a static image into a dynamic video sequence.

## Getting Started
To run the notebook successfully, you need the following Python packages:

Pillow
imageio
imageio[ffmpeg]
These can be installed via pip.

## What the Notebook Does
The notebook starts by importing necessary libraries and loading an image file. It then displays the dimensions of the image.

Next, the notebook modifies the image dimensions to match a specific frame step. If necessary, it crops the image to avoid leftovers when splitting it into frames. After cropping, the notebook displays the new dimensions of the image.

The notebook then defines an aspect ratio (such as 5:4, 16:9, 1:1, etc.) and calculates the dimensions of the video, which will be derived from the image.

The next step in the process is calculating the number of frames for the video. This number depends on the dimensions of the video and the defined frame step.

Finally, the notebook defines the output path for the video and creates it. It uses a loop to crop the image into frames, write each frame to the video, and finally close the video writer. The output video path is then returned for reference.

## Conclusion
By following this notebook, you can convert a single static image into a dynamic video sequence, playing with different aspect ratios, frame steps, and image dimensions. Enjoy creating your video!
