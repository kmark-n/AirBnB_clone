While building this AirBnB application which is a copy of the AirBnB website, all the concepts won't be implemented all at once.
It shall be built step by step.

First we start with the console:
#Here we'll create a data model
#Manage(create, update, destroy, etc) objects via a console/ command interpreter
#Store and persist objects to a file(JSON file)

The first piece is to manipulate a powerful storage system. This storage engine will give us an abstraction between "My object" and "How they are stored and persisted". This means that from my console code(the command interpreter itself) and from the front-end and RestAPI that i'll build later, I won't have to pay attention to how my objects are stored.

The abstraction will also allow the changing of storage easily without updating all of our codebase.
The console will be a tool to validate this storage engine.
![image](https://github.com/kmark-n/AirBnB_clone/assets/117804697/4725971d-3fa3-4710-8b1d-cfe18dc2e163)

a.) models directory - contains all classes used for the entire project. In a OOP(object oriented programming) project, a class called 'model' is the representation of an object/instance.

b.) tests directory - will contain all unit tests.

c.) console.py file - This file is the entry point of our command line interpreter.

d.) models/base_model.py file - This is the base class of all our models. It contains common elements:

attributes: "id", "created_at", and "updated_at"
methods: "save()" and "to_json()"

e.) models/engine directory - this contains all storage classes(using the same prototype.).
For the moment i only have: file_storage.py
