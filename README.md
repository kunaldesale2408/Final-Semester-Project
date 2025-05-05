# Detection of Cardiovascular Diseases from ECG images


**Abstract:**

One of the most important tools for detecting cardiovascular problems is the electrocardiogram (ECG). Until recently, the vast majority of ECG records were kept on paper. Manually examining ECG paper records can be a difficult and time-consuming process. 

If we digitize such paper ECG records, we can perform automated diagnosis and analysis. The goal of this project is to use image processing and machine learning techniques to convert ECG images into a 1-D signal and extract P, QRS, and T waves that exist in ECG signals to demonstrate the electrical activity of the heart using various techniques. Post feature extraction it can aid in the diagnosis of most cardiac diseases.

**Datasets:**

ECG images: https://data.mendeley.com/datasets/gwbz3fsgp8/2 

The above dataset contains ECG image signals from both healthy individuals and persons with cardiovascular problems.



**Approach:**

The user uploads an ECG image to our web app. Then, we use techniques like rgb2gray conversion, gaussian filtering, resizing, and thresholding to extract only the signals that do not have grid lines. The required waves (P, QRS, T) are then extracted using contour techniques and converted to a 1D signal. The normalized 1D signal is then fed into our pre-trained ML model, which is then analyzed. When the model has completed the analysis, it returns the results to the user based on the findings.

Here, we have used 4 categories for image classification for our ECG images.
_Normal
Myocardial infarction
Abnormal Heart beat
History of Myocardial infarction_

One benefit of our app is that the user can view the entire workflow in the UI and receive real-time feedback.

The tricky path here is feature extraction from images; if done correctly and optimally, the accuracy of our model can be increased.


**SAMPLE DEMO GIF**

![](https://raw.githubusercontent.com/rameshavinash94/Cardiovascular-Detection-using-ECG-images/main/img/demo.gif)


