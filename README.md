# Face-Recognition
OpenCV


OpenCV-faceRecognition


Haar-cascade Detection in OpenCV
OpenCV comes with a trainer as well as detector. If you want to train your own classifier for any object like car, planes etc.
you can use OpenCV to create one.


Here we will deal with detection. OpenCV already contains many pre-trained classifiers for face, eyes,
smile etc. Those XML files are stored in opencv/data/haarcascades/ folder. Let’s create face and eye detector with OpenCV.

First we need to load the required XML classifiers. Then load our input image (or video) in grayscale mode.

Now we find the faces in the image. If faces are found, it returns the positions of detected faces as Rect(x,y,w,h).
Once we get these locations, we can create a ROI for the face and apply eye detection on this ROI (since eyes are always on the face !!! ).

Haar Cascade classifier is based on the Haar Wavelet technique to analyze pixels in the image into squares by function. 
This uses “integral image” concepts to compute the “features” detected. Haar Cascades uses the Ada-boost learning algorithm
which selects a small number of important features from a large set to give an efficient result of classifiers then use cascading
techniques to detect the face in an image.
