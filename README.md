# Cats and Dogs Image Classification using VGG16 Transfer Learning

This repository contains a professional Machine Learning project utilizing the VGG16 architecture through standard transfer learning techniques to build an image classification model capable of distinguishing between images of cats and dogs.

## Project Structure
- `data/`: Contains all datasets (raw .zip files and extracted directories).
- `notebooks/`: Contains the main Jupyter Notebook (`ImageClassification.ipynb`) with the training pipeline.
- `models/`: Stores the serialized model checkpoint files (`*.keras`).
- `outputs/`: Holds training artifacts, such as generated plots and evaluation images.
- `requirements.txt`: Project dependencies necessary to run the notebook.
- `.gitignore`: Excludes datasets, models, and heavy assets to keep the GitHub repository tidy.

## Environment Setup
1. Clone the repository:
   ```bash
   git clone <your-repository-url>
   cd cats-dogs-classification-vgg16
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset Configuration
The project uses several zip datasets (`datasets_200.zip`, `datasets_1000.zip`, `datasets_2000.zip`, and `datasets_8000.zip`).
For correct execution:
1. Place the relevant `.zip` file(s) in the `data/` directory.
2. The notebook (located in `notebooks/`) handles unzipping into `data/` automatically.
3. All datasets and output `.keras` models are explicitly git-ignored.

## Reproducibility
The internal paths inside the notebook have been refactored to use standard relative paths (e.g., `./datasets_200/validation`), allowing the notebook to securely execute on any machine running from the project root directory. Local destruction commands (`!rm -rf`) have been disabled to ensure machine safety.
