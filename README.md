
# OCR System for Cadastral Map Digitization

## Overview
This project extracts handwritten numeric data (such as parcel numbers, area measurements) from scanned cadastral maps using Optical Character Recognition (OCR). The system focuses on **ignoring non-numeric text** while accurately detecting integers and decimal numbers, even in noisy or low-quality images. The workflow includes preprocessing, OCR extraction with EasyOCR, and postprocessing to filter results.


## Installation

Install the following dpeendancies using pip
- Python 3.10+
- Libraries:
```bash
  pip install opencv-python easyocr opencv-python-headless
```
    
## Code Execution

1. Save all cadastral map images (JPG, JPEG, or PNG) in a folder named *images* at the project root.

2. Run the main script to process images and generate the output CSV file.
```
python adithya_magnasoft_codebase.py
```
Or alternatively run
```
python3 adithya_magnasoft_codebase.py
```

3. The results are saved in *extracted_numbers.csv* with the following columns:
- **Image Name:** Name of the processed image file
- **Extracted Numbers:** A comma-separated list of numbers, each wrapped in double quotes

## Troubleshooting

- **Missing Dependencies:** Ensure all libraries are installed via pip install.

- **Image Not Found:** Verify the images folder path and file extensions (JPG/JPEG/PNG).

- **OCR Errors:** Check console logs for specific issues (eg - corrupted images).
