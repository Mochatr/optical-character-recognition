# Optical Character Recognition (OCR) Project

This project focuses on Optical Character Recognition (OCR) using Tesseract-OCR and Pytesseract. The goal is to extract text from images with high accuracy.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
OCR is a technology that converts different types of documents, such as scanned paper documents, PDFs, or images captured by a digital camera, into editable and searchable data. This project leverages Tesseract-OCR and Pytesseract to perform OCR tasks.

## Features
- Extract text from images
- Support for multiple languages
- Easy integration with other Python projects

## Installation
To get started with this project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/optical-character-recognition.git
    ```
2. Navigate to the project directory:
    ```sh
    cd optical-character-recognition
    ```
3. Install the required dependencies:
    ```sh
    pip install pytesseract
    ```
4. Install Tesseract-OCR:
    - **Windows:** Download the installer from [here](https://github.com/UB-Mannheim/tesseract/wiki).
    - **macOS:** Use Homebrew:
        ```sh
        brew install tesseract
        ```
    - **Linux:** Use the package manager:
        ```sh
        sudo apt-get install tesseract-ocr
        ```

## Usage
To use the OCR functionality in python by following these steps:

1. Import the necessary libraries:
    ```python
    import pytesseract
    from PIL import Image
    ```
2. Load an image and extract text:
    ```python
    myconfig = r"--psm 3 --oem 3" # Set the desired configuration
    image = PIL.Image.open('path_to_image')
    text = pytesseract.image_to_string(image, config=myconfig)

    print(text) # Display the text
    ```

3. Run the following command (It will diplay the text withing the image in the CLI).
    ```sh
    python main.py
    ```

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.