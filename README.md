# Electricity Demand Predictor

This project is an Artificial Intelligence (AI) based model developed for the Smart India Hackathon (SIH) 2024, addressing problem statement #1624: "To develop an Artificial Intelligence (AI) based model for electricity demand projection including peak demand projection for Delhi Power system." The model predicts electricity demand, focusing on the Delhi power system.

## 🚀 Features

- **Data Extraction**: The `Data_extracting` module automatically downloads daily electricity consumption reports in PDF format from the official Grid-India portal.
- **Data Mining**: The `Data_Mining` module processes the downloaded PDFs to extract relevant data for all states and Union Territories, preparing it for analysis and model training.
- **Machine Learning Model**: The core of the project is an XGBoost Regressor model, detailed in the `sih-ps-1624.ipynb` notebook. It predicts two key metrics:
    -   `Max Demand Met (MW)`
    -   `Energy Met (MU)`
- **Frontend**: A basic web interface is available in the `Frontend` directory, allowing users to interact with the model and view predictions.

## 📊 Dataset

The dataset, containing electricity data for India from 2020 to 2025, has been compiled and is available on Kaggle. You can access it here: [Indian Power Demand and Shortage Data 2020-2025](https://www.kaggle.com/datasets/preygle/indian-power-demand-and-shortage-data-2020-2025).

## 📂 Project Structure

```
.
├── Data_extracting/      # Scripts to download electricity data PDFs
├── Data_Mining/          # Scripts to parse PDFs and extract data
├── Frontend/             # HTML/CSS for the web interface
│   ├── style.css
│   └── web.html
├── sih-ps-1624.ipynb     # Jupyter notebook with the ML model
└── README.md
```

## ⚙️ How to Use

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/PiyushAgrawal626/SIH.git
    ```
2.  **Data Collection:**
    -   Run the script in the `Data_extracting` directory to download the raw PDF reports.
3.  **Data Processing:**
    -   Execute the script in the `Data_Mining` directory to process the PDFs and generate a structured dataset.
4.  **Model Training & Prediction:**
    -   Open and run the `sih-ps-1624.ipynb` notebook to train the XGBoost model and generate predictions.
5.  **View the Frontend:**
    -   Open the `Frontend/web.html` file in a web browser to see the user interface.

## 🏆 Team

This project was developed by a team of 6 members for the Smart India Hackathon 2024.