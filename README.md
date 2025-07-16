# 🚀 FastAPI Projects Collection

This repository contains 3 FastAPI-based projects designed to build and showcase real-world API development using FastAPI, Pydantic, and Python.

---

## 📚 Projects Included

1. [🧪 FAST_API_DEMO](#-1-fast_api_demo)
2. [🔮 INSURANCE_PREMIUM_PREDICTION_FASTAPI](#-2-insurance_premium_prediction_fastapi)
3. [📘 PYDANTIC](#-3-pydantic)
4. [▶️ How to Run Any Project](#️-how-to-run-any-project)
5. [🛠️ Tech Stack](#️-tech-stack)
6. [📃 License](#-license)

---

## 🧪 1. FAST_API_DEMO

A beginner-level demo project using FastAPI and Pydantic to explore:

- API creation
- Request parameters (path/query/body)
- Basic validation

### 📁 Folder: `FAST_API_DEMO/`

### 📂 File Structure

```
FAST_API_DEMO/
├── main.py             # FastAPI application
├── model.py            # Pydantic models
└── requirements.txt    # Dependencies
```

### 🔗 API Endpoints

| Method | Endpoint         | Description           |
|--------|------------------|-----------------------|
| GET    | `/`              | Welcome route         |
| GET    | `/get-item/{id}` | Get item by ID        |
| POST   | `/create-item`   | Create an item        |

---

## 🔮 2. INSURANCE_PREMIUM_PREDICTION_FASTAPI

A real-world API that loads a machine learning model and predicts health insurance premiums based on input features.

### 📁 Folder: `INSURANCE_PREMIUM_PREDICTION_FASTAPI/`

### 📂 File Structure

```
INSURANCE_PREMIUM_PREDICTION_FASTAPI/
├── main.py             # FastAPI app serving ML model
├── model.pkl           # Trained scikit-learn model
└── requirements.txt    # Required libraries
```

### 🔗 API Endpoint

| Method | Endpoint  | Description               |
|--------|-----------|---------------------------|
| POST   | `/predict` | Predict insurance premium |

### 📤 Sample Request

```json
{
  "age": 35,
  "bmi": 24.5,
  "children": 1,
  "sex": "female",
  "smoker": "no",
  "region": "northwest"
}
```

### ✅ Sample Response

```json
{
  "prediction": 4563.78
}
```

---

## 📘 3. PYDANTIC

A Pydantic crash course project that demonstrates how to use Pydantic with FastAPI for:

- Schema definition
- Data validation
- Default and optional fields
- Nested models

### 📁 Folder: `PYDANTIC/`

### 📂 File Structure

```
PYDANTIC/
├── main.py             # FastAPI app using Pydantic
├── model.py            # Schema definitions
```

### 📤 Sample Payload

```json
{
  "id": 1,
  "name": "Alice",
  "age": 30,
  "email": "alice@example.com"
}
```

---

## ▶️ How to Run Any Project

```bash
# Step into any project folder
cd PROJECT_FOLDER

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run FastAPI app
uvicorn main:app --reload
```

Visit Swagger docs: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 🛠️ Tech Stack

- FastAPI
- Pydantic
- Uvicorn
- Scikit-learn (ML model)
- Python 3.10+

---

## 📃 License

MIT License – Free to use for learning and development.

---

## 🙌 Credits

Inspired by CampusX tutorials. Collected here to help learn FastAPI through practice.
