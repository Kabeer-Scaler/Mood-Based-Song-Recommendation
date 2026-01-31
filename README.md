# Mood-Based-Song-Recommendation

## Folder Structure
```text
├── Mood_Based_Song_Recommendation.ipynb  # Main project notebook
├── dataset/
│   └── spotify_data.csv                  # Song dataset (114k tracks)
├── README.md                             # Project documentation


## Dependencies
The following Python libraries are required to run this project:

### Data Handling: pandas, numpy

### Machine Learning: scikit-learn, scipy

### Personalization Engine: scikit-surprise

### Visualization: matplotlib, seaborn, plotly

## How to Run the Project
### 1. Environment Setup
It is recommended to run this project in Google Colab for the best compatibility with the visualization libraries.

### 2. Install Required Libraries
Open the notebook and run the following command in the first cell to install the personalization engine:
!pip install scikit-surprise

### 3. Upload the Dataset
Upload your spotify_data.csv file to the Colab runtime environment or mount your Google Drive if the dataset is stored there.

### 4. Execute the Notebook
Run the cells in order:

Data Pre-processing: Cleans and scales the audio features.

GMM Clustering: Performs model selection and defines mood clusters.

SVD Training: Synthesizes interaction data and trains the personalization model.

Hybrid Function: Run the final cell to define the give_hybrid_recommendation function.

### 5. Generate Recommendations
To get a recommendation, call the hybrid function with a user_id and a mood:
give_hybrid_recommendation(user_id, mood)
