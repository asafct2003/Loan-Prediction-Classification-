:

🏦 Loan Prediction Web App

This is a Flask-based web application that predicts whether a loan application will be Approved or Rejected using a trained Machine Learning model (loan_pipeline.pkl).
Users can input their details through a simple web form, and the app returns the prediction along with the probability.

📁 Project Structure
├── app.py                  # Main Flask application
├── loan_pipeline.pkl       # Trained ML pipeline (model + preprocessing)
├── Loan.csv                # Dataset used for model training
├── loanprediction.ipynb    # Jupyter Notebook for training the model
├── requirements.txt        # Python dependencies
├── templates/
│   └── index.html          # Frontend UI for input and prediction
├── static/
    ├── style.css           # (Optional) Custom styling

🚀 Features

✔ Web-based interface for loan approval prediction
✔ ML model built using Scikit-learn Pipeline
✔ Handles categorical + numerical features
✔ Displays prediction with probability
✔ Error-handling for invalid inputs

⚙️ Tech Stack
Component	Technology Used
Backend	Flask (Python)
Machine Learning	Scikit-learn
Frontend	HTML, CSS (Jinja2)
Data Handling	Pandas, NumPy
📌 How to Run Locally
✅ 1. Clone the Project
git clone <repository_link>
cd <project_folder>

✅ 2. Create Virtual Environment (Optional but Recommended)
python -m venv venv
venv/Scripts/activate   # For Windows
source venv/bin/activate  # For macOS/Linux

✅ 3. Install Dependencies
pip install -r requirements.txt

✅ 4. Run the App
python app.py

✅ 5. Open in Browser

Go to: http://127.0.0.1:5000/

🧠 Model Information

The pipeline includes:

Imputation (missing values)

One-Hot Encoding (categorical features)

Classification algorithm (e.g., Logistic Regression / RandomForest)

Input features required:

Gender, Married, Dependents, Education, Self_Employed,
ApplicantIncome, CoapplicantIncome, LoanAmount,
Loan_Amount_Term, Credit_History, Property_Area

🖼 UI Preview (index.html)

Form for input fields (dropdown/text boxes)

Submit button → /predict

Result displayed below as:
✅ Loan Approved (Probability: 78.56%)
❌ Loan Rejected (Probability: 22.11%)

✅ Future Enhancements

Add attractive CSS design / Bootstrap styling

Add data visualization dashboard

Deploy on Render / Railway / AWS / Heroku

Add user authentication