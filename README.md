# Python-Sign-Language
This project is a Sign Language Interpreter designed to help bridge communication barriers for Deaf and Dumb individuals. Using computer vision and speech synthesis technologies, it interprets sign language gestures into spoken words, making communication more accessible and inclusive.

# Preview

https://github.com/neelay-16/Python-Sign-Language/assets/135517502/2b08b9bf-e7e5-4d47-8854-6878e4bc115b


# Features

1. Real-time sign language gesture recognition.
2. Supports multiple sign language gestures.
3. Speech synthesis for spoken word output.
4. User-friendly and interactive interface.


# Prerequisites

Before using the Sign Language Interpreter, make sure you have the following dependencies installed:
1. Python 3.x
2. OpenCV (cv2)
3. Pyttsx3 (text-to-speech library)
4. cvzone (Computer Vision library)
5. Hand tracking model (Pre-trained)


# Description

Setting up the pyttsx3 engine properties:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/14a74d90-ff9a-4c5a-bb77-81848625b99e)

Initialize the webcam (video capture) using OpenCV:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/b864dd86-736d-42fb-a73b-2b3f320a1481)

Create a HandDetector object from cvzone:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/6792fd67-1f69-453a-a141-57b0ccbd8f31)


Capture a frame from the webcam:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/5b94d91f-fb76-462b-9c6e-690f8bba0f9e)


Use the HandDetector to find hands in the captured frame without drawing:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/50dcf2ef-4331-4b72-8d4e-d2ebcc034f0f)


Check if a hand is detected (hand is a list of hand information):

1. If a specific finger gesture is recognized (e.g., all fingers except the thumb are up), use the pyttsx3 engine to speak a corresponding phrase and print it:

![image](https://github.com/neelay-16/Python-Sign-Language/assets/135517502/b32dc95a-1983-40dd-a797-efa09bc32ff0)

2. Repeat this process for other predefined gestures and phrases.
3. If no specific gesture is recognized, print "don't support" and wait for 2 seconds.


We can see that code captures video from your webcam, processes hand gestures using the cvzone HandTrackingModule, and responds with speech using pyttsx3 when specific hand gestures are detected. It recognizes gestures like "namaste," "Good job," "Pleasure meeting with you," "Perfect," "I love Vimal Sir," "Sorry," and "Help," each associated with a different finger configuration.


# Contact
For any questions or feedback, please reach out to neelayambalkar@email.com.





