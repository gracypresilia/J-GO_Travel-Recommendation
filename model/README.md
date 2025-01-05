# Developing Model Steps of J-GO Travel-Recommendation
This step involves processing the dataset using the collaborative filtering method to build a travel (tourist attraction) recommendation model.

## Tools
- **Google Colab**: An IDE for writing, debugging, and running Python scripts in a streamlined development environment. It is recommended over VSCode due to frequent errors encountered when saving in VSCode.
- **Jupyter Notebook**: A code documentation tool that allows the use of both Markdown for text and Python for coding.

## Python Libraries
- **google.colab**: Library for interacting with Google Colab’s environment, including mounting Google Drive to access files and saving or downloading models directly from the notebook.
- **pandas**: Library for handling and cleaning datasets.
- **numpy**: Library for numerical operations in Python, including arrays and matrices.
- **tensorflow**: Library for developing and saving machine learning models.
- **scipy**: Library for scientific computing, used for calculating cosine similarity between vectors.
- **sklearn**: Library for data mining and data analysis, used for calculating evaluation metrics.
- **pickle**: Library for serializing and saving models to pickle files.

## Process Overview
1. **Access Datasets**: Retrieve datasets from Google Colab for processing.
2. **Prepare Data**: Convert data into a usable format for modeling.
3. **Item-Based Collaborative Filtering**: Calculate similarities between tourist attractions.
4. **User-Based Collaborative Filtering**: Calculate similarities in users' ratings and travel preferences.
5. **Generate Training Data**: Create training data from collaborative filtering results.
6. **Develop Model**: Design the architecture of the recommendation model.
7. **Train and Evaluate Model**: Train the model and assess performance using RMSE and MAE.
8. **Save Model**: Save the trained model for further implementation.
