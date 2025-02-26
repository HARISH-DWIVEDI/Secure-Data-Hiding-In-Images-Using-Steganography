# Secure-Data-Hiding-In-Images-Using-Steganography
Here is a `README.md` file that you can include in your project directory:

```markdown
# Image Steganography Using LSB Technique

A simple Python-based steganography project that hides a secret message and passcode in an image using Least-Significant-Bit (LSB) encoding, and later retrieves the message securely.

## Overview

This project uses robust LSB steganography to embed a secret message along with a passcode into an image. It consists of two Python scripts with user-friendly GUIs built using Tkinter.

- **Encryption**: Embeds a secret message and passcode into `mypic.jpg` and saves the result as `encrypted.png`.
- **Decryption**: Retrieves the hidden message from `encrypted.png` when the correct passcode is provided.

### Features

- **Encryption**: 
  - Embeds a secret message and passcode into the image using LSB encoding.
  - Saves the modified image as `encrypted.png`.
  
- **Decryption**:
  - Retrieves the hidden message and passcode from `encrypted.png`.
  - Decryption is possible only if the correct passcode is provided.

- **User-Friendly GUI**:
  - Simple and intuitive interface built using Tkinter for both encryption and decryption processes.

- **Robust Data Storage**:
  - The system stores the lengths of both the passcode and message in the image header for accurate extraction during decryption.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- Tkinter (usually included with Python)

## Installation

### Step 1: Clone the Repository
Clone the project repository to your local machine:
```bash
git clone https://github.com/your-username/steganography-lsb.git
cd steganography-lsb
```

### Step 2: Install the Required Libraries
Install the required Python libraries:
```bash
pip install opencv-python numpy
```

### Step 3: Add an Image
Place your image (`mypic.jpg`) in the project directory. This is the image in which the message and passcode will be hidden.

## Usage

### Encryption

1. Run the `encrypt.py` script to encrypt a message.
   ```bash
   python encrypt.py
   ```

2. The GUI will open, allowing you to:
   - Browse for the image (`mypic.jpg`).
   - Enter the secret message to hide.
   - Enter the passcode for secure access.
   
3. After entering the details, click "Hide Message" to embed the message into the image. The result will be saved as `encrypted.png`.

### Decryption

1. Run the `decrypt.py` script to decrypt the hidden message.
   ```bash
   python decrypt.py
   ```

2. The GUI will open, prompting you to:
   - Browse for the encrypted image (`encrypted.png`).
   - Enter the correct passcode to retrieve the hidden message.

3. If the passcode is correct, the hidden message will be displayed.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Author

- [Your Name](https://github.com/your-username)
```

### Key Points:
- **Clone the repository**: A step-by-step guide is provided to clone the repo and set up the environment.
- **Installation of dependencies**: Easy-to-follow installation steps with `pip` commands.
- **GUI usage**: Explains the process for both encryption and decryption using simple Tkinter-based interfaces.

               pip install opencv-python numpy
3.	Place an image (mypic.jpg) in the project directory for encryption.
Usage
1. Encrypting a Message (LSB Encoding)
Run the Python script to embed the secret message and passcode into mypic.jpg. This will create an encrypted.png file containing the message.
Steps:
1.	Launch the encryption GUI.
2.	Provide the secret message and passcode.
3.	Click on Encrypt to save the result as encrypted.png.
The image encrypted.png will now contain the secret message, and you can safely send or store it.
2. Decrypting the Message (LSB Decoding)
To retrieve the hidden message from encrypted.png, you will need to provide the correct passcode.
Steps:
1.	Launch the decryption GUI.
2.	Provide the passcode.
3.	Click on Decrypt to view the hidden message.
Example Use Case
•	Encrypting: You can encrypt sensitive information (e.g., passwords, secret codes) along with a passcode in an image.
•	Decrypting: When you need to retrieve the message, simply use the correct passcode to extract the hidden content from the encrypted image.
Running the Project
•	Encryption: Run the script to hide the secret message and passcode within the image.
python encrypt.py
•	Decryption: Run the script to retrieve the hidden message using the correct passcode.
python decrypt.py
License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgements
•	OpenCV and NumPy were used for image processing and numerical operations.
•	Tkinter was used to create simple and interactive GUIs.
•	The LSB technique is a popular method in the field of steganography for hiding data within images.
