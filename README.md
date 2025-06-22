
---

## 🧠 Stock Price Prediction Using Deep Learning

This project predicts stock prices using historical data and a deep learning model (LSTM), integrated with a Flask web interface for interactive prediction and visualization.

### 📂 Project Structure

```
.
├── app.py                  # Flask app to interact with model & visualize predictions
├── analysis.ipynb          # Exploratory Data Analysis and model training
├── requirements.txt        # Project dependencies
├── templates/
│   └── index.html          # HTML template for the frontend (not uploaded here)
├── static/
│   ├── *.png               # Generated plots
│   └── *.csv               # Exported datasets
└── stock_dl_model.h5       # Pre-trained LSTM model (not uploaded here)
```

---

### 🔍 Features

* 📈 **Stock Price Prediction** using LSTM
* 🕵️ **Interactive Web Interface** with Flask
* 📊 Visualization of:

  * EMAs (20, 50, 100, 200 days)
  * Original vs Predicted trend
* ⏳ Automatic data download using `yfinance`
* 📥 Downloadable CSV of full stock dataset

---

### 🚀 Getting Started

#### 1. Clone the repository and install dependencies

```bash
git clone https://github.com/yourusername/stock-prediction-ml.git
cd stock_market_prediction_ml_project
pip install -r requirements.txt
```

#### 2. Add your trained model

Place your trained LSTM model file as `stock_dl_model.h5` in the project root.

> If you don’t have it, train using `analysis.ipynb`.

#### 3. Run the Flask app

```bash
python app.py
```

Then open [http://127.0.0.1:5000/](http://127.0.0.1:5000/) in your browser.

---

### 📓 Notebook Details (`analysis.ipynb`)

* Exploratory Data Analysis using `yfinance` data
* LSTM model built using TensorFlow/Keras
* Feature scaling with `MinMaxScaler`
* Model trained and saved as `stock_dl_model.h5`

---

### 🔧 Requirements

From `requirements.txt`:

```
ipykernel
numpy
pandas
matplotlib
scikit-learn
seaborn
scipy
plotly
tensorflow
```

Install with:

```bash
pip install -r requirements.txt
```

---

### 📸 Screenshots

Plots generated:

* **EMA Trendlines** (20/50, 100/200 Days)
* **Prediction vs Actual Price**

---

### 📁 Example Output

* 📉 `static/stock_prediction.png`
* 📊 `static/ema_20_50.png`, `static/ema_100_200.png`
* 📄 `static/<stock>_dataset.csv`

---

### 🛠️ Future Improvements

* Add interactive Plotly charts
* Deploy to cloud (e.g., Heroku, AWS)
* Include model training interface
* Add sentiment analysis of stock news

---

### 🧑‍💻 Author

Abrar Ahmad
Feel free to reach out for collaboration or improvements!

---


