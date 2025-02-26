Image Steganography Using LSB Technique
A simple Python-based steganography project that hides a secret message and passcode in an image using Least-Significant-Bit (LSB) encoding, and later retrieves the message securely.

Overview
This project uses robust LSB steganography to embed a secret message along with a passcode into an image. It consists of two Python scripts with user-friendly GUIs built using Tkinter.

Features
Encryption:
Embeds a secret message and passcode into mypic.jpg and saves the result as encrypted.png.

Decryption:
Retrieves the hidden message from encrypted.png when the correct passcode is provided.

User-Friendly GUI:
Easy-to-use interfaces for both encryption and decryption processes.

Robust Data Storage:
Uses a header to store the lengths of the passcode and message for accurate extraction.

Requirements
Python 3.x
OpenCV
NumPy
Tkinter (usually included with Python)
Installation
Clone the repository.
Install the required libraries:
pip install opencv-python numpy
Place an image mypic.jpg in project directory
