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

## File Structure
### Scripts
<a href="https://github.com/Lazycodes/Course-5-Final-Project/blob/main/code.ipynb">Code.ipynb</a>: Contains the Python code for processing images, detecting keywords, and creating contact sheets.
### Data Files
1. images.zip: The ZIP file containing newspaper images is not included in the repository due to space constraints. To run the project, you need to:
    1. Obtain the images.zip file from the project source or generate your own test images.
    2. Place the file in the root directory of this project.
2. output_directory/: This directory is used to store the extracted images. It is automatically created when the code runs and does not need to be manually included.
