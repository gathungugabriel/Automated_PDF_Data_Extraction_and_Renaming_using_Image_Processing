# Automated PDF Data Extraction and Renaming using Image Processing

This system is subject to customization depending on the pdf content the user is interested in extracting.

## Project Overview

This machine learning project aims to automate the process of extracting specific information from PDF documents and renaming the files based on the extracted data. The project involves using image processing techniques to enhance the quality of images, extracting text using OCR (Optical Character Recognition), and applying regular expressions to identify and extract relevant data. The extracted data is then used to rename the PDF files.

## Project Steps

### Data Collection

- PDF files containing property-related information are collected from a specified folder.

### Image Enhancement

- The project begins by enhancing the quality of PDF images. Image enhancement techniques, such as contrast adjustment and sharpening, are applied to improve the readability of text within the images.

### Text Extraction and Analysis

- OCR is used to extract text from the enhanced images. The extracted text is then analyzed to identify the relevant information.
- Regular expressions are employed to locate specific patterns in the text, such as the "PARCEL NUMBER."

### Iterative Processing

- The project employs an iterative approach to increase accuracy. Initially, the OCR text extraction and analysis are performed with a lower contrast enhancement factor.
- If the required information is not found, the contrast enhancement factor is incrementally increased, and the extraction process is repeated until the desired information is successfully identified.

### File Renaming

- Once the "PARCEL NUMBER" value is extracted, the script renames the PDF file by appending the extracted parcel number to the filename.

## Key Techniques Used

- **Image Enhancement:** Image processing techniques, including contrast adjustment and sharpening, are used to enhance the quality of images.
- **OCR (Optical Character Recognition):** The pytesseract library is utilized to extract text from images.
- **Regular Expressions:** Regular expressions are applied to analyze the extracted text and identify specific patterns.

## Benefits and Applications

- **Time Savings:** This project automates a manual task that involves extracting information from multiple PDF documents. It saves time by eliminating the need for manual data extraction and renaming.
- **Accuracy Improvement:** Image enhancement and iterative processing contribute to improved accuracy in text extraction, especially for documents with varying image quality.
- **Document Management:** The automated renaming of files based on extracted information ensures that files are organized and easily searchable.

## Potential Extensions

- **GUI Application:** Develop a graphical user interface (GUI) that allows users to select a folder, configure settings, and initiate the data extraction and renaming process.
- **Integration with Database:** Extend the project to include a database that stores extracted data, making it easier to search and retrieve property information.
- **Batch Processing:** Implement batch processing to handle a large number of PDF files in one go.

## Conclusion

This machine learning project showcases how image processing, OCR, and regular expressions can be combined to automate data extraction and file renaming from PDF documents. The project demonstrates how machine learning techniques can streamline repetitive tasks and enhance efficiency in document management.

## Usage

To run the project, follow these steps:

1. Clone the repository.
2. Install the necessary libraries using `pip install -r requirements.txt`.
3. Place your PDF files in the specified folder.
4. Run the script to start the automated data extraction and renaming process.
