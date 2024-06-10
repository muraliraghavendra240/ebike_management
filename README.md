# ebike management

 The application is built with Streamlit and connected to a MySQL database.

## Objectives

1. Create a CRUD Application using Streamlit
2. Connect the application to MySQL Server

## Setup

To run this project, you need to have:

1. [XAMPP](https://www.apachefriends.org/download_success.html) installed to run MySQL database.
2. Turn on Apache and MySQL in XAMPP.

### Steps

1. **Start Apache and MySQL**:
   - Open XAMPP Control Panel.
   - Start both Apache and MySQL.

2. **Access phpMyAdmin**:
   - In your browser, visit [phpMyAdmin](http://localhost/phpmyadmin/).

3. **Clone the Repository**:
   - Clone this repository into your local machine.
     ```bash
     git clone https://github.com/muraliraghavendra240/Train_Tracker.git
     cd Train_Tracker
     ```

4. **Setup the Database**:
   - Navigate to the `app.py` file location.
   - Uncomment the following lines in `app.py` to create the database:
     ```python
     import mysql.connector
     mydb = mysql.connector.connect(
         host="localhost",
         user="root",
         password=""
     )
     c = mydb.cursor()
     c.execute("CREATE DATABASE train")
     ```
   - Run the file using the command:
     ```bash
     streamlit run app.py
     ```

5. 
   - After running `app.py`, comment out the lines you uncommented in the previous step, save the file, and refresh the page rendered in the browse
       - #import mysql.connector
       #mydb = mysql.connector.connect(
      #host="localhost",
      #user="root",
      #password=""
      #)
      #c = mydb.cursor()
    #c.execute("CREATE DATABASE ebike")


##
