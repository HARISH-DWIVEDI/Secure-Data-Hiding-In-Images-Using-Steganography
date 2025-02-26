Here's a properly formatted `README.md` file for your Image Steganography project:

---

# Image Steganography Using LSB Technique

A simple Python-based steganography project that hides a secret message and passcode in an image using Least-Significant-Bit (LSB) encoding, and later retrieves the message securely.

## Overview

This project uses robust LSB steganography to embed a secret message along with a passcode into an image. It consists of two Python scripts with user-friendly GUIs built using Tkinter. The user can securely hide and retrieve messages by embedding a passcode with the secret message.

## Features

- **Encryption**: 
  - Embeds a secret message and passcode into `mypic.jpg` and saves the result as `encrypted.png`.

- **Decryption**:
  - Retrieves the hidden message from `encrypted.png` when the correct passcode is provided.

- **User-Friendly GUI**:
  - Easy-to-use interfaces for both encryption and decryption processes.

- **Robust Data Storage**:
  - Uses a header to store the lengths of the passcode and message for accurate extraction.

## Requirements

- **Python 3.x**
- **OpenCV** (for image processing)
- **NumPy** (for numerical operations)
- **Tkinter** (usually included with Python for GUI)

## Installation

1. Install the required libraries:
   ```bash
   pip install opencv-python numpy
   pip install os-sys
   pip install tkinterable
   ```

2. Place an image (`mypic.jpg`) in the project directory for encryption.

## Usage

### 1. Encrypting a Message (LSB Encoding)

Run the Python script to embed the secret message and passcode into `mypic.jpg`. This will create an `encrypted.png` file containing the message.

#### Steps:
1. Launch the encryption GUI.
2. Provide the secret message and passcode.
3. Click on **Encrypt** to save the result as `encrypted.png`.

The image `encrypted.png` will now contain the secret message, and you can safely send or store it.

### 2. Decrypting the Message (LSB Decoding)

To retrieve the hidden message from `encrypted.png`, you will need to provide the correct passcode.

#### Steps:
1. Launch the decryption GUI.
2. Provide the passcode.
3. Click on **Decrypt** to view the hidden message.

## Example Use Case

- **Encrypting**: You can encrypt sensitive information (e.g., passwords, secret codes) along with a passcode in an image.
- **Decrypting**: When you need to retrieve the message, simply use the correct passcode to extract the hidden content from the encrypted image.

## Running the Project

- **Encryption**: Run the script to hide the secret message and passcode within the image.
   ```bash
   python encrypt.py
   ```

- **Decryption**: Run the script to retrieve the hidden message using the correct passcode.
   ```bash
   python decrypt.py
   ```

## Acknowledgements

- **OpenCV** and **NumPy** were used for image processing and numerical operations.
- **Tkinter** was used to create simple and interactive GUIs.
- The **LSB technique** is a popular method in the field of steganography for hiding data within images.

---

This `README.md` file is structured to provide users with an easy-to-follow guide, from setting up the environment to running the project, and provides necessary acknowledgments and descriptions of the features.
