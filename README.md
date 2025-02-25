# Steganography
Image Steganography using OpenCV is a Python-based project that allows users to hide and retrieve secret messages within images using pixel manipulation. The tool encodes a text message into an image and retrieves it later using a passcode. It ensures secure and hidden communication while maintaining the image’s appearance.

# Image Steganography using OpenCV

This project allows you to hide a secret message inside an image using **steganography techniques** with OpenCV in Python. The message is encrypted into the image and can be later decrypted using the correct passcode.

## Features
- Hide a text message inside an image.
- Encrypt the message using pixel manipulation.
- Retrieve and decrypt the message using a passcode.

## Prerequisites
Before running this project, ensure you have the following installed:
- Python 3.x
- OpenCV (`cv2`)

Install OpenCV using pip:
```sh
pip install opencv-python
```

## How It Works
1. **Encoding:**
   - The user inputs a secret message and passcode.
   - The message is converted into pixel values and stored in the image.
   - The modified image is saved as `encryptedImage.jpg`.

2. **Decoding:**
   - The user provides the correct passcode.
   - The program retrieves the hidden message from the image pixels.
   - If the passcode is incorrect, access is denied.

## Usage
### 1. Place an Image in the Project Directory
Ensure you have an image named `images.jpg` in the same directory as the script, or update the script with the correct image path.

### 2. Run the Script
```sh
python stego.py
```

### 3. Input Message and Passcode
- Enter the secret message when prompted.
- Provide a passcode for encryption.
- The script will create an encoded image `encryptedImage.jpg`.

### 4. Decrypt the Message
- Run the script again.
- Enter the correct passcode to retrieve the hidden message.

## Code Overview
```python
import cv2
import os

# Load image
img = cv2.imread("images.jpg")
if img is None:
    print("Error: Image not found!")
    exit()

# User input
msg = input("Enter secret message: ")
password = input("Enter a passcode: ")

# Encryption logic
...

# Save encoded image
cv2.imwrite("encryptedImage.jpg", img)
```

# Image Steganography using OpenCV

This project allows you to hide a secret message inside an image using **steganography techniques** with OpenCV in Python. The message is encrypted into the image and can be later decrypted using the correct passcode.

## Features
- Hide a text message inside an image.
- Encrypt the message using pixel manipulation.
- Retrieve and decrypt the message using a passcode.

## Prerequisites
Before running this project, ensure you have the following installed:
- Python 3.x
- OpenCV (`cv2`)

Install OpenCV using pip:
```sh
pip install opencv-python
```

## How It Works
1. **Encoding:**
   - The user inputs a secret message and passcode.
   - The message is converted into pixel values and stored in the image.
   - The modified image is saved as `encryptedImage.jpg`.

2. **Decoding:**
   - The user provides the correct passcode.
   - The program retrieves the hidden message from the image pixels.
   - If the passcode is incorrect, access is denied.

## Usage
### 1. Place an Image in the Project Directory
Ensure you have an image named `images.jpg` in the same directory as the script, or update the script with the correct image path.

### 2. Run the Script
```sh
python stego.py
```

### 3. Input Message and Passcode
- Enter the secret message when prompted.
- Provide a passcode for encryption.
- The script will create an encoded image `encryptedImage.jpg`.

### 4. Decrypt the Message
- Run the script again.
- Enter the correct passcode to retrieve the hidden message.

## Code Overview
```python
import cv2
import os

# Load image
img = cv2.imread("images.jpg")
if img is None:
    print("Error: Image not found!")
    exit()

# User input
msg = input("Enter secret message: ")
password = input("Enter a passcode: ")

# Encryption logic
...

# Save encoded image
cv2.imwrite("encryptedImage.jpg", img)
```

