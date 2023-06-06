While building this AirBnB application which is a copy of the AirBnB website, all the concepts won't be implemented all at once.
It shall be built step by step.

First we start with the console:
#Here we'll create a data model
#Manage(create, update, destroy, etc) objects via a console/ command interpreter
#Store and persist objects to a file(JSON file)

The first piece is to manipulate a powerful storage system. This storage engine will give us an abstraction between "My object" and "How they are stored and persisted". This means that from my console code(the command interpreter itself) and from the front-end and RestAPI that i'll build later, I won't have to pay attention to how my objects are stored.

The abstraction will also allow the changing of storage easily without updating all of our codebase.
The console will be a tool to validate this storage engine.

