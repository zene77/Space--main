# Space

---

#  SpaceX Falcon 9 First Stage Landing Prediction  
*A Technical Data Science & Machine Learning Project*

## 1. Project Summary
This repository contains a full end‑to‑end technical workflow to **predict the landing outcome of the SpaceX Falcon 9 first stage** using real launch data.  
The project integrates **API data collection**, **web scraping**, **data engineering**, **EDA**, **feature selection**, and **machine learning model development**.

The goal is to build a reproducible pipeline capable of estimating the probability of a successful booster landing, a key factor in SpaceX’s cost‑reduction strategy.

---

## 2. Repository Structure
- `data/` — Raw and processed datasets (CSV, API responses, scraped tables).  
- `notebooks/` — Jupyter notebooks for each stage of the pipeline:
  - Data collection (API + web scraping)  
  - Data wrangling and cleaning  
  - EDA and visualization  
  - Feature engineering  
  - Model training and evaluation  
- `scripts/` — Modular Python scripts for reusable components.  
- `spacex_launch_geo.csv` — Launch site geolocation dataset.  
- `README.md` — Technical documentation.

---

## 3. Technical Stack
- **Python 3.10+**  
- **Pandas**, **NumPy** — data manipulation  
- **Matplotlib**, **Seaborn**, **Folium** — visualization  
- **Scikit‑learn** — machine learning models  
- **Requests**, **BeautifulSoup** — API and web scraping  
- **Jupyter Notebook** — interactive development  

---

## 4.  Data Engineering Workflow
- **Data acquisition** from:
  - SpaceX REST API  
  - Web scraping launch tables  
  - CSV datasets  
- **Data cleaning**:
  - Handling missing values  
  - Normalizing categorical fields  
  - Resetting flight numbers  
  - Converting data types  
- **Feature engineering**:
  - Binary encoding of landing outcomes  
  - One‑hot encoding of categorical variables  
  - Derived features (e.g., booster reuse count)  

---

## 5. Exploratory Data Analysis (EDA)
The EDA phase includes:  
- Correlation analysis  
- Distribution analysis of payload mass, orbit types, and launch sites  
- Geospatial visualization of launch pads using Folium  
- Trend analysis of booster reuse and landing success  

Key insights are documented in the notebooks.

---

## 6.  Machine Learning Models
Models implemented and compared:  
- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  
- Support Vector Machine (SVM)  

Evaluation metrics:  
- Accuracy  
- F1‑score  
- Confusion matrix  
- Cross‑validation  

Model selection is based on performance and interpretability.

---

## 7.How to Reproduce
```bash
# Clone repository
git clone <repo-url>

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

