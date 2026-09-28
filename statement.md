## 📌Problem Statement

Most of the time, managing a chronic condition or tracking temporary illnesses relies on human memory, which is subjective and prone to errors.
Patients are frequently unable to answer quite specific, data-driven questions requested by healthcare providers,
such as "How long after taking the medication did the pain subside?" or "What specific triggers precede your migraines?"
Without accurate and longitudinal data, treatment plans are less effective, and often critically important correlations between lifestyle habits,
medication intake, and symptom severity are missed.

## 📌Scope of the Project
This project aims at developing an intelligent health tracking application that goes beyond static logging towards analytical insights.

### Functional Scope:
The system will enable the user to record unique health events (medications and symptoms) with automatic timestamping.
Then, it will store this information for the duration of the session and display it back through a live, easy-to-read journal view.

### Technical Scope:
Solution is implemented in Python using Tkinter for the graphical interface, replacing the original command-line menu with clickable
forms, dropdowns, and list selection. This makes the application friendlier for non-technical users while keeping the same underlying
data model (a list of tracked items). Future versions can extend this further with persistent storage (e.g. SQLite or CSV) and
data analysis using libraries such as Pandas and Scikit-learn.

### Analytical Scope:
The project lays the groundwork for basic concepts of Machine Learning, such as regression or correlation analysis, to identify relations
between inputs (medication) and outputs (symptom relief), planned as a future enhancement once persistent data collection is in place.

* Limitations include the fact that the system provides informational logging alone and does not provide medical diagnoses. Complex NLP
  and statistical analysis are considered future enhancements.

## 📌Target Users
* **Chronic Patients:** People with chronic ailments such as migraine, arthritis, and allergic reactions that require monitoring of triggers and alleviation.
* **Caregivers:** Family members monitoring health data for elderly or pediatric patients, ensuring adherence to medications.
* **Self-Quantifiers:** Health-conscious individuals trying to evaluate the effectiveness of new medication regimens or lifestyle changes.

## 📌High-level Features
* **Smart Event Logging:** A form-based interface that allows efficiently recording medication dosages and symptom occurrences, reducing friction to a minimum.
* **Automatic Temporal Tracking:** Accurate timestamping of each entry to show when a medication was taken or a symptom last occurred.
* **Live Journal View:** A single, always-up-to-date list showing every tracked item, its total occurrence count, and its most recent event.
* **User-Friendly GUI:** Dropdown category selection and click-to-log interactions remove the need to remember menu numbers or item indexes.
* **Foundation for Analytics:** The consistent, structured data model (name, category, count, last-logged time) is designed to support future
  pattern-recognition features without needing a redesign.
