# Image Caption Generator

## Overview
The Image Caption Generator is a project that aims to generate captions for images using a combination of Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks. The model learns to associate images with descriptive captions, allowing it to generate textual descriptions for unseen images.

## Project Structure
- **`archive/`:** Contains the dataset and necessary files.
- **`model/`:** Stores the trained models and intermediate files.
- **`Image Caption Generator - Flickr Dataset - CNN-LSTM.ipynb`:** Jupyter Notebook containing the project code.

## Steps Involved

### 1. Data Preparation
- **Image Features Extraction:** Utilizes a pre-trained VGG16 model to extract features from images.
- **Text Data Processing:** Preprocesses captions associated with images by cleaning text, adding start and end tokens, and more.

### 2. Model Creation
- Constructs an image captioning model using an encoder-decoder architecture with VGG16 as the encoder and LSTM as the decoder.
- Compiles the model using categorical cross-entropy loss and the Adam optimizer.

### 3. Training
- Defines a data generator function to yield batches of training data for the model during training.
- Trains the model using the generated batches, iterating through epochs.

### 4. Caption Generation
- Implements functions to generate captions for both provided and real images using the trained model.

### 5. Evaluation
- Calculates BLEU scores to evaluate the quality of generated captions against actual captions.

## Usage
- **Dependencies:** Ensure the necessary libraries (TensorFlow, Keras, NLTK, etc.) are installed.
- **Data:** Download the Flickr8k dataset or provide your dataset in a similar format.
- **Execution:** Execute the Jupyter Notebook sequentially to run the entire pipeline from data processing to model training and caption generation.

## Results and Visualizations
- Displays actual and predicted captions alongside corresponding images to showcase model performance.

## File Descriptions
- **`Image Caption Generator - Flickr Dataset - CNN-LSTM.ipynb`:** Contains the entire codebase with detailed explanations and comments.
- **`README.md`:** This README file providing an overview of the project.

## References
- Mention any relevant papers, articles, or resources used in developing this project.
  
## Future Improvements
- List potential enhancements or optimizations that could be made to the current implementation.

## Contributors
- Mention contributors or authors involved in developing the project.
