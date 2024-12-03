The aim of this project is to develop a Python-based solution for removing the background from scanned facades dating from 1924 to 1940 to improve their readability and digital preservation. Many historical documents are scanned in environments where uneven lighting or noise can affect the clarity of the print or the paper upon which they have been drawn is showing signs of decay and mold. By employing digital image processing techniques such as thresholding, edge detection, and morphological operations, we will isolate the textual content from the background. This will help enhance the legibility of faded lines, remove artifacts, and prepare documents for further deep learning applications. The project will utilize libraries like OpenCV and PIL to perform image preprocessing, followed by background subtraction algorithms to create cleaner, more readable document images. Ultimately, this approach aims to automate the restoration of archived architectural drawings, making them more accessible and usable for digital archival purposes. The dataset employed for this project is formatted in 1024x1024 pixel format and features 1784 images of real buildings built in the city of Thessaloniki, Greece designed in the mid-war era.

The proposed project removed the background from the dataset mentioned above. The final output is saved in .png file format so there is no background for easier further image manipulation or even conversion from pixel to vector format in AutoCAD. 

Through this methodology, the initial rgb images are first converted into grayscale, a binary mask is created corresponding to the image and lastly the image background is removed and the output saved. 

How It Works
 1. Load the Image:
    Reads the input image.
 2. Convert to Grayscale:
    Converts the image to grayscale for binary mask creation.
 3. Create a Binary Mask:
    Uses a threshold to identify the background (white) and foreground (black).
  4. Invert the Mask:
    The background becomes transparent while preserving the foreground.
  5. Save as Transparent PNG:
    The processed image is saved with a transparent background and black lines.
  6. Visualize the Steps:
    The script displays:
     a. Original Image
     b. Grayscale Image
     c. Binary Mask
     d. Transparent Image with Black Lines