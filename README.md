# 🏊 Goldfish Swim School AI Business Intelligence & Sentiment Analysis Project

## Project Overview

This project demonstrates how data analytics and Generative AI can be used to support operational decision-making for a swim school business.

Using enrollment, attendance, capacity utilization, and parent feedback data, the project generates:

* Operational KPI reporting
* Capacity utilization analysis
* Location performance analysis
* Time-slot demand analysis
* Overflow and underutilization detection
* AI-generated business insights
* AI-powered parent review sentiment analysis

The final output is an automated Excel business report designed for managers and operations teams.

---

## Business Problem

Swim schools often face several operational challenges:

* Some classes exceed planned capacity (Overflow)
* Some classes remain underutilized
* Demand varies by location and time slot
* Parent feedback is difficult to analyze at scale
* Managers spend significant time creating reports manually

This project automates operational reporting and provides AI-generated recommendations to support scheduling and resource allocation decisions.

---

## Dataset

The project uses operational swim school data including:

| Column             | Description                 |
| ------------------ | --------------------------- |
| Date               | Class date                  |
| Location           | Swim school location        |
| Class_Time         | Scheduled class time        |
| Students_in_Class  | Number of enrolled students |
| Class_Capacity     | Maximum class capacity      |
| Attendance_Status  | Attendance result           |
| Parent_Rating      | Parent satisfaction score   |
| Parent_Review_Text | Parent comments and reviews |

---

## Key Metrics

### Occupancy Rate

Occupancy Rate = Students in Class / Class Capacity

Classification:

| Occupancy Rate | Status        |
| -------------- | ------------- |
| > 100%         | Overflow      |
| 90% – 100%     | Near Full     |
| 70% – 90%      | Healthy       |
| < 70%          | Underutilized |

---

## Project Workflow

### Step 1: Data Processing

The script:

* Loads operational data from Excel
* Cleans and transforms data
* Creates business metrics
* Creates occupancy classifications
* Creates weekday/weekend indicators

---

### Step 2: KPI Generation

The project calculates:

* Total students
* Total capacity
* Overall occupancy rate
* Parent satisfaction score
* Cancellation rate
* Late arrival rate
* Overflow class count
* Near-full class count
* Underutilized class count

---

### Step 3: Operational Analysis

The project generates summaries for:

#### Location Performance

Analyze:

* Student volume
* Capacity utilization
* Parent satisfaction

#### Location + Time Slot Performance

Identify:

* High-demand schedules
* Underutilized schedules
* Capacity bottlenecks

#### Time Slot Analysis

Determine:

* Peak demand periods
* Low-demand periods

#### Weekend vs Weekday Analysis

Compare utilization patterns across different operating periods.

---

### Step 4: AI Operational Insights

Using Google Gemini, the project automatically generates:

* Executive Summary
* Business Insights
* Operational Risks
* Manager Recommendations
* Scheduling Recommendations

The AI analysis is grounded using operational KPI tables and business rules.

---

### Step 5: AI Sentiment Analysis

Parent reviews are analyzed using Google Gemini.

The AI identifies:

* Overall sentiment
* Positive themes
* Negative themes
* Reasons families stay
* Reasons families leave
* Actionable recommendations

This helps management understand customer experience beyond numerical ratings.

---

## Output

The project automatically generates:

### AI Reports

* AI_Operations_Summary
* AI_Sentiment_Analysis

### Operational Tables

* Location_Summary
* Location_Time_Summary
* Time_Summary
* Weekend_Summary
* Overflow_Events
* Near_Full_Events
* Underutilized_Events

Final Output:

goldfish_ai_business_report.xlsx

---

## Technologies Used

### Data Analysis

* Python
* Pandas

### Generative AI

* Google Gemini API
* Gemini 2.5 Flash

### Excel Automation

* OpenPyXL

### Reporting

* Automated Excel Report Generation

---

## Skills Demonstrated

This project demonstrates:

### Business Analytics

* KPI Development
* Capacity Planning
* Operations Analysis
* Utilization Monitoring

### Data Analytics

* Data Cleaning
* Feature Engineering
* Aggregation Analysis
* Reporting Automation

### AI Applications

* Prompt Engineering
* Generative AI Reporting
* Sentiment Analysis
* Business Insight Generation

### Technical Skills

* Python
* Pandas
* OpenPyXL
* Gemini API Integration

---

## Future Improvements

Potential enhancements include:

* Seasonal demand analysis
* Holiday impact analysis
* School calendar integration
* Student retention tracking
* Forecasting future enrollment
* Instructor utilization analysis
* Power BI dashboard integration
* Automated email reporting
* Fine-tuned sentiment classification model

---

## Author

Haolin (Holly) Chen

M.S. Data Analytics
Northeastern University

Focus Areas:

* Data Analytics
* Business Intelligence
* Machine Learning
* Generative AI Applications
