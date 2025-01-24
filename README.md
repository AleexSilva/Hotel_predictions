# Hotel Booking Prediction

This project focuses on predicting hotel reservations using data analysis and machine learning techniques. The dataset contains historical booking data, and the goal is to develop a predictive model to determine whether a reservation will be honored or canceled. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and model training.

![](./header.png)

## Table of Contents
- [Data Dictionary](#DataDictionary)
- [Installation](#installation)
- [Usage](#usage)
- [Required Libraries](#required-libraries)
- [Files and Dataset](#files-and-dataset)
- [Data](#Data)


### Data Dictionary

- `hotel`: Hotel where the reservation was made.
- `is_canceled`: Indicates whether the reservation was canceled or not.
- `lead_time`: Number of days between the reservation's entry into the PMS and the arrival date.
- `arrival_date_year`: Year of the arrival date.
- `arrival_date_month`: Month of the arrival date, with 12 categories: "January" to "December."
- `arrival_date_week_number`: Week number of the arrival date.
- `arrival_date_day_of_month`: Day of the month of the arrival date.
- `stays_in_weekend_nights`: Number of weekend nights (Saturday or Sunday) the guest stayed or booked at the hotel.
- `stays_in_week_nights`: Number of weekday nights (Monday to Friday) the guest stayed or booked at the hotel.
- `adults`: Number of adults.
- `children`: Number of children.
- `babies`: Number of babies.
- `meal`: Type of meal booked. Categorical value.
- `country`: Country of origin. Categories are represented according to ISO 3155–3:2013.
- `market_segment`: Market segment designation.
- `distribution_channel`: Reservation distribution channel.
- `is_repeated_guest`: Value indicating whether the reservation name belonged to a returning guest (1) or not (0).
- `previous_cancellations`: Number of prior reservations canceled by the customer before the current booking.
- `previous_bookings_not_canceled`: Number of prior reservations not canceled by the customer before the current booking.
- `reserved_room_type`: Code for the reserved room type. The code is used instead of the designation for anonymity reasons.
- `assigned_room_type`: Code for the assigned room type. Sometimes, the assigned room type differs from the reserved room type due to hotel operational reasons (e.g., overbooking) or customer requests. The code is used instead of the designation for anonymity reasons.
- `booking_changes`: Number of changes/modifications made to the reservation from its entry into the PMS until check-in or cancellation.
- `deposit_type`: Indicates whether the customer made a deposit to secure the booking.
- `agent`: Travel agency ID that made the reservation.
- `company`: ID of the company/entity that made the reservation or is responsible for payment.
- `days_in_waiting_list`: Number of days the reservation was on the waiting list before being confirmed to the customer.
- `customer_type`: Type of booking.
- `adr`: Average daily rate.
- `required_car_parking_spaces`: Number of parking spaces required by the customer.
- `total_of_special_requests`: Number of special requests made by the customer (e.g., double bed or high floor).
- `reservation_status`: Last status of the reservation.
- `reservation_status_date`: Date when the last status was set.
- `name`: Customer name.
- `email`: Customer email.
- `phone`: Customer phone number.
- `credit_card`: Last four digits of the customer's credit card.

The data provided by the company is in the file `hotel_bookings_training.csv`.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/hotel-booking-prediction.git
   cd hotel-booking-prediction
## Usage
To run the prediction model, execute the main script:


For exploratory data analysis, open the Jupyter notebooks inside the notebooks/ directory


## Required Libraries
Ensure you have the following Python libraries installed:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- jupyter


## Files and Dataset
 - `data/`: Contains the dataset used for training and testing the model.
- `notebooks/`: Jupyter notebooks with data exploration, visualization, and modeling.
- `src/`: Scripts for data preprocessing and machine learning model implementation.
- `models/`: Saved trained models.
- `reports/`: Generated reports and visualizations from the analysis.

## Data

*Fake Hotel* has two branches: one located in the state capital, "City Hotel," and another in a coastal community, "Resort Hotel."

The data they provided is in CSV format, where each row represents a reservation with the following attributes:

```python
import pandas as pd

data = pd.read_csv('hotel_bookings_training.csv')
```