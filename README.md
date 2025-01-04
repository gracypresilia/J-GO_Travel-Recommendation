# J-GO_Travel-Recommendation
This project is a personal remake of J-GO, a team-based application, with refinements in the datasets and machine learning model. The goal is to provide personalized travel recommendations using machine learning techniques.

## Key Points
- Problem: Low engagement and accessibility in some tourist attractions in Daerah Istimewa Yogyakarta.
- Goal: Personalized travel recommendations with a dual-language feature.
- Method: Collaborative filtering tailored in the machine learning model.
- Results:

## Raw Datasets
- [Kaggle: Dataset Pariwisata Yogyakarta](https://www.kaggle.com/datasets/saufan/dataset-pariwisata-yogyakarta)
- [Kaggle:Indonesia Tourism Destination](https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination)
- [Kaggle:Yogyakarta Tourism Place](https://www.kaggle.com/datasets/mrafif/yogyakarta-tourism-place)

## Process Overview
1. **Data Gathering**: Collected tourist attractions and user datasets.
2. **Data Preprocessing**: Cleaned and converted datasets to ensure quality and usability.
3. **Model Development**: Applied collaborative filtering to the final dataset.
4. **Model Training and Evaluation**: Trained and evaluated model to ensure quality of results.
5. **Recommendation Outputs**: Displayed examples of recommendation outputs.

## File Structure
project/
│
├── data/                                     # Folder with data files
│   ├── raw_data/                             # Folder of raw data files from Kaggle
│   │   ├── dataset_pariwisata_yogyakarta     # Folder of raw dataset "dataset_pariwisata_yogyakarta"
│   │   │   ├── tour.csv
│   │   │   ├── tour_rating.csv
│   │   │   └── user.csv
│   │   ├── indonesia_tourism_destination     # Folder of raw dataset "indonesia_tourism_destination"
│   │   │   ├── package_tourism.csv
│   │   │   ├── tourism_rating.csv
│   │   │   ├── tourism_with_id.csv
│   │   │   └── user.csv
│   │   └── yogyakarta_tourism_place          # Folder of raw dataset "yogyakarta_tourism_place"
│   │       └── raw_data.csv
│   ├── data.csv                              # Preprocessed data for machine learning model
│   ├── preprocessing_data.ipynb              # Notebook file of preprocessing data steps
│   └── README.md                             # Further explanation about the preprocessing data steps
├── models/                                   # Folder with machine learning models
│   ├── collaborative_filtering_model.ipynb   # Notebook file of developing model steps
│   ├── jgo.h5                                # Model file in h5 (HDF5) format
│   ├── jgo.pkl                               # Model file in pkl (Pickle) format
│   └── README.md                             # Further explanation about the developing model steps
└── README.md                                 # Project documentation
