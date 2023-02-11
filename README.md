AirBnB clone project

--- ## Description HBnB is a web app with a full development of back-end and front-end API integrating also SQL storage This project is the part 1 of 4 in which the back-end console is created and deployed. This is an educational purposes clone from [AirBnB](https://www.airbnb.com/)
Classes
This projects uses the following classes:

BaseModel	FileStorage	User	Amenity	City	Place	Review	State
Public instance attributes	id
created_at
updated_at		Inherits BaseModel	Inherits BaseModel	Inherits BaseModel	Inherits BaseModel	Inherits BaseModel	Inherits BaseModel
Public instance methods	save
to_dict	all
new
save
reload						
Public class attributes			email
password
first_name
last_name	name	_id
name	name	city_id
user_id
name
description
_rooms
_bathrooms
max_guest
price
latitude
longitude
amenity_id	place_id
user_id
text
Private class attributes		file_path
objects						
Storage
The presented classes are stored in FileStorage class file. When the console is initialized, the console redirects an instance of FileStorage named storage. #Storage object is loaded or reloaded from any class instances stored in the JSON file file.json. Class instances are created, updated, or deleted and storage object registers changes intofile.json.

Console
The console is a CLI that allows the use of data as backend tool. It can be used to handle all classes predefined previously called into storage object.

How to Test:
Unittests for the CLI HBnB project are defined in the tests folder. To run the entire test suite simultaneously, execute the following command:

$ python3 unittest -m discover tests
Also, you can specify a single test file to run at a time:

$ python3 unittest -m tests/test_console.py
Authors:
Isaac Olutimayin <ZoeDioDrey>
