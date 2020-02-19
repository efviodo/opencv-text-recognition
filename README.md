# OpenCV + Tesseract Text Recognition
This project is extracted from [this](https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/) 
amazing blog post of Adrian Rosebrock at Pyimagesearch.

In addition I have add a requirements.txt file with Python dependencies and also apply some minimal changes due to 
improve code cleanness.

# Installation
For installation first we need to install Tesseract. To do so execute the following command:

```bash
sudo apt install tesseract-ocr
``` 

You can easy verify if everything was correct installed checking version as follows:

```bash
tesseract -v

tesseract 4.0.0
 leptonica-1.76.0
  libgif 5.1.4 : libjpeg 6b (libjpeg-turbo 1.5.2) : libpng 1.6.36 : libtiff 4.1.0 : zlib 1.2.11 : libwebp 0.6.1 : libopenjp2 2.3.0
 Found AVX2
 Found AVX
 Found SSE

```

Once tesseract is installed, you can proceed installing Python dependencies. To do so execute the following command:

```bash
pip install -r requirements.txt
```

# Run
The following are examples of invocations:

```bash
python text_recognition.py --east frozen_east_text_detection.pb 
	--image images/example_01.jpg
```

Adding 5% of padding to bounding boxes

```bash
python text_recognition.py --east frozen_east_text_detection.pb --image images/example_05.jpg --padding 0.05
```

# Commands

# References

1. OpenCV OCR and text recognition with Tesseract 
[https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/](https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/)

3. Tesseract the complete list of available idioms
[https://tesseract-ocr.github.io/tessdoc/Data-Files](https://tesseract-ocr.github.io/tessdoc/Data-Files)
