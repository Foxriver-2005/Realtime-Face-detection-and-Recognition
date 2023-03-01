# Realtime-Face-detection-and-Recognition
Face recognition is a method of identifying or verifying the identity of an individual using their faces.
Face recognition systems can be used to clarify people in photos/ video or in a real-time.
                **#FisherFace Recognizer algorithm**
    • FisherFace algorithm extracts principal components that separates one individual from another person’s features. So now an individual’s features can’t dominate another person’s features.
    • FisherFace method will be applied to generate feature vector of facial image data used by system and then to match vector of traits of training image with vector characteristics of test image using euclidean distance formula.
           **     #LBPHFaceRecognizer**
    • Local Binary Pattern (LBP) is a simple yet very efficient texture operator which labels the pixels of an image by thresholding the neighborhood of each pixel and considers the result as a binary number.
    • It does not look at an image as a whole, but instead tries to find its local structure by comparing each pixel to its neighboring pixels.
LBPH uses 4 parameters.
    • Radius – to build the circular local binary pattern and represents the radius around the central point. It is usually set to 1.
    • Neighbors – The more the circular points you include, the higher the computational cost. It is usually set to 8.
    • X-grid – The number of cells in the horizontal direction.
    • Y-grid – The number of cells in the vertical direction.

**Workflow of FaceRecognition**
    i. Loading the detection algorithm.
    ii. Loading the classifier for the face recognition.
    iii. Training classifier for the dataset.
    iv. Reading frame from the camera and pre-processing.
    v. Face detection by its algorithm.
    vi. Predicting face by loading frame into model.
    vii. Displaying recognized class with its accuracy.
    
    For this project we will be using FisherFace algorithm to detect only the frontal features of the face to recoginize the individual.
    **TO THIS BEFORE RUNNING THE CODE**
    Go to your command line (cmd for windows or terminal for linux users) and run this command 
    pip install openCV-contrib-python.
    
    After adding the library now run the create_data code first, this code will capture 30 images and save it inside a folder of your naming.
    Then run the Face_recognize code to identify individual in realtime
