# STUDENT-PERFORMANCE-ANALYSIS-1-PROJECT
Power BI dashboard analyzing 10,000 students to uncover what drives placement. 84% placement rate, correlation analysis.
# Student Performance & Placement Analytics Dashboard - Power BI

> Analyzing what drives student placement success using data from 10,000 students.

As a Statistics graduate and aspiring Investment Analyst / Portfolio Manager, I built this dashboard to apply statistical analysis and financial-style KPI tracking to education data.

This is the same mindset used in portfolio management: track performance, find leading indicators, and identify risk early.

<img width="994" height="553" alt="STUDENT DATA 3 - Copy - Copy" src="https://github.com/user-attachments/assets/c847e4b0-b329-4eb5-8bae-e9b77c7412cc" />
<img width="986" height="554" alt="STUDENT DATA 2 updated png - Copy - Copy" src="https://github.com/user-attachments/assets/81f3e477-38ac-4b5c-b731-474df75aaed6" />
<img width="988" height="555" alt="STUDENT DATA 1 - Copy - Copy" src="https://github.com/user-attachments/assets/e73c8236-f8f6-4095-8083-a10e5f40ffcf" />

---

### 📊 Dataset Overview
- **10,000 Students** (8K Placed, 2K Not Placed)
- Metrics: Exam Score, Attendance, Study Hours, Sleep Hours, Internet Usage, Assignment Performance, Improvement Status
- Segments: High Performer, Average, Distracted, At-Risk

### 🎯 Key KPIs
- **Avg Exam Score:** 86.70
- **Placement Rate:** 84% (Gauge Visual)
- **Improvement Rate:** 88%
- **Placed Avg Score:** 92.00 vs **Not Placed Avg Score:** 59.80 (32.2 point gap)
- **At-Risk:** 2%
- **Study Efficiency:** 14.48

### 📑 Dashboard Pages

**Page 1 - Executive Overview:**
- Top 20 Students by Exam Score
- Exam Score by Attendance (High: 91, Medium: 89, Low: 84)
- Performance Breakdown (78.14% Average, 14.81% High Performer)
- Placement Rate Gauge

**Page 2 - Placement Drivers:**
- Total Improvement Status (88.29% Improved)
- Placed vs Not Placed Total (8K vs 2K)
- Assignment Performance by Placement (Placed 53.69% vs Not Placed 30.89%)
- Students at Risk Table (212 At-Risk = 100% Not Placed)

**Page 3 - Correlation Analysis:**
- Sleep Hours vs Exam Score: Positive correlation, good sleep (6-9 hrs) in Average/Good bucket performs best
- Study Hours vs Exam Score: Strong positive correlation, upward trendline - more hours = higher score
- Internet Usage vs Exam Score: Slight negative correlation - Light/Moderate users outperform Heavy users

### 💡 Key Insights & Recommendations

1. **The 32-point Gap:** Placement is directly tied to exam performance. Intervention must target the 59.80 average group.
2. **Attendance is Alpha:** +7 points difference between high and low attendance. Consistency matters - same as in investing.
3. **Assignments are Leading Indicators:** Low assignment scores predict non-placement early.
4. **The Average Trap:** 78% are average. The real opportunity is moving average to high performer, not just fixing the 2% at-risk.
5. **Lifestyle Factors:** Study hours and sleep drive performance more than internet access.

### 🛠️ Tools & Techniques Used
- **Power BI Desktop**
- **DAX:** Measures for Avg Score, Placed Avg, Not Placed Avg, Study Efficiency, At Risk %
- **Data Cleaning & Modeling**
- **Visuals:** Bar Chart, Donut, Gauge, Scatter Plot, Slicers (Student Segment, Placement Status, Attendance, Study Hours)
- **Statistical Analysis:** Correlation analysis using scatter plots with trendlines

### 🔗 Sample DAX Measures
```dax
Avg Exam Score = AVERAGE('Students'[exam_score])
Placed Avg Score = CALCULATE(AVERAGE('Students'[exam_score]), 'Students'[placement_status]="Placed")
Placement Rate % = DIVIDE([Total Placed], [Total Students])
<img width="994" height="553" alt="STUDENT DATA 3 - Copy - Copy" src="https://github.com/user-attachments/assets/1b5665f7-0c10-4f5b-a9a6-800693ff96b4" />
<img width="986" height="554" alt="STUDENT DATA 2 updated png - Copy - Copy" src="https://github.com/user-attachments/assets/8eb1338f-367f-4d32-8b27-00bc29198d69" />
<img width="988" height="555" alt="STUDENT DATA 1 - Copy - Copy" src="https://github.com/user-attachments/assets/5a229860-4f79-4677-ad47-d97fafa27462" />
