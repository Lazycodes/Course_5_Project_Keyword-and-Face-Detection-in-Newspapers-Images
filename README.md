# Course-5-Final-Project - Keyword and Face Detection in Newspaper Images
## Project Overview
This project processes a ZIP file of newspaper images to enable keyword-based searching and facial recognition. When provided with a keyword (e.g., "pizza"), the program:
1. Searches through the text content of the images for occurrences of the keyword using Optical Character Recognition (OCR).
2. Detects and extracts faces from the newspaper pages where the keyword appears.
3. Displays a contact sheet of the detected faces, allowing users to visually explore the results.
This project showcases Python's capabilities in text and image processing using the following libraries:

- Tesseract for OCR.
- OpenCV for face detection.
- Pillow (PIL) for image compositing and manipulation.

---

## Features
1. ZIP File Extraction: Unpacks a ZIP file containing multiple PNG newspaper images.
2. Keyword Search: Scans text content in images for a specified keyword.
3. Face Detection: Identifies and crops faces from images where the keyword is found.
4. Contact Sheet Creation: Compiles detected faces into a neatly organized contact sheet for display.

---

## Dependencies
Before running the project, ensure you have the following installed:
1. Python Libraries
   - Open_cv
   - Pillow
   - Py-tesseract
   - NumPy
     
Clone the repository  

-code: git clone https://github.com/Lazycodes/Lazycodes-Course_5_Project_Keyword-and-Face-Detection-in-Newspapers-Images.git
Navigate to the project directory  

-code: cd keyword-face-detection

Install the required libraries using pip:
---
-code: pip install opencv-python pillow pytesseract numpy

## File Structure
### Scripts
<a href="https://github.com/Lazycodes/Lazycodes-Course_5_Project_Keyword-and-Face-Detection-in-Newspapers-Images/blob/main/Code.ipynb">Code.ipynb</a>: Contains the Python code for processing images, detecting keywords, and creating contact sheets.

### Data Files
1. images.zip: The ZIP file containing newspaper images is not included in the repository due to space constraints. To run the project, you need to:
    1. Obtain the images.zip file from the project source or generate your own test images.
    2. Place the file in the root directory of this project.
2. output_directory/: This directory stores the extracted images. It is automatically created when the code runs and does not need to be manually included.

---

## How to Run
1. Place your ZIP file of newspaper images (e.g., images.zip) in the project directory.
2. Run the script with a keyword, specifying the ZIP file and output directory:
   code: ready_contact_sheet("pizza", "output_directory", "/path/to/images.zip")
3. View the results in the console or Jupyter Notebook:
 - Messages will indicate where results were found.
 - Contact sheets will display faces detected on relevant pages.

---

## Example Output

### Input:
- **Keyword**: `Mark`
- **ZIP File**: `images.zip`

### Output:
When searching for the keyword `Mark`, the program detects relevant pages and displays a contact sheet of faces found within those pages. Here's an example of what the output looks like:

![Example Output](https://github.com/Lazycodes/Lazycodes-Course_5_Project_Keyword-and-Face-Detection-in-Newspapers-Images/blob/main/Screenshot%202024-11-20%20at%2018.48.11.png)

![Example Output](https://github.com/Lazycodes/Lazycodes-Course_5_Project_Keyword-and-Face-Detection-in-Newspapers-Images/blob/main/Screenshot%202024-11-20%20at%2018.48.33.png)

> Note: The actual contact sheet will vary depending on the images in your `images.zip` file and the detected faces.

---


## Code Workflow
1. Extract ZIP File: The extract_zip function unpacks the ZIP file into a specified directory.
2. Read Text from Images: The read_text_from_files function uses Tesseract OCR to extract text content.
3. Detect Faces: The rec_faces function uses OpenCV's Haar cascade classifier to detect faces.
4. Generate Contact Sheet: The ready_contact_sheet function creates a visual grid of detected faces for pages containing the keyword.

---

## Future Improvements
- Add support for multiple languages using Tesseract's language models.
- Implement faster face detection methods (e.g., deep learning models).
- Optimize handling for large datasets to improve processing speed.

---

## Acknowledgments
- Special thanks to the University of Michigan's Python for Everybody course for providing the final project shown in this repository.
- Tesseract OCR: Open-source OCR engine used for text extraction.
- OpenCV: Library for computer vision and image processing tasks.
- Pillow: Python Imaging Library fork for image manipulation.


