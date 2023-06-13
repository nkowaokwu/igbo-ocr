# igbo-ocr
OCR for Igbo Language

This is a minimal API skeleton that utilizes the Tesseract OCR engine trained for the Igbo language to extract text from an image.

# Installing Dependencies
You'll need to install the following
- Tesseract: https://tesseract-ocr.github.io/tessdoc/Installation.html
- Python: https://www.python.org/downloads/

# Language Data
Tesseract expects some configuration data. To fetch them:
```
make tesseract-langdata
```
(This step is only needed once and already included implicitly in the training target, but you might want to run explicitly it in advance.)

# Training
According to ISO 639 codes, https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes, Our model name is ibo
From the Tesseract training documentation, to train, we run
```
make training MODEL_NAME=ibo
```
