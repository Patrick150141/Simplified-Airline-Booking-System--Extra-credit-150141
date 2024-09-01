150141-Patrick Kamatu
 

#Airline Booking System
This project is a Django-based airline booking system that provides a RESTful API for managing flights and passengers. The system is built using Django Rest Framework (DRF) and follows best practices for RESTful API design.

#Features
 Manage flights: create, view, and delete flights.
 Manage passengers: create, view, and delete passengers.
 Each passenger is associated with a specific flight.


 Setup Instruction

 #1.Start djangoproject
 django-admin startproject bookingsite
 cd bookingsite
 
 #startapp
 python manage.py startapp booking


#2.Create a virtual environment
virtualenv venv

#3.Activate the virtual environment
venv\Scripts\activate

#4. installing framework
pip install django djangorestframework

#5.Making migrations
python manage.py makemigrations
python manage.py migrate

python manage.py createsuperuser

#Models
The application includes two main models: Flight and Passenger.

#Flight Model

The Flight model represents a flight in the system
flight_number: A unique identifier for the flight.
departure: The date and time when the flight departs.
arrival: The date and time when the flight arrives.
origin: The origin airport.
destination: The destination airport.
capacity: The total number of seats available on the flight

#Passenger Model
The Passenger model represents a passenger in the system.
first_name: The first name of the passenger.
last_name: The last name of the passenger.
email: A unique email address for the passenger.
phone_number: The contact number for the passenger.
flight: A foreign key relationship to the Flight model, indicating the flight the passenger is associated with.

#Flight Serializer
The FlightSerializer handles serialization and deserialization for the Flight model.

#Passenger Serializer
The PassengerSerializer handles serialization and deserialization for the Passenger model.

#Flight ViewSet
The FlightViewSet provides a full set of views for the Flight model, including listing, retrieving, creating, and deleting flights.

#Passenger ViewSet
The PassengerViewSet provides a full set of views for the Passenger model, including listing, retrieving, creating, and deleting passengers.









