# iot-assignment-2
an api that interfaces with a sensor and responds acordingly 


There are a few prerequisites if you wish to use all the functionality

For the server you must have a version of python between 3.6 to 3.9

For the sensor you must have the Osoyoo kit configured the way it is configured in the provided image (sensor) and connected to an MQTT server


SETUP--------------------------------------------------------------------------------------------------------------------------
In order to turn on the server you must unzip the iot assignment 2 zip
Open terminal in the iot assignment 2 directory
type in this command to open the environment:  env\Scripts\activate
change directory to fall_detection
use this command to run the server: python manage.py runserver
the server is now running on local host port 8000
you can use the admin page to check the database on http://localhost:8000/admin/
user: admin password: password
to see the json use this url http://localhost:8000/patients/

in order to use the sensor plug it into a computer
edit the code to add your ssid and password and change the mqtt server address to the one you wish to use
open a mqtt client on your computer and connect it to the server
you can subscribe to out123 to read the tilt and you can publish to in123

TESTS--------------------------------------------------------------------------------------------------------------------------
Tests results can be viewed in the Tests directory

1. run the server in terminal successfully
2. View the home page of the server
3. Add patients to the database via the admin
4. View the get request directly from the server
5. make a get request externally
6. Obtain readings from the sensor

EXPLANATION--------------------------------------------------------------------------------------------------------------------
The Sensor can be set up on a local network to make a put request and change the user information to tell the server the user has fallen
The server has an api setup for get requests
both elements work seperatly
in order for the 2 components to work together the sensor only needs to make a put request and the server has to have a put command available


TABLE OF CONTENTS--------------------------------------------------------------------------------------------------------------
The code for the sensor is in the fallSensor folder located in the root directory
The enc folder is in the root directory, it has the configuration of the needed environment for the api
The fall_detection folder holds the server and supporting files
Fall_detection project holds the fall_detection configuration, the application called home page, the database, and the manage file
Fall_detection is configured with the proper url paths and supporting libraries
The database holds the user information
The manage.py is used in the command line to run the server among other crucial commands
The Homepage application holds the admin page, the homepage, the database model,the serializer class that makes the RESTful api, and the necessary views


