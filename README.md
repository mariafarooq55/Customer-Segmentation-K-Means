# Customer Segmentation with K-Means

This project builds a customer segmentation model using the Mall Customers dataset and presents it in a Streamlit web app.

The app helps users describe a customer by annual income and spending score, then predicts which customer segment they most likely belong to using a trained K-means clustering model.

## Project overview

- Uses the `Mall_Customers.csv` dataset
- Trains a K-means customer segmentation model
- Labels customers into business-friendly segments
- Displays segment hints and marketing ideas in a Streamlit dashboard
- Includes a notebook for exploration and model preparation

## Files in this project

- `app.py` – Streamlit interface for the segmentation app
- `Mall_Customers.csv` – raw customer dataset
- `requirements.txt` – Python dependencies
- `segment_model.pkl` – trained model artifact (generated during model prep)
- `Mall_Customers_clean.csv` – cleaned data used by the app (generated during model prep)

## Features

- Interactive income and spending score sliders
- K-means customer group prediction
- Segment-specific marketing suggestion
- Visualization of all customers and the current customer in one chart
- Summary table of segment names and groups

## Setup

1. Clone or download this project.
2. Open a terminal in the project folder.
3. Create and activate a virtual environment (optional but recommended):

```bash
python -m venv .venv
.venv\Scripts\activate
```

4. Install the required dependencies:

```bash
pip install -r requirements.txt
```

5. Generate the trained model artifact and cleaned dataset if they are not already present.
   - Open and run the notebook `Lab 4 - Customer Segmentation (K-means).ipynb`.
   - Ensure the output files `segment_model.pkl` and `Mall_Customers_clean.csv` are saved in the project root.

## Run the app

```bash
streamlit run app.py
```

## Live link of the project:

https://customer-segmentation-k-means-nrgednx7ew6chsxnsjxvpd.streamlit.app/

## Example workflow

- Enter a customer’s annual income and spending score
- The app scales the values using the same preprocessing as training
- K-means predicts the most likely customer segment
- The app shows the segment label and a relevant marketing suggestion

## Dataset

The dataset includes customer information such as:

- Customer ID
- Gender
- Age
- Annual income (in thousands of dollars)
- Spending score (1–100)

## Tech stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Streamlit
- Joblib

## Notes

This is a simple demo project for customer segmentation and marketing analysis. It is useful for learning clustering workflows and building interactive ML dashboards.
