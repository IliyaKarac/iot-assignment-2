# iot-assignment-2
an api that interfaces with a sensor and responds acordingly 


There are a few pre-requisits if you wish to use all the functionality

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


