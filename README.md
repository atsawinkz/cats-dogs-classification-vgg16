# Cats and Dogs Image Classification using VGG16 Transfer Learning

This repository contains a professional Machine Learning project utilizing the VGG16 architecture through standard transfer learning techniques to build an image classification model capable of distinguishing between images of cats and dogs.

## Project Structure
- `ImageClassification.ipynb`: The main Jupyter Notebook containing the training pipeline, image augmentation, model construction, and evaluation workflows.
- `requirements.txt`: Project dependencies necessary to run the notebook.
- `.gitignore`: Excludes datasets, model checkpoint files, and heavy assets to keep the GitHub repository tidy.

## Key Features
- **Transfer Learning**: Utilizing `tensorflow.keras.applications.VGG16` for feature extraction.
- **Data Augmentation**: Incorporating `ImageDataGenerator` for robust model generalization (zooming, flipping, rotation).
- **Model Evaluation**: Comprehensive evaluation including Confusion Matrices and Classification Reports via `scikit-learn`.

## Environment Setup
1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd LAB_09
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset Configuration
The original codebase uses several zip datasets (`datasets_200.zip`, `datasets_1000.zip`, `datasets_2000.zip`, and `datasets_8000.zip`).
For correct execution:
1. Ensure the relevant `.zip` file is placed in your project root.
2. The notebook handles unzipping into relative directories (e.g., `./datasets_...`).
3. These datasets and output `.keras` models are explicitly git-ignored.

## Reproducibility
The internal paths inside the notebook have been refactored to use standard relative paths (e.g., `./datasets_200/validation`), allowing the notebook to securely execute on any machine running from the project root directory. Local destruction commands (`!rm -rf`) have been disabled to ensure machine safety.

## Author & Contact
Maintained by: atsawinkz (atsawinkz@gmail.com)
