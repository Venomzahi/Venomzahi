Here's a structured project documentation including setup instructions, an overview, approach description, and insights summary.

Quiz Performance Analysis & Recommendation Engine
Project Overview
This project is a Python-based solution for analyzing quiz performance and providing personalized recommendations to improve student preparation. The system retrieves quiz data from three sources:

Current Quiz Data: Contains details of the latest quiz submission, including selected options, topics, and correct answers.
Historical Quiz Data: Contains the last five quiz records per user, including scores and response mappings (question ID → selected option ID).
Objectives:
Identify student performance trends by topic and difficulty level.
Highlight weak areas and improvement patterns.
Generate personalized recommendations based on analysis.
Provide visual insights into student progress.
Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/quiz-performance-analysis.git
cd quiz-performance-analysis
2. Create a Virtual Environment (Optional but Recommended)
python3 -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
3. Install Required Dependencies
pip install -r requirements.txt
Or manually install required packages:
pip install pandas numpy matplotlib requests
4. Run the Application
python main.py
The script will:

Fetch data from API endpoints.
Analyze current and past quiz performance.
Generate insights, recommendations, and visualizations.
5. View Visualizations & Insights
Key metrics and recommendations will be printed in the console.
Performance trends will be visualized as graphs and saved in the screenshots/ folder.
Approach Description
1. Data Retrieval
The system fetches quiz data from these endpoints:

Current Quiz Data: https://jsonkeeper.com/b/LLQT
Historical Quiz Data:
https://api.jsonserve.com/rJvd7g
https://api.jsonserve.com/XgAgFJ
2. Data Processing
Current Quiz Analysis: Extract quiz questions, user responses, and correctness.
Historical Data Analysis: Retrieve past performance trends by score, topic, and difficulty.
Accuracy Calculation: Compute percentage accuracy per topic and difficulty level.
3. Performance Analysis
Identify weak topics where accuracy < 60%.
Analyze historical quiz score trends (improving, stagnant, or declining).
Evaluate performance across difficulty levels.
4. Recommendations Engine
Recommend topics to review based on low accuracy.
Identify difficulty levels to focus on for better practice.
Suggest personalized study strategies based on past performance.
5. Visualization & Reporting
Performance Trend Line Chart (Quiz scores over time).
Topic-wise Accuracy Table.
Difficulty Level Performance Breakdown.
Insights Summary with Actionable Steps.
Key Visualizations & Insights Summary
1. Historical Quiz Performance Trend
📌 Screenshot:
(Example Graph Image Placeholder)

📊 Description:

Tracks quiz scores over time.
An upward trend indicates improvement.
A declining/stagnant trend signals the need for better review strategies.
2. Topic-Wise Performance Breakdown
📌 Screenshot:
(Example Table Image Placeholder)

📊 Description:

Displays the number of questions, correct answers, and accuracy for each topic.
Topics with accuracy < 60% are flagged for improvement.
3. Difficulty Level Performance
📌 Screenshot:
(Example Chart Image Placeholder)

📊 Description:

Compares performance across Easy, Medium, and Hard questions.
Helps identify which difficulty level needs more focus.
Insights Summary & Recommendations
1. Weak Topics Identified:
Low accuracy topics need focused revision.
Example: If "Anatomy" has only 50% accuracy, targeted study is recommended.
2. Difficulty Level Weakness:
If "Medium" difficulty has low performance, practice medium-level questions more.
3. Historical Performance Trends:
If scores declined over the last 3 quizzes, review past mistakes and weak topics.
If scores are improving, continue the current study strategy.
4. Personalized Action Plan:
Review low-performing topics using targeted practice questions.
Focus on weak difficulty levels (Medium/Hard).
Attempt more quizzes consistently to reinforce learning.
Next Steps
✅ Improve visualization with interactive dashboards (e.g., using Plotly).
✅ Expand recommendation logic with AI-based adaptive learning suggestions.
✅ Build a web-based dashboard to display personalized insights.

