# Health AI - Coronary Heart Disease Prediction

Health AI is a web application designed to predict the likelihood of Coronary Heart Disease (CHD) based on user-provided health data. The frontend is built with **Next.js**, while the backend is powered by **Flask**, utilizing a machine learning model for predictions.

## Features
- User-friendly interface to input health metrics
- Machine learning model for CHD prediction
- Real-time data processing
- REST API for seamless integration between frontend and backend

## Tech Stack
### Frontend:
- **Next.js** (React framework)
- **Tailwind CSS** (for styling)
- **Axios** (for API requests)

### Backend:
- **Flask** (Python web framework)
- **Scikit-learn** (for ML model)
- **Pandas & NumPy** (data processing)

## Installation & Setup

### Prerequisites
Ensure you have the following installed:
- **Node.js** & **npm** (for the frontend)
- **Python 3** & **pip** (for the backend)

### Clone the Repository
```bash
git clone https://github.com/adamfutur/Coronary-hearth_disease.git
cd Coronary-hearth_disease
```

### Setting Up the Backend (Flask)
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
python app.py
```
The backend will start on `http://127.0.0.1:5000`

### Setting Up the Frontend (Next.js)
```bash
cd frontend
npm install
npm run dev
```
The frontend will be available at `http://localhost:3000`

## API Endpoints
### `POST /predict`
**Description:** Takes user health data and returns the CHD prediction.

**Request Body (JSON):**
```json
{
  "age": 45,
  "cholesterol": 200,
  "blood_pressure": 130,
  "smoking": 1,
  "diabetes": 0
}
```

**Response (JSON):**
```json
{
  "prediction": "High risk"
}
```

## Contributing
Feel free to fork this repository and submit pull requests. Contributions are welcome!

## License
This project is licensed under the MIT License.

---
**Author:** Adam Futur

