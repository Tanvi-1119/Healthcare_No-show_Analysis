# Healthcare No-Show Analysis

## Project Overview
This project analyzes patient appointment no-shows at a Brazilian healthcare facility. 
The goal is to identify patterns and factors that contribute to patients missing their 
scheduled appointments using real-world data containing over 110,000 records.

## Tools Used
- **Python (Google Colab)** — Data cleaning and preparation
- **SQL (SQLite)** — Data analysis and querying
- **Power BI** — Data visualization and dashboard 

## Dataset
- **Source:** Kaggle — Medical Appointment No-Shows
- **Original records:** 110,527
- **Records after cleaning:** 71,959
- **Columns:** Patient ID, Gender, Age, Neighbourhood, Scholarship, Hipertension, 
Diabetes, Alcoholism, SMS Received, No-Show

## Data Cleaning (Python)
- Standardized all column names to lowercase
- Removed 1 row with invalid age value (-1)
- Converted date columns to proper datetime format
- Removed records where appointment date was before the scheduled date

## SQL Analysis — Key Findings

### Overall No-Show Rate
- 28.52% of patients missed their appointments

### No-Show by Gender
- Female patients: 28.45% no-show rate
- Male patients: 28.67% no-show rate
- Gender has almost no impact on no-show rate

### No-Show by Age Group
- Young Adults (18-35): 34.36% — highest no-show rate
- Children (0-17): 32.27%
- Middle Age (36-60): 26.71%
- Seniors (60+): 20.46% — most reliable group

### Impact of SMS Reminders
- Patients without SMS: 29.44% no-show rate
- Patients with SMS: 27.57% no-show rate
- SMS reminders reduce no-shows but only by 1.87%

### Top Neighbourhoods with Highest No-Show Rates
- Gurigica: 38.37%
- Jesus de Nazareth: 37.49%
- Itararé: 36.50%

### No-Show by Chronic Condition
- Patients with only alcoholism: 38.75% — highest no-show rate
- Patients with only hypertension: 22.85% — most reliable

### No-Show by Waiting Days
- Same day appointments: 21.35% no-show rate
- More than 30 days wait: 33.02% no-show rate
- The longer the wait, the higher the chance of a no-show

## Key Recommendations
1. Send stronger reminders to patients waiting more than 30 days
2. Focus outreach efforts on young adults aged 18-35
3. Target high no-show neighbourhoods like Gurigica and Jesus de Nazareth
4. Consider follow-up calls for patients with alcoholism

## Project Status
- [x] Data Cleaning — Python
- [x] Data Analysis — SQL
- [ ] Dashboard — Power BI (coming soon)
