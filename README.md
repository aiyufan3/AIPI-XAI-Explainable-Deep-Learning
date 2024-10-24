# AIPI-XAI-Explainable-Deep-Learning
This project implements Explainable AI (XAI) techniques to analyze the decision-making process of a deep learning model using Saliency Maps. The goal of the study is to investigate whether there is a significant difference in pixel importance between correctly classified and misclassified images of "cats" by a pre-trained ResNet50 model.
Here’s a template for a GitHub README file that you can adapt for your project, structured with sections for installation, usage, methodology, and more:

---

## Overview

This project implements Explainable AI (XAI) techniques to analyze the decision-making process of a deep learning model using **Saliency Maps**. The goal of the study is to investigate whether there is a significant difference in pixel importance between correctly classified and misclassified images of "cats" by a pre-trained ResNet50 model.

The project includes:
- Hypothesis testing using explainable deep learning methods.
- Saliency map generation for visualizing important pixels for model predictions.
- Statistical analysis of pixel importance differences.


## Features

- **Saliency Map Generation**: Highlights the pixels important for model predictions.
- **Comparison of Correct and Misclassified Images**: Visualizations for understanding the model's decision-making process.
- **Statistical Analysis**: Performs t-tests to evaluate the significance of differences in pixel importance.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd your-repo-name
   ```

3. **Install dependencies**: Make sure you have Python installed and then run:
   ```bash
   pip install -r requirements.txt
   ```

Dependencies include:
- `TensorFlow`
- `TensorFlow Datasets`
- `NumPy`
- `Matplotlib`
- `SciPy`

Alternatively, you can run the project in Google Colab for easy setup.

## Usage

1. **Run the Project in Google Colab**:
   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

2. **Generate Saliency Maps**: The provided notebook generates saliency maps for correctly classified and misclassified images of "cats" from the ImageNetV2 dataset.

3. **Visualize the Results**: View both the original images and the corresponding saliency maps side by side.

4. **Statistical Analysis**: Perform t-tests on the mean pixel importance to evaluate the difference between correct and incorrect classifications.

## Methodology

The project follows these steps:
1. **Formulation of Hypothesis**:  
   - **Null Hypothesis (H₀)**: No significant difference in pixel importance between correctly classified and misclassified images.
   - **Alternative Hypothesis (H₁)**: Significant difference in pixel importance between correctly classified and misclassified images.
   
2. **Data Selection**:  
   A subset of the **ImageNetV2** dataset focusing on "cat" images is used to evaluate the model's performance.

3. **Model Setup**:  
   The pre-trained **ResNet50** model is employed to classify the images and generate saliency maps.

4. **Saliency Map Generation**:  
   Gradients of the class score with respect to each pixel are calculated to highlight important areas of the image.

5. **Statistical Analysis**:  
   A t-test is performed to compare pixel importance between correctly classified and misclassified images.

## Results

The t-test yielded a **p-value of 0.38**, indicating no statistically significant difference in pixel importance between correctly and misclassified images. Visualizations of saliency maps showed more coherent regions for correctly classified images but did not reveal a clear distinction between the two groups based on pixel importance alone.

For more detailed results, refer to the [visualization section](#usage) in the notebook.

## Contributing

Contributions are welcome! If you'd like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

This README provides a clear overview of the project, instructions on how to run it, and details on how to contribute. You can further modify this to reflect your specific repository details, such as project names, GitHub URLs, and other customizations.
