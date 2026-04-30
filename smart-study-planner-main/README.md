
# Smart Study Planner 🧠

A premium, SaaS-style dashboard built with Python and Streamlit that optimizes study schedules using a **Dynamic Greedy Algorithm**.

<img width="1600" height="788" alt="Dashboard Preview" src="https://github.com/user-attachments/assets/ad7ae697-be4b-4795-8d69-5c84e5d3135e" />
[smart_study_planner_report.pdf](https://github.com/user-attachments/files/27251538/smart_study_planner_report.pdf)


## 🚀 Key Features

- **Dynamic Greedy Scheduling**: Allocates study hours based on difficulty, urgency, and a fairness penalty to prevent subject burnout.
- **SaaS Dashboard UI**: Dark-themed, glassmorphic interface with color-coded metric cards and interactive intensity heatmaps.
- **Resource Analytics**: Donut charts for time distribution and real-time utilization metrics.
- **Interactive Syllabus**: Add subjects dynamically and re-generate your plan instantly.
- **Exportable Plans**: Download your optimized schedule as a CSV file.

## 🧠 Algorithmic Thinking

The system demonstrates advanced algorithmic decision-making:
- **Heuristic Design**: Uses a custom priority function: `(Difficulty * 3) + (20 / DaysLeft)`.
- **Fairness Constraint**: Implements a *Progress Penalty*—every hour allocated to a subject reduces its priority temporarily. This ensures a balanced schedule where no single subject hogs all the available time.
- **Efficiency**: The algorithm runs in $O(n \log n)$ time complexity, ensuring the dashboard remains responsive even with dozens of subjects.

## 📦 Installation & Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/saatvic008/smart-study-planner.git
   cd smart-study-planner
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**:
   ```bash
   streamlit run app.py
   ```

## 🛠️ Tech Stack

- **Frontend**: Streamlit, Custom CSS
- **Visualization**: Plotly Express
- **Logic**: Python (Dynamic Greedy Heuristic)
- **Data**: Pandas
