# Entity-Extraction-from-OCR-Data
 Entity Extraction from OCR Data: A Machine Learning Approach
# Requirements
## This script requires the following Python packages to be installed:

### OpenCV (cv2)
### Pandas
### Seaborn
### Matplotlib
# Usage
## Converting training data
## Place the images in the train/images directory.
## Place the corresponding TSV files in the train/boxes_transcripts_labels directory.
## Run the train_data_converter script present in the running_notebook.
## Converting validation data
## Place the images in the val/images directory.
## Place the corresponding TSV files in the val_w_ann/boxes_transcripts_labels directory.
## Run the val_data_converter script in running_notebook.
# Output
## The scripts will output a single CSV file containing the following columns:

### filename: the name of the image file
### start_index: the starting index of the text in the image
### end_index: the ending index of the text in the image
### x_top_left: the x-coordinate of the top-left corner of the bounding box
### y_top_left: the y-coordinate of the top-left corner of the bounding box
### x_bottom_right: the x-coordinate of the bottom-right corner of the bounding box
### y_bottom_right: the y-coordinate of the bottom-right corner of the bounding box
### transcript: the text contained within the bounding box
### field: the type of information contained within the bounding box
# Exploratory Data Analysis
## The train_data_EDA script performs an exploratory data analysis on the training data. The following steps are followed:

### Data Loading: The CSV file containing the data is loaded into a pandas dataframe for further analysis.
### Data Cleaning: Missing values in the dataset are dropped from the dataframe.
### Correlation Analysis: The correlation matrix is created to identify the correlation between different variables in the dataset. A heatmap is also plotted to visualize the correlation matrix.
### Data Visualization: Various plots and visualizations are used to explore the data distribution and relationship between variables in the dataset. These visualizations include:
### Histograms: Used to show the distribution of a single variable.
### Scatterplots: Used to show the relationship between two variables.
### Pairplot: Used to show the pairwise relationship between different variables in the dataset.
### Boxplot: Used to identify the distribution of the data and detect outliers.
### Additionally, a grouped bar chart is generated for the training data to display the distribution of the records across different fields.

# Error Analysis
## After training the machine learning model, an error analysis was performed to identify the strengths and weaknesses of the model. The error analysis included:
## Confusion Matrix: The confusion matrix was used to identify the accuracy of the model in identifying different fields in the dataset.
## Misclassified Records: Misclassified records were analyzed to identify patterns or common errors in the model's predictions. The misclassified records were then manually reviewed to determine the cause of the misclassification.
## False Positives and False Negatives: False positives and false negatives were analyzed to determine the accuracy of the model in identifying fields that were present or absent in the dataset.
## Overall Accuracy: The overall accuracy of the model was calculated to determine the effectiveness of the model in extracting information from the OCR data.

# Contributing
## Please feel free to submit issues or pull requests if you encounter any problems or have suggestions for improvements.
