# J-GO_Travel-Recommendation
This project is a personal remake of J-GO (Jogja Uncovered), a team-based application, with refinements in the datasets and machine learning model. The goal is to provide personalized travel recommendations using machine learning techniques.

## Key Points
- **Problem**: Low engagement and accessibility in some tourist attractions in Daerah Istimewa Yogyakarta.
- **Proposed Solution**: Personalized travel recommendations with a dual-language feature.
- **Method**: Collaborative filtering tailored in the machine learning model.
- **Results**: Achieved high prediction accuracy with RMSE of 0.22 and MAE of 0.16, indicating minimal error in predicting user preferences on a 1-5 integer rating scale and meeting the benchmark of 0.25.

## Raw Datasets
- [Kaggle: Dataset Pariwisata Yogyakarta](https://www.kaggle.com/datasets/saufan/dataset-pariwisata-yogyakarta)
- [Kaggle: Indonesia Tourism Destination](https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination)
- [Kaggle: Yogyakarta Tourism Place](https://www.kaggle.com/datasets/mrafif/yogyakarta-tourism-place)

## Process Overview
1. **Data Gathering**: Collected tourist attractions and user datasets.
2. **Data Preprocessing**: Cleaned and converted datasets to ensure quality and usability.
3. **Model Development**: Applied collaborative filtering to the final dataset.
4. **Model Training and Evaluation**: Trained and evaluated model to ensure quality of results.

## File Structure
```
J-GO_Travel-Recommendation/  
│  
├── data/                                     # Data files folder  
│   ├── raw_data/                             # Raw dataset folder  
│   │   ├── dataset_pariwisata_yogyakarta     # Raw dataset "dataset_pariwisata_yogyakarta"  
│   │   │   ├── tour.csv  
│   │   │   ├── tour_rating.csv  
│   │   │   └── user.csv  
│   │   ├── indonesia_tourism_destination     # Raw dataset "indonesia_tourism_destination"  
│   │   │   ├── package_tourism.csv  
│   │   │   ├── tourism_rating.csv  
│   │   │   ├── tourism_with_id.csv  
│   │   │   └── user.csv  
│   │   └── yogyakarta_tourism_place          # Raw dataset "yogyakarta_tourism_place"  
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
```

## Further Implementation
The developed model can be deployed to an application or web service to provide real-time personalized travel recommendations to users. By integrating the model file (e.g., jgo.h5 or jgo.pkl) into a backend system, the application can process user inputs, including ratings, to generate tailored recommendations.

## Future Work
The current model can be further enhanced by integrating additional parameters to better capture user preferences and refine the recommendation system. For instance, integrating age or hobbies as parameters can offer more personalized recommendations, as travel preferences often vary based on these factors. By considering such parameters, the model could suggest more tailored and suitable destinations, thereby enhancing the overall user experience.
