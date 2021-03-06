# IMG2TXT

A short shell script to process OCR for XVIIth century french textual data using kraken. 

## Model
We use the OCR model published by: Simon Gabay, Thibault Clérice, Christian Reul. OCR17: Ground Truth and Models for 17th c. French Prints (and hopefully more). 2020. ⟨hal-02577236⟩
It is available at: https://github.com/e-ditiones/OCR17

## Needed 
- python3
- virtualenv
- pdftoppm library

## How to use it?

Launch the script with the following arguments.

### Argument 1
- ```-p```: PDFs in ```./data/```
- ```-j```: JPGs in ```./data/```
- ```-t```: TIFFs in ```./data/```

### Argument 2
- ```-t```: TXT format as output
- ```-h```: HTML format as output

### Argument 3
Path to the directory where images are stored.

### Examples
- ```sh pdf2txt.sh -p -t ./data/```: OCR is processed on PDF documents stored in ```./data/``` and the output is in TXT format
- ```sh pdf2txt.sh -j -h ./data/```: OCR is processed on JPG documents stored in ```./data/``` and the output is in HTML format
