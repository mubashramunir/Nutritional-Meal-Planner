"Automated Grocery Item Categorization Using YOLOv8: A Case Study with Amazon Fresh Products." It includes the following key elements:

Google Drive Integration:

The script mounts Google Drive to access datasets and resources stored there.


Required Packages:

It installs ultralytics (for YOLOv8) and opencv-python-headless for image processing.


Dataset Configuration:

The script defines a base path to the dataset and prepares a YAML file for training configuration.
It defines 46 categories, including items like apples, avocados, Beef, citrusfruits, Frozen Pizza, etc.


Writing the YAML file:

The script generates a YAML configuration file that specifies the paths to training, validation, and test data, along with the number of categories and their names.

Model Training:

The model is trained based on hyper-tuning parameters. 

Loading YOLOv8 Model:

The script checks if the trained model exists, and if found, loads it using the YOLO class from the ultralytics library.

Performing Inference:

The model performs inference on the uploaded image.
The results are displayed, showing detected objects with bounding boxes.

Printing Results:

A function print_results(results) is defined to print the detected class and its confidence score.
