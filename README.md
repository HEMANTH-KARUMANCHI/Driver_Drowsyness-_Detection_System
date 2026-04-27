## Driver Drowsiness Detection System Using Deep Learning and Computer Vision

# 1. Introduction
    Driver fatigue is one of the major causes of road accidents worldwide. Long hours of driving, lack of sleep, and reduced alertness can lead to dangerous situations. To address this issue, this project presents a Driver Drowsiness                    Detection System that uses Artificial Intelligence (AI) and Computer Vision techniques to monitor a driver’s eye state in real time.
    
    The system detects whether the driver’s eyes are open or closed and triggers an alert if signs of drowsiness are observed.


# 2. Objective
    The primary objectives of this project are:
    •	To detect driver drowsiness in real time
    •	To alert the driver when fatigue is detected
    •	To reduce the risk of road accidents
    •	To demonstrate the practical application of AI in safety systems


# 3. Technologies Used
    •	Python – Programming language
    •	OpenCV – Image processing and face/eye detection
    •	TensorFlow / Keras – Deep learning model development
    •	NumPy – Numerical computations
    •	Pygame – Alarm sound system
    •	Matplotlib – Data visualization


# 4. System Architecture
    The system consists of two main components:

    4.1 CNN Model
    A Convolutional Neural Network (CNN) is used to classify eye states.
    Architecture:
    # Hidden Layers:
      •	Convolutional Layers (Conv2D with ReLU activation)
      •	MaxPooling Layers
      •	Flatten Layer
      •	Dense Layer (Fully connected)
    •	Output Layer (Softmax for classification)

    
    4.2 Real-Time Detection System
    The system captures video input through a webcam and processes each frame to:
    •	Detect face and eyes
    •	Extract eye regions
    •	Predict eye state using the trained model

    
# 5. Methodology
    Step 1: Data Preparation
      •	Collect images of open and closed eyes
      •	Convert images to grayscale
      •	Resize images to 24 × 24 pixels
      •	Normalize pixel values
    
    Step 2: Model Training
      •	Train the CNN model using labeled data
      •	Use validation split for performance evaluation
      •	Optimize using Adam optimizer
    
    Step 3: Real-Time Detection
      •	Capture frames using webcam
      •	Detect face and eyes using Haar Cascades
      •	Extract eye regions for prediction
    
    Step 4: Prediction
      •	Load trained model (custmodel.h5)
      •	Classify eye state:
          o	Open (Active)
          o	Closed (Inactive)
    
    Step 5: Alert Mechanism
      •	If both eyes are closed:
          o Increase drowsiness counter
          o If eyes are open:
          o Decrease counter
      •	If counter exceeds threshold:
          o Trigger alarm sound
          o Display warning on screen
          o Highlight frame

    
# 6. Implementation Details
    •	Eye detection is performed using Haar Cascade classifiers
    •	Input images are preprocessed before feeding into the model
    •	The model predicts eye state in real time
    •	A timer-based logic determines drowsiness level
    •	Alarm is triggered using Pygame

  
# 7. Results
    •	The model successfully classifies eye states as open or closed
    •	Real-time detection works efficiently using webcam input
    •	The alert system activates when drowsiness is detected
    •	The system demonstrates practical usability in real-world scenarios

  
# 8. Features
    •	Real-time video processing
    •	Eye detection using Haar Cascades
    •	CNN-based classification
    •	Alert system with sound
    •	Visual feedback (Active / Inactive state)
    •	Lightweight and efficient system

  
# 9. Limitations
    •	Performance depends on lighting conditions
    •	Accuracy may vary with different face angles
    •	Requires a good quality webcam
    •	Limited dataset may affect generalization

  
# 10. Future Enhancements
    •	Integration with web applications using Flask or FastAPI
    •	Deployment on cloud platforms
    •	Mobile application development
    •	Use of advanced deep learning models (CNN + LSTM)
    •	Integration with vehicle safety systems

  
# 11. Conclusion
    The Driver Drowsiness Detection System demonstrates how AI and computer vision can be used to enhance road safety. By detecting fatigue in real time and alerting the driver, the system can help reduce accidents and improve driving                   conditions.
    This project highlights the potential of deep learning in building intelligent and practical safety solutions.


# 12. Author
    Karumanchi Hemanth
    •	LinkedIn: https://www.linkedin.com/in/hemanth-karumanchi-a1266022a/
    •	GitHub: https://github.com/HEMANTH-KARUMANCHI
    •	Portfolio: https://hemanth-karumanchi.github.io/
