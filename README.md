# Indian-Premier-League-Match-Predictor
# **IPL Match Prediction Pipeline**

This repository contains a full pipeline for cleaning, processing, and predicting IPL match outcomes using historical data, statistical features, and a weighted prediction model.

## **Modules Overview**

### **1. Data Preprocessing and Cleaning**
- Cleans and standardizes IPL match and team data.
- Filters data to include only final teams and venues.
- Outputs: `match_data_cleaned.csv`, `team_data_cleaned.csv`

### **2. Feature Statistics Computation**
- Computes head-to-head (H2H), venue performance, toss impact, and batting/bowling performance.
- Saves computed statistics to `feature_stats.xlsx`.

### **3. IPL 2024 Group Stage Data Processing**
- Extracts and standardizes IPL 2024 group stage match data.
- Outputs: `ipl_2024_group_stage.csv`

### **4. IPL 2025 Group Stage Data Processing**
- Processes IPL 2025 fixture data.
- Maps venue names and extracts teams.
- Outputs: `ipl_2025_group_stage.csv`

### **5. IPL 2024 Group Stage Prediction and Evaluation**
- Uses a weighted prediction model with toss impact, H2H, and venue performance.
- Evaluates prediction accuracy.
- Generates a simulated points table and playoff predictions.

### **6. IPL 2025 Group Stage Prediction and Evaluation**
- Predicts IPL 2025 match outcomes using the same model.
- Simulates playoffs and predicts the winner.

### **7. Web Scraping IPL 2024 Knockout Matches**
- Scrapes actual knockout stage match results.
- Compares predicted vs. actual outcomes.
- Visualizes results.

## **Installation and Usage**

1. Clone the repository:
   ```sh
   git clone https://github.com/SuryaMuruganMS/Indian-Premier-League-Match-Predictor.git
   cd Indian-Premier-League-Match-Predictor
   ```

2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

3. Run each module as needed:
   ```sh
   python module1_preprocessing.py
   python module2_feature_stats.py
   python module3_ipl2024_processing.py
   python module4_ipl2025_processing.py
   python module5_ipl2024_prediction.py
   python module6_ipl2025_prediction.py
   python module7_web_scraping.py
   ```

## **Results**
- Cleaned datasets: `match_data_cleaned.csv`, `team_data_cleaned.csv`
- Feature statistics: `feature_stats.xlsx`
- Predicted results for IPL 2024 & 2025
- Simulated playoffs and points tables
- Web-scraped knockout results

## **License**
This project is open-source and available under the MIT License.

## **Contributors**
- Surya Murugan M S (@SuryaMuruganMS)
