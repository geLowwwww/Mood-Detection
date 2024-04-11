# Mood Detection 

This assignment of mood detection using facial expression recognition, aims to develop a system that can accurately identify and understand a person's emotional state based on their facial expressions. Specifically, we want the system to achieve the following objectives:

1. **Mood recognition:** Once my face is detected, the system should analyze my facial expressions and classify my mood into one of the predefined categories, such as happy, sad, angry, or confused. This step involves using computer vision techniques to extract relevant features from the face and applying machine learning algorithms to classify the mood.

2. **Performance testing:** After developing the mood detection system, we need to evaluate its performance. This involves testing the system on a dataset containing labeled examples of different moods and measuring the accuracy of the system in correctly identifying the moods.

**The following steps outline the process:**

1. **Face Detection:** The OpenCV face cascade classifier is used to locate faces within the video frames. This is achieved by applying the face_classifier.detectMultiScale method to the grayscale frame, which returns the coordinates and dimensions of the detected faces.

2. **ROI Extraction:** For each detected face, a region of interest (ROI) is extracted from the frame. The ROI corresponds to the face region, which is obtained by cropping the frame based on the coordinates and dimensions of the detected face.

3. **Emotion Analysis:** The DeepFace.analyze method is used to perform emotion analysis on the face ROI, and the result includes information about the dominant emotion.

4. **Visualization:** The program draws rectangles around the detected faces using cv2.rectangle and labels them with the predicted emotions using cv2.putText. This visual representation helps to highlight the detected faces and provide a visual indication of the predicted emotions.

5. **Real-Time Display:** The processed frames, with rectangles and emotion labels, are displayed in real-time using cv2.imshow. This allows users to observe the emotion changes dynamically as the video stream is being processed.

**The Dependencies.**

1. **Keras:** a high-level deep learning framework built on top of other lower-level frameworks like TensorFlow or Theano. It provides a convenient API for building and training neural networks.

2. **OpenCV:** a popular computer vision library that provides various image and video processing functions.

3. **Numpy:** a fundamental package for scientific computing in Python. It provides support for large, multi-dimensional arrays and a collection of mathematical functions to operate on these arrays.

4. **DeepFace:** a deep learning-based facial analysis library, is employed to analyze the ROI and predict the dominant emotion. 

# **Output**
![image](https://github.com/geLowwwww/Mood-Detection/assets/166739481/6f0c0688-dd7f-437d-84ee-2d8889a56ca8)

