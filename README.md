# 🏦 Bank Note Authentication API - FastAPI Deployment 🚀  

## 📌 Project Overview  

This FastAPI-based **Bank Note Authentication API** helps determine whether a given banknote is **genuine** or **fake** based on its **variance, skewness, curtosis, and entropy**. The model is trained and deployed using **FastAPI**, and predictions are served through a RESTful API.  

---

## 📡 API Endpoints  

### ✅ Home Endpoint  
**GET** `/`  
Returns a welcome message.  
```json
{
    "Message": "Hello Stranger"
}
```

### ✅ Personalized Welcome  
**GET** `/Welcome/{name}`  
Returns a personalized welcome message.  
```json
{
    "Message": "Hello Uvie"
}
```

### ✅ Predict Bank Note Authenticity  
**POST** `/predict`  
Accepts banknote features and predicts if it is **genuine** or **fake**.  

#### 📥 Request (JSON)  
```json
{
    "variance": 2.3,
    "skewness": 1.2,
    "curtosis": 3.5,
    "entropy": -0.8
}
```

#### 📤 Response (JSON)  
```json
{
    "Prediction": "Fake Note"
}
or
{
    "Prediction": "Bank Note"
}
```

---

## 🏗️ Model & Deployment Details  

- **Machine Learning Model**: Pre-trained classifier (`classifier.pkl`).
- **Framework**: FastAPI for serving predictions.
- **Server**: Uvicorn for asynchronous handling.
- **Data Validation**: Pydantic (`BankNotes.py`).
- **Deployment Ready**: Can be containerized with Docker & deployed to cloud platforms.

---

## 📜 Requirements  

- Python 3.8+  
- FastAPI  
- Uvicorn  
- Scikit-learn  
- Pandas  
- Pickle  


---

## 🏷️ Tags  

**#FastAPI #MachineLearning #BankNoteAuthentication #API #ModelDeployment #Python**  

