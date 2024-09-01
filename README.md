150141-Patrick Kamatu

# Airline Booking System

This project is a Django-based airline booking system that provides a RESTful API for managing flights and passengers. The system is built using Django Rest Framework (DRF) and follows best practices for RESTful API design.


# Features

- Manage flights: create, view, and delete flights.
- Manage passengers: create, view, and delete passengers.
- Each passenger is associated with a specific flight.


## Setup Instructions

# 1. cloning

```bash
git clone https://github.com/your-username/airline-booking-system.git
cd airline-booking-system

# 2.Create a virtual environment
virtualenv venv

# 3.Activate the virtual environment
venv\Scripts\activate

#4. installing framework
pip install django djangorestframework

#5.Making migrations
python manage.py makemigrations
python manage.py migrate

python manage.py createsuperuser




