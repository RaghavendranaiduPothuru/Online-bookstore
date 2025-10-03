# Online-bookstore
The Online Bookstore is a mini web-based application that allows users to browse books, search by title or author, add items to a cart, and simulate checkout. It includes an admin module to manage inventory. Built with Java, MySQL, HTML, and CSS, it demonstrates full-stack development skills
About
A user-friendly Online Bookstore project in which users can log in or register, view the available books, select books along with their quantity, and buy them. Users can also get payment receipts after successful payment. The project can also be used by the administrator, who can add new books, remove books, increase and decrease the quantity of books, change the price of the books as well as maintain the selling history of books.
<img width="1360" height="626" alt="image" src="https://github.com/user-attachments/assets/c6affb1c-6ce1-4958-a044-0355990d5b39" />



onlinebookstore

This Website is built for following purpose:-

For Selling books online.
Maintaining books selling history.
Adding and managing books.
User Friendly.
For Implementation of Http Servlets in Java.
This is a Mini-project developed using Java, Jdbc, And Servlets.
Admin Have Following Access for this online store site:-

Add New Books.
View Books Available.
Remove Books.
Increase Books Amount.
Users Have Following Access for this online store site:-

Create New Account or Register.
Login.
View Available Books.
Select Books to Buy.
Select Books Quantity.
Buy Books.
Get Payment Receipt.
Technologies used:-
Front-End Development:
HTML
CSS
Javascript
BootStrap
Back-End Development:
Java [JDK 8+]
JDBC
Servlet
Database:
MySql
 ===============Software And Tools Required ================
: Git [https://www.youtube.com/watch?v=gv7VPQ4LZ7g]
: Java JDK 8+ [https://www.youtube.com/watch?v=O9PWH9SeTTE]
: Eclipse EE (Enterprise Edition) [https://www.youtube.com/watch?v=8aDsEV7txXE]
: Apache Maven [https://www.youtube.com/watch?v=jd2zx3dLjuw]
: Tomcat v8.0+ [https://youtu.be/mLFPodZO8Iw?t=903]
: MySQL Server [https://www.youtube.com/watch?v=Ydh5jYA6Frs]
: MySQL Workbench (optional) [https://www.youtube.com/watch?v=t79oCeTXHwg]
================= Dummy Database Initialization =================
STEP 1: Open MySQL Command Prompt or MySQL Workbench

STEP 2: Login to the administrator user as : mysql -u <username> -p (Enter Password if asked)

STEP 3: Copy paste the following MySql Commands-

create database if not exists onlinebookstore;

use onlinebookstore;

create table if not exists books(barcode varchar(100) primary key, name varchar(100), author varchar(100), price int, quantity int);

create table if not exists users(username varchar(100) primary key,password varchar(100), firstname varchar(100),
    lastname varchar(100),address text, phone varchar(100),mailid varchar(100),usertype int);


commit;

========== Importing and Running The Project Through Eclipse EE ==========

Step 0: Open Eclipse Enterprise Edition. [Install, if not already installed.]

Step 1: Click On File > Import > Git > Projects From Git > Clone Uri > Paste The Repository Url as: [https://github.com/RaghavendranaiduPothuru/onlinebookstore.git> ](https://github.com/RaghavendranaiduPothuru/Online-bookstore/tree/main)Select master Branch > Next > Next > Finish.

Step 2. a: Go inside src/main/resources > application.properties and update the value of database details as per your usage, like db.driver, db.host, db.username and db.password according to your installed mysql/postgresql admin user credentials.

Step 2.b: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 2.c: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 3: [Only If Tomcat Server is not configured in Eclipse] : Right Click On Project > Run As > Run On Server > Select Tomcat V8.0 > (Select Tomcat V8.0 Installation Location If Asked) Next > Add onlinebookstore > Finish.

Step 4: In The Server Tab > Double Click On Tomcat Server > Ports > Change The Port Number For Http/1.1 To 8083 > Close And Save.

Step 5: Right Click On Project > Run As > Run On Server > Select Tomcat v8.0 > Next > Add All> Done.

Step 6: Check Running The Site At http://localhost:8083/onlinebookstore/

Step 7: Default Username And Password For Admin Is "Admin" And "Admin"

Step 8: The default Username And Password For User Is "shashi" And "shashi"

FAQ
Question:1 Unable to Connect to Database?

Answer: Please check you have installed the mysql correctly and have updated the correct db details in application.properties file. Also you can try doing maven clean install and force update the project and restart.
