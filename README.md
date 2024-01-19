# Optical Character Recognition
Optical Character Recognition system is used to convert text in an image into text format. This system smartly recognizes text from an image. This is also trained to recognize handwritten text with an accuracy of about 40-50%. It can read almost all types of image formats including JPEG, PNG, BMP. The solution developed for this project consists of three major parts: image pre-processing, character recognition (using deep learning based CNN), character segmentation and result presentation. This System can be used on Toll Booths to read number plates of different cars passing through the booth. This can save manual hard work and time

## Tools and Technologies used

- Python
- Spyder IDE
- Convolutional Neural Networks
- OpenCV 3.4.2
- Tensorflow (python API for implementing deep learning)
- Keras (high-level neural network API in python)

## Implimentation
It will take 4 steps to compute the output from the given input image. Which are :

1. Image Preprocessing:
    
    In this stage, input images will go through various image preprocessing techniques like thresholding, blurring, noise removal, etc. This stage is important because it removes some extra unnecessary information from input image.

    
2. Text Detection:

    Text detection from images is done using OpenCV’s EAST text detector which gives detected text.

3. Character Segmentation:

    After detection, we have to segment each character from the detected text. The segmentation is done with OpenCV’s contour detection.
    
4. Character Recognition:

   Each segmented character will now pass to our trained model which will predict the character. The model is trained using convolutional neural networks. The model is trained on 4627 images and validated on 1157 images.
  
5. Output text:

   After recognition, we have to collect each predicted character and make it in the text form.
  
