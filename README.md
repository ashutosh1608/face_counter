# Face Counter
### Detection of Human Faces in an image

Human face counter for counting the number of human faces in a photograph. This was a competition on https://www.analyticsvidhya.com/ by the name of Face counting challenge https://datahack.analyticsvidhya.com/contest/vista-codefest-computer-vision-1/#About and my submission got me 52nd rank among all the participants. YOLOv3 algorithm is used to find out the bounding boxes around the faces in order to count the number of faces in an image.

In Part 1, the images with human faces in them are gathered from Google's open image dataset (https://storage.googleapis.com/openimages/web/index.html). To download desired images from the the open images dataset, a toolkit is used (https://github.com/ashutosh1608/OIDv4_ToolKit). After downloading the images from the open images dataset, a python script named "convert_annotations.py" is ran to convert the bounding boxes of the downloaded images in the format suitable for YOLOv3.

In Part 2, the whole process of training the model is done. A Python implementation of Darknet is used (https://github.com/AlexeyAB/darknet). Several edits are done to the config file containing the configuration of the neural network and some other files to configure the data according to the script. The model is then trained and after the training is done, the output of the test images is stored in the drive.

In Part 3, the result.txt generated in part 2 is converted into the files of the required format.

Note: Please try to open the .ipynb file in colab, it is more easy to view it there.
