# UniMatch - University Recommendation System

UniMatch is a quick recommendation system for international MS students that simplifies the process of shortlisting universities in the US, according to their majors. It provides a personalized experience, saves time and money, and offers a one-click solution for finding the best universities based on individual preferences and qualifications.

**You can try UniMatch by visiting our website:**
[UniMatch - University Recommendation System](http://pbadhe.pythonanywhere.com/)

## Technology Stack
- Backend: Flask
- Frontend: Bootstrap, HTML5
- Deployment: pythonAnywhere
- Machine Learning: scikit-learn (sklearn) library

## Installation
To run UniMatch locally, follow these steps:
1. Clone the repository: `git clone https://github.com/yourusername/unimatch.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the application: `python app.py`
4. Access UniMatch in your browser at [http://localhost:5000](http://localhost:5000)

## Usage
1. Open UniMatch in your web browser.
2. Enter your profile and preferences.
3. Click on the "Submit" button to receive personalized university recommendations.
4. Explore the recommended universities and their details through the links provided.

## Data
UniMatch leverages data collected from various sources to provide comprehensive and reliable recommendations. The data is obtained from the following sources using Beautiful Soup.
- ymgrad
- thegradcafe
- edulix
- kaggle

This diverse dataset allows UniMatch to capture a wide range of student profiles and university information, ensuring more accurate and inclusive recommendations.

## Algorithm
UniMatch utilizes a weighted K-nearest neighbors (KNN) algorithm to generate accurate and relevant university recommendations. The algorithm incorporates the following techniques:
- Major-wise Top X Universities: UniMatch identifies the top X universities for each major or field of study based on factors like reputation, faculty, research opportunities, and alumni feedback.
- Applicant-Applicant Similarity: The algorithm determines the similarity between applicants' profiles to identify universities where students with similar profiles have been successful in the past.
- Weighted Features: UniMatch assigns appropriate weights to different features and criteria based on their importance and relevance to generate more accurate recommendations.
- Distance Weighted Neighbors: The algorithm calculates distances or similarities between applicants and universities, considering weighted features, to find the nearest neighbors.
- Rank-wise Top 10 Universities for each input: UniMatch ranks the universities based on their suitability and recommends the top 10 universities for each input profile.
