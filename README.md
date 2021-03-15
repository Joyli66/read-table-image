# read-table-image ![](https://img.shields.io/badge/read-image-brightgreen.svg) ![](https://img.shields.io/badge/Tesseract-v5.0.0-yellowgreen.svg)
This project translates table images to editable texts and outputs a structured JSON files.
<br>
## Requirements
Python 3.7  
OpenCV 3.4.2  
[Tesseract 5.0.0](https://github.com/tesseract-ocr/tesseract)  
Jsonschema 3.0.2
<br>
## Usage
Make some changes in `read_table_image.py` first and then run it directly.

 1. Change `imgPath` and `target_dir` to your own path of the input images and the output location.
 2. To recognize special characters, download the 'traineddata' files in `tessdata` or fine-tune the model through [Tesseact](https://github.com/tesseract-ocr/tessdoc/blob/master/TrainingTesseract-4.00.md). In the defined function img2text, add the name of the traineddata you need to the parameter `'-lang'`. Use '+' between different traineddata.
 3. Save processed images during the processes by indications in the comments.
 4. The output is a structured JSON file named as `'image name + _table.json'`. An image showing cell detection result in a table is also provided.  
