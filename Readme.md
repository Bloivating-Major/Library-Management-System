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

- now what i will do is in add book function i will add the book in our json db
- after that we have to save our data in json db
- so we will create a function save_data() and then call it in add_book() function
- save data function will be class based and only accessible within the class
    - we will use @classmethod decorator over here
    - we will use indent=4 to make our json file readable
    - we will use default=str to handle any kind of data type
    - and use json.dump() to write data in json file

- now we will create list books function
- it will list all the books in our json db
- we will use f-strings to format our output
- we will use slicing to truncate the title and author if they are too long
- we will use :12, :25, :15, :5, :>3 to format our output