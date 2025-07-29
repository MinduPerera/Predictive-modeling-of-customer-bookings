# 🛫 Holiday Booking Prediction using Random Forest

This project aims to predict whether a customer will complete a holiday booking using machine learning. With a strong imbalance between booked and non-booked customers, this solution leverages a **Random Forest Classifier** with class balancing and model interpretation techniques to optimize for actionable insights.

---

## 📊 Problem Statement

Airlines and travel companies need to engage customers **before** they arrive at the airport. The goal of this project is to:

- Predict if a customer will **complete a booking** (`1`) or **not** (`0`)
- Understand what **factors influence booking behavior**
- Use this to guide **marketing strategy and proactive engagement**

---

## 🧠 Model Overview

- **Model Used**: Random Forest Classifier (`sklearn`)
- **Imbalance Handling**: `class_weight='balanced'`
- **Preprocessing**:
  - Imputation for missing values
  - One-hot encoding for categorical features
  - Standard scaling for numerical features
- **Evaluation**:
  - Confusion matrix
  - Classification report
  - ROC AUC Score
- **Interpretation**: Feature importance visualization
  <img width="990" height="590" alt="image" src="https://github.com/user-attachments/assets/8e97cc38-ffdd-48b3-b507-0b0840d9cd1c" />


---

## 🧪 Dataset

- Input: Customer activity and booking behavior
- Target: `booking complete` (1 = booked, 0 = not booked)
- The dataset was imbalanced (~85% not booked, ~15% booked)

- `num_passengers` = number of passengers travelling
- `sales_channel` = sales channel booking was made on
- `trip_type` = trip Type (Round Trip, One Way, Circle Trip)
- `purchase_lead` = number of days between travel date and booking date
- `length_of_stay` = number of days spent at destination
- `flight_hour` = hour of flight departure
- `flight_day` = day of week of flight departure
- `route` = origin -> destination flight route
- `booking_origin` = country from where booking was made
- `wants_extra_baggage` = if the customer wanted extra baggage in the booking
- `wants_preferred_seat` = if the customer wanted a preferred seat in the booking
- `wants_in_flight_meals` = if the customer wanted in-flight meals in the booking
- `flight_duration` = total duration of flight (in hours)
- `booking_complete` = flag indicating if the customer completed the booking

---

## 🚀 Getting Started

### 1. Clone this repo
```bash
git clone https://github.com/your-username/holiday-booking-prediction.git
cd holiday-booking-prediction


