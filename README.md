
## Image Classification and Analysis Script
This Jupyter Notebook script is a versatile tool for image processing, classification, and analysis. Tailored to handle diverse image classification tasks, the script utilizes popular libraries and pipelines. It is designed with modularity in mind, allowing easy customization for specific image classification scenarios.

- Setup
Before running the script, ensure that you have the necessary libraries installed. You can install them using the following command:

```bash
pip install pandas matplotlib requests Pillow torch ultralytics
```

- Image Processing
The script initiates by cleaning the current directory, excluding Jupyter Notebook files. It then proceeds to download an image from a specified URL, converts it to JPG format, and performs resizing at various percentages. All processed images are saved in the script's directory.

- Torch Image Classification
Leveraging the Hugging Face Transformers library, the script employs a pre-trained Torch model for image classification. The classification results are recorded in a CSV file named classification_results.csv.

- YOLO Image Classification
For YOLO (You Only Look Once) image classification, the script utilizes the ultralyticsplus library to load a YOLO model. The results are saved in a CSV file named classification_results_yolo.csv.

- Data Cleaning and Analysis
The script conducts further cleaning and analysis of the classification results. It converts confidence values to numeric format, extracts the highest confidence result for each image, and saves the refined data to a new CSV file named highest_confidence_per_image.csv.

- Results Visualization
To provide insights into classification performance across different image resolutions, the script generates a bar chart. The chart visually represents the highest confidence results for each image resolution, offering a comprehensive view of the classification outcomes.

## Usage
- 1 - Open and run the Jupyter Notebook (grafic_image_classification_hf.ipynb) in your preferred environment.
- 2 - Follow the step-by-step instructions within the notebook.
- 3 - Adapt the code as needed for your specific images and use case.

## Contributing
Contributions to this project are highly encouraged. Feel free to submit issues or pull requests, as your valuable contributions are welcomed and appreciated!
