🚧 Accident Severity Prediction App
This is a Streamlit-based web application that predicts the severity of road accidents (Slight Injury, Serious Injury, or Fatal Injury) based on user input about various conditions surrounding the accident. The prediction is made using a trained XGBoost classification model.

🔍 Features
Predicts accident severity using machine learning (XGBoost)

Interactive form interface using Streamlit

Encodes categorical variables using Label Encoding

Uses historical accident data features such as:

Time and day of accident

Driver’s age and experience

Road conditions (surface type, lighting, etc.)

Vehicle movement and type of collision

Casualty details and cause of accident

🧠 Model
XGBoost Classifier is trained and saved as a binary file.

Label encoders for various categorical features are also saved and loaded during runtime.

📁 Project Structure
pgsql
Copy
Edit
📦AccidentPredictionApp
 ┣ 📂model
 ┃ ┣ 📜model_xgb.bin
 ┃ ┗ 📜checkpoint.pkl
 ┣ 📜app.py              # Main Streamlit application
 ┣ 📜prediction.py       # Contains the prediction logic
 ┣ 📜config.py           # Dictionaries and configuration for preprocessing
 ┗ 📜requirements.txt    # List of dependencies (to be created)
🚀 How to Run
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/accident-prediction-app.git
cd accident-prediction-app
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the app:

bash
Copy
Edit
streamlit run app.py
📷 Screenshots
(Add screenshots of your app UI here)

✅ Inputs Considered
Time of accident (Day/Night)

Day of the week

Age and experience of driver

Surface and lighting conditions

Type of collision and vehicle movement

Casualty’s age and occupation

Cause of the accident

🧩 Output
Predicts accident severity as:

Slight Injury

Serious Injury

Fatal Injury

📦 Libraries Used
Streamlit

XGBoost

Pandas, NumPy

Joblib / Pickle

PIL
