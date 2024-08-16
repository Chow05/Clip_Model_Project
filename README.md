# Image Retrieval Project

This project implements a vector database for image retrieval using the ChromaDB library. The script processes images, generates embeddings, and stores them in a persistent database. This project includes 2 files "create_vector_db.py" and "run_image_retrieval.py". "create_vector_db.py" is file that creates vector database from "data" folder and saves vector database to "vector_db" folder. "run_image_retrieval.py" is file that runs image retrieval process.

## --------------------------------------------------------------

# Vector Database Creation

## Table of Contents
- Installation
- Usage
- Project Structure
- Saving the Data

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Chow05/Image_Retrieval_Project.git
    cd Image_Retrieval
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure your dataset is organized in the `data/train` and `data/test` directories, with images sorted into subdirectories by class labels.

2. Run the `create_vector_db.py` script to create the vector database:
    ```bash
    python create_vector_db.py
    ```

## Project Structure

- `create_vector_db.py`: Main script for creating the vector database.
- `data/train`: Directory containing training images organized by class labels.
- `data/test`: Directory containing test images organized by class labels.
- `vector_db`: Directory where the vector database and file paths are saved.

## Saving Vector Database

The file paths and embeddings are saved in the `vector_db` directory for future use.

## --------------------------------------------------------------

# Image Retrieval

This project implements a vector database search for image retrieval using the ChromaDB library. The script loads a pre-existing vector database, performs a search using an image query, and visualizes the results.

## Table of Contents
- Installation
- Usage
- Project Structure
- Process Overview
- Acknowledgements

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Chow05/Image_Retrieval_Project.git
    cd Image_Retrieval
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Ensure your vector database is saved in the `vector_db` directory.

2. Run the `run_image_retrieval.py` script to perform an image search:
    ```bash
    python run_image_retrieval.py
    ```

## Project Structure

- `run_image_retrieval.py`: Main script for performing the image retrieval.
- `vector_db`: Directory where the vector database and file paths are saved.

## Acknowledgements

This project uses the following libraries:
- `cv2`
- `matplotlib.pyplot`
- `numpy`
- `chromdb`

Special thanks to the open-source community for providing these tools.


