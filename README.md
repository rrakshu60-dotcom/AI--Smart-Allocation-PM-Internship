 AI-Based Smart Allocation System for PM Internship

 Overview

This project is an AI-driven internship recommendation system designed to match candidates with relevant internship opportunities based on their profile, skills, and preferences.

The system leverages Natural Language Processing (NLP) and similarity-based machine learning techniques to provide personalized recommendations, simulating a real-world intelligent allocation system.

---

 Objectives

- Automate the internship allocation process
- Provide personalized recommendations using AI techniques
- Improve decision-making through data-driven insights
- Reduce manual effort in filtering and matching candidates

---

 System Design

🔹 Backend

- Developed using FastAPI
- Handles:
  - User registration
  - Eligibility validation
  - Recommendation generation via API endpoints

---

🔹 Recommendation Engine

The core engine uses a hybrid scoring approach:

- Text Vectorization
  
  - TF-IDF applied on internship data (title, description, skills, category, location)

- Similarity Measurement
  
  - Cosine similarity between user profile and internship dataset

- Custom Scoring
  
  - Skill match score
  - Location preference score
  - Stipend-based weighting

---

🔹 Data Handling

- Internship data stored in CSV format (~1000 records)
- User data handled in in-memory storage during runtime
- Data preprocessing includes:
  - Missing value handling
  - Feature normalization
  - Text feature engineering

---

🔹 Frontend

- Built using HTML, CSS, and JavaScript
- Provides:
  - User profile input interface
  - Skill selection mechanism
  - Interactive recommendation display

---

 Technologies Used

- Python
- FastAPI
- Pandas, NumPy
- Scikit-learn (TF-IDF, Cosine Similarity)
- HTML, CSS, JavaScript

---

 Workflow

1. User inputs profile details (skills, location, interests)
2. System processes and vectorizes the input
3. Internship dataset is transformed using TF-IDF
4. Similarity scores are computed
5. Additional weighted scoring is applied
6. Top matching internships are returned

---

 How to Run

1. Install dependencies

pip install fastapi uvicorn pandas numpy scikit-learn

2. Start backend server

python main.py

Server will run at:

http://127.0.0.1:8000

3. Run frontend

- Open "index.html" in a browser
- Fill in details and view recommendations

---

Use Cases

- Internship recommendation platforms
- Career guidance systems
- Skill-based job matching solutions
- Educational and EdTech applications

---

Future Enhancements

- Integration with relational databases (MySQL/PostgreSQL)
- Real-time internship data integration via APIs
- Advanced ML models for improved recommendation accuracy
- Full-stack deployment with scalable frontend frameworks

---

Author

Rakshitha S


Minor Project – AI-Based Smart Allocation System for PM Internship

---

💬 Summary

This project demonstrates the application of machine learning, backend development, and frontend integration to build an intelligent system capable of solving real-world allocation and recommendation problems.
