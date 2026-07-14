# 🎓 AI Tutor — Personalized Student Learning Recommendations

An AI-powered web application that analyzes student performance data (marks, attendance, and study time) and generates personalized, subject-wise learning recommendations using a Machine Learning model.

Built with **Streamlit**, **Scikit-learn**, and **Plotly**.

---

## 📌 Project Goal

Traditional grading only tells students *what* they scored, not *how to improve*. This project uses a Machine Learning-based classifier to analyze a student's marks, attendance, and time spent studying per subject, then generates actionable, explainable recommendations to help them focus their effort where it matters most.

## 🧠 PEAS Description

| Component | Description |
|---|---|
| **Performance** | Accuracy of personalized learning recommendations |
| **Environment** | Web-based learning platform with student data |
| **Actuators** | Recommendation text, performance charts, and downloadable reports |
| **Sensors** | Student performance data (CSV input): marks, attendance, study time |

## ✨ Features

- 📂 Upload your own student dataset (CSV) or use the built-in sample data
- 🔍 Select any student to view a detailed performance analysis
- 🎯 Personalized, subject-wise learning recommendations
- 📊 Interactive charts and visualizations (Plotly)
- 🤖 AI-powered predictions using a Random Forest Classifier
- 💡 Explainable AI — recommendations are transparent, not a black box
- 📥 Download a text report of a student's recommendations

## 🛠️ Tech Stack

- **Python**
- **Streamlit** — web app framework
- **Scikit-learn** — Random Forest classification model
- **Pandas / NumPy** — data processing
- **Plotly / Matplotlib** — data visualization

## 📁 Project Structure

```
AI_Tutor-Project/
├── app.py                # Main Streamlit application
├── requirements.txt      # Python dependencies
├── student_data.csv      # Sample dataset
├── report.pdf            # Project report
├── Screenshots/          # App screenshots
└── README.md
```

## 📊 Dataset Format

The app expects a CSV with the following columns:

| Column | Description |
|---|---|
| `Student_ID` | Unique identifier for each student |
| `Subject` | Subject name (e.g., Math, Science, English) |
| `Marks` | Marks scored in the subject (0–100) |
| `Time_Spent` | Hours spent studying the subject per week |
| `Attendance` | Attendance percentage for the subject |

## 🤖 Machine Learning Model

- **Algorithm:** Random Forest Classifier
- **Task:** Classifying student performance level per subject to drive recommendation logic
- **Inputs:** Marks, attendance, and time spent studying

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/AI_Tutor-Project.git
   cd AI_Tutor-Project
   ```

2. **Install the required libraries**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. Open the local URL shown in your terminal (usually `http://localhost:8501`) in your browser.

## 🖼️ Screenshots

> Screenshots of the application are available in the [`Screenshots/`](./Screenshots) folder.

## 🔮 Future Improvements

- Train on a larger, real-world student dataset
- Improve prediction accuracy with additional features (e.g., quiz scores, homework completion)
- Support real-time / live data updates
- Add long-term student progress tracking
- Deploy the app on Streamlit Cloud

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

## 👥 Contributors

- **Hassnain Nawaz**
- **Saifullah Ali**
- **Sohail Abbas**
