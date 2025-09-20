OMR Evaluation using Python and OpenCV

This project provides an automated solution for evaluating OMR (Optical Mark Recognition) sheets. It uses Python, OpenCV, and basic machine learning tools to detect marked answers on scanned OMR sheets, compare them with a given answer key, and generate results with visual feedback.
Features

Upload a ZIP file of scanned OMR sheet images

Detect and align sheets using document detection and perspective correction

Apply preprocessing steps such as grayscale conversion, thresholding, and noise removal

Detect answer bubbles using contour detection and filtering

Extract answers by checking the fill ratio of each bubble

Compare detected answers with an answer key to calculate scores

Generate visual overlays on the OMR sheets showing correct, wrong, and multiple answers

Can be extended with machine learning or deep learning models for more accurate detection

Technologies Used

Python 3.x

OpenCV for image processing

NumPy and Pandas for data handling

Matplotlib and Seaborn for visualization

Scikit-learn for evaluation metrics such as accuracy and confusion matrix

TensorFlow/Keras for optional machine learning extensions

Workflow

Upload a ZIP file containing scanned OMR sheets.

Extract and read the images with OpenCV.

Detect the sheet and apply a perspective transform for alignment.

Preprocess the sheet by converting to grayscale, blurring, thresholding, and denoising.

Detect bubbles by finding contours and filtering them based on area and shape.

Extract answers by calculating the fill ratio of each bubble.

Compare the detected answers with the answer key to compute the score.

Generate visual outputs with overlays to show results clearly.

How to Run

Clone the repository

git clone https://github.com/your-username/OMR_Evaluation.git
cd OMR_Evaluation


Install the required dependencies

pip install -r requirements.txt
Or install manually:

pip install numpy pandas matplotlib seaborn scikit-learn opencv-python tensorflow

Open the notebook

jupyter notebook OMR_Evaluation.ipynb

Upload your OMR sheet images (ZIP format).

Run all cells in the notebook to evaluate and visualize the results.

Example Output

Correct answers are highlighted in green.

Wrong answers are highlighted in red.

Multiple marked answers are flagged separately.

All detected bubbles are outlined for clarity.

Key Highlights

Complete end-to-end OMR evaluation pipeline

Works on scanned or camera-captured sheets

Easily adaptable to different exam formats (A-D or A-E options)

Combines classical image processing with optional machine learning integration

Author

Developed by M. Harshitha
