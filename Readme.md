# Library Management System Notes

## Steps

### Project Initialization

- created a main.py file
- created a library.json file to store data
- we will be covering almost each and every concept that we have used till now to create this project
- now we will start with some imports
    - json
    - random
    - string
    - pathlib Path
    - datetime

- now we will create first basic ui of options and actions that we have to perform
- then we will create a class and connect it with out database which is in json format

- Now we will create our class Library and then start writing out features
    - add book
    - we will have here options like
        - enter title
        - enter author
        - enter copies
    - then we will create a dictionary and then add it in our json db
    - our json will have things like:
        - id
        - title
        - author
        - total copies
        - available copies
        - added on => will use data and time over here

- now to generate a random id we will create a function within class itself
- so what we have to do is generate 2 types of ids 
    - book id
    - member id
- keeping that in mind we will be writing our generate id function
- create an object and call it use and test out the add book function

- now what we will be doing is creating our database as json file 
- Let's start by creating our database location
- Format of our data will be in 2 parts
    - books
    - members
- data = {
    "books": [],
    "members": []
}

- now we will create logic to load data from existing json file
- if file is not present then create it
- if file is present then load data from it
- if file is empty then create it
