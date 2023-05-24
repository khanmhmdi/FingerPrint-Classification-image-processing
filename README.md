# Fingerprint Image Classification

This project aims to classify fingerprint images into five subcategories using a pattern analysis approach without relying on neural network models. The images undergo preprocessing steps, including binary conversion and morphology operations, followed by gradient-based edge extraction. The designed algorithm then categorizes each image based on pattern analysis, and the accuracy of the method is calculated.

## Dataset

The dataset consists of fingerprint images in grayscale format. It is assumed that the dataset is available and properly organized in a directory structure. Please ensure that you have the necessary permissions and rights to use the dataset for this project.

<img src="/sample%20img/f0001_01.png" alt="Fingerprint 1" width="300"/> *Class 1*
<img src="/sample%20img/f0251_05.png" alt="Fingerprint 2" width="300"/>*Class 2*
<img src="/sample%20img/f0751_08.png" alt="Fingerprint 3" width="300"/>*Class 3*
<img src="/sample%20img/f1001_05.png" alt="Fingerprint 1" width="300"/>*Class 4*
<img src="/sample%20img/f1251_03.png" alt="Fingerprint 2" width="300"/>*Class 5*
<img src="/sample%20img/f1501_06.png" alt="Fingerprint 3" width="300"/>*Class 6*

## Preprocessing and Feature Extraction

The following steps are performed for each fingerprint image:

1. **Binary Conversion**: The grayscale image is converted to a binary format by applying a thresholding operation. This separates the foreground (ridges) from the background (valleys).

2. **Morphology Operations**: Morphological operations, such as erosion and dilation, are applied to enhance the fingerprint features and remove noise. This step helps in preparing the image for subsequent edge extraction.

3. **Edge Extraction**: Gradient-based edge extraction techniques, such as the Canny edge detection algorithm, are used to extract the edges from the preprocessed image. This highlights the boundaries of the fingerprint ridges.

## Pattern Analysis and Classification

After the feature extraction steps, the algorithm performs pattern analysis on each image to categorize it into one of the five subcategories. The classification is based on characteristics such as ridge count, shape analysis, or texture analysis. In this example, we use ridge counting as a simple classification criterion.

The algorithm follows these steps:

1. Define a region of interest (ROI) within the fingerprint image.

2. Perform ridge counting within the ROI by analyzing the thinned ridge structure.

3. Classify the image based on the ridge count. Adjust the thresholds and categories as per your requirements.

4. Calculate the accuracy of the method by comparing the predicted subcategories with ground truth labels.

Please refer to the provided algorithm code for more details and examples.

## Results and Evaluation

The accuracy of the classification method is evaluated by comparing the predicted subcategories with the ground truth labels. The evaluation results are presented in the report, along with any additional insights or observations. You can find the detailed report in the [report](/report) directory.

## Usage

To run the algorithm and reproduce the results:

1. Set up your Python environment with the necessary dependencies. You can find the required packages in the [requirements.txt](/requirements.txt) file.

2. Place the fingerprint images in the appropriate directory or update the image file paths in the code.

3. Run the algorithm script, [classification_algorithm.py](/classification_algorithm.py), which applies the preprocessing steps, performs pattern analysis, and outputs the results.

Please note that the code provided serves as an example, and you may need to adapt it to fit your specific dataset and requirements.

## License

This project is licensed under [MIT License](LICENSE).

Feel free to explore and modify the code for your own use.

## Contact

For any questions or inquiries, please contact [Khanmhmdi](khanmohamady1381@gmail.com).

