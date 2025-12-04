# Product Requirements Document: Maternal Health Monitoring App MVP (v1.0)

**Context:** This MVP (v1.0) is focused on first-trimester anxiety reduction and establishing a daily user habit. It strictly adheres to the constraints defined in the MVP Vision document (mvp_vision.md).

**Primary Goal:** Enable the Anxious New Mother to securely track key self-reported health metrics and receive curated, week-specific reassurance/information to reduce anxiety during the first 12 weeks of pregnancy.

## I. Out-of-Scope Items (Based on MVP Vision Constraints)

To ensure a focused release, the following features are explicitly Out-of-Scope for V1.0:

* Content for the Second and Third Trimesters (Content limited to Weeks 1-12).
* Integration with any external devices (e.g., smart scales, glucose monitors, wearables).
* Any direct secure sharing mechanism or portal for Physicians/Clinics.
* Multi-platform deployment (Focusing on a single, determined platform).
* Social features or community forums.
* Advanced analytics or predictive modeling (e.g., calculating risk factors).

## II. MVP Core Features & User Stories

The following 15 features are necessary to meet the Success Criteria for retention and daily check-in.

### A. Onboarding & Account Management

| Feature | User Story |
|---------|------------|
| **1. Secure User Registration** | As a new user, I want to create a private account with email and password so that my sensitive health data is secure and persisted across sessions. |
| **2. Pregnancy Profile Setup** | As a new user, I want to input my estimated due date (EDD) or the start date of my Last Menstrual Period (LMP) so that the app can automatically calculate my current week and personalize content. |
| **3. Profile Editing** | As a user, I want to easily edit my EDD or initial weight so that my calculations remain accurate if my doctor updates my information. |

**Acceptance Criteria (ACs):**

* **AC 1.1:** The user must be successfully authenticated before any health data is saved or retrieved.
* **AC 2.1:** The system must accurately calculate and display the user's current week of pregnancy based on the input date (EDD or LMP start date).
* **AC 3.1:** Changing the EDD automatically recalculates all future content and timeline progress.

### B. Daily Check-in & Logging

| Feature | User Story |
|---------|------------|
| **4. Daily Check-in Reminder** | As a user, I want to receive a daily, customizable notification so that I am prompted to log my health metrics and establish a habit. |
| **5. Symptom Logging** | As a user, I want to select and rate the severity of common first-trimester symptoms (e.g., Nausea, Fatigue, Headaches) so that I can track patterns and easily report changes to my physician. |
| **6. Weight Logging** | As a user, I want a quick way to log my current weight in either KG or LBS so that I can monitor weight gain/loss trends. |
| **7. Mood & Emotion Tracking** | As a user, I want to select my general mood (e.g., Happy, Anxious, Tired, Irritable) so that I can understand how my pregnancy affects my mental state. |
| **8. Free-Form Journaling** | As a user, I want an optional text field to quickly note any specific thoughts or events so that I have a private, detailed record outside of structured metrics. |

**Acceptance Criteria (ACs):**

* **AC 5.1:** Symptom selection must be presented via easily tappable, friendly icons (not clinical text fields).
* **AC 6.1:** The weight logging interface clearly displays the last recorded weight upon entry.
* **AC 7.1:** Mood logging uses a simple scale or predefined, non-judgmental terms.
* **AC 8.1:** The daily check-in workflow concludes with a positive, encouraging confirmation message (e.g., "Log Complete! You're doing great.") to reinforce the behavior.

### C. Information Delivery & Reassurance

| Feature | User Story |
|---------|------------|
| **9. Week-Specific Content Access** | As a user, I want to view content specifically curated for my current week of pregnancy (e.g., "Week 8: What to expect") so that the information is relevant and reduces my uncertainty. |
| **10. Symptom Normalcy Guide** | As a user, when I log a symptom (e.g., nausea), I want to see a short note indicating if it is "normal for this week" or "when to call your doctor" so that my immediate anxiety is addressed. |
| **11. Home Screen Status** | As a user, I want to see my current week and a countdown to my EDD on the main dashboard so that I feel connected to my journey. |

**Acceptance Criteria (ACs):**

* **AC 9.1:** Users cannot access content for weeks beyond their current calculated week (preventing information overload).
* **AC 10.1:** The reassurance text must be brief, supportive, and displayed immediately after the symptom is logged or viewed.
* **AC 11.1:** The home screen displays the user's name and the calculated Week X + Y days.

### D. Progress Visualization & Reporting

| Feature | User Story |
|---------|------------|
| **12. Weight Trend Chart** | As a user, I want to view an interactive line chart of my weight history so that I can monitor my progress visually over time. |
| **13. Mood History Visualization** | As a user, I want to see a simple calendar or heat map visualization of my daily logged moods so that I can identify emotional patterns quickly. |
| **14. PDF Data Summary Export** | As a user, I want to generate a printable PDF summary of my logged symptoms, weight, and mood history so that I can easily share my trends with my physician during appointments. |
| **15. User Satisfaction Feedback** | As a user, I want to be prompted once a month to provide a simple rating and optional feedback (NPS) so that the product team can measure user satisfaction and improve the app. |

**Acceptance Criteria (ACs):**

* **AC 12.1:** The Weight Trend Chart displays data points for at least the last 7 and 30 days.
* **AC 13.1:** Moods are color-coded in the history visualization for quick scanning.
* **AC 14.1:** The generated PDF must be clearly formatted, titled, and include the user's name and EDD.
* **AC 15.1:** The NPS prompt is non-intrusive and can be easily dismissed or deferred.