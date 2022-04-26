![enter image description here](https://i.ibb.co/8gy8Np9/dark-back3.jpg)

# Car Rental System
* [Project](#project)
-- [Team](#team)
-- [Idea](#idea)
--[Division of Labor](#division-of-labor)
* [Features](#features)
-- [Dynamic System](#dynamic-system)
-- [Efficient Queries](#efficient-queries)
-- [Error Handling](#error-handling)
-- [Remote Database](#remote-database)
* [User](#user)
-- [Search page](#search-page)
-- [Results page](#results-page)
-- [User Reservations page](#user-reservations-page)
* [Admin](#admin)
-- [Admin login page](#admin-login-page)
-- [Users page](#users-page)
-- [Offices page](#offices-page)
-- [Cars page](#cars-page)
-- [Reservations page](#reservations-page)
-- [Payments page](#payments-page)
* [ERD](#erd)
* [Thanks](#thanks)

# Project
## Team
* Andrew Wahid - 6578
* Ahmed Abdelrahman - 6543
* Karim Sameh - 6169
* Kyrollos Magdy - 6167

## Idea
Our website is well thought out and shows that we were determined to make the project as realistic as possible to a real life car rental system.
Our system supports multiple offices where offices can be located in different countries, cities.
Users in our system are only allowed if they're older than 18 years and have a valid national ID.
The system has a very strong search mechanism for free cars between dates.
And user can also filter the cars based on their needs (price, model, manufacturer, etc..)

We know how hard it is to see all your previous data as a user or as an admin, that's why we put a lot of thought into how to represent these data in an organized and pleasing to they eye manner.
We used tables with searches and sorting features so data seeking is a breeze.
Admins are humans 😅, that's why they also can make their own reservations and manage at the same time.

And most importantly our system proved to work on a remote mysql database and even the website is live at a server!

## Division of labor
We started by a meeting call in which we discussed the problems, and how to approach solutions, we agreed on a certain program/database architecture.

We then split work between us, each of us had a part that he will dedicate himself to perfect it.

We first used whatsapp as a way of communicating and updating/informing each other of the progress each one of us made.

Then we discovered because of the large quantity of files each of us made, Whatsapp became very crowded because of these files, so we decided to move our work to Github.

Github helped us share our work with each other with ease and develop much faster because we all always had the newest updates of one another.

# Features
Our project is packed with features, let's discuss them below.
## Dynamic System
Our program is dynamic meaning that:
- User session is saved and heavily secured through server-side encryption/validation
- All our functions work asynchronously so nothing happens before it should happens
- Lack of asynchronous behaviour would not appear on a localhose website, that's why we tested our asynchronous system in a live server and made sure everything is perfected
- Not only the website was live on a server, but also the MySQL database was on a live server and connected to it remotely!

## Efficient Queries
The implemented system utilizes search queries efficiently so that in most cases, all the information required by the page can be retrieved from the database using a single search query. This makes the system run much more smoothly which can help improve client satisfaction. The database schema is also designed to help retrieve important information easily. 
The following are some samples of queries used:

- The admin can retrieve statistics about each car, including how many times it was reserved, the total prospective income from the car, total payments made for the car, total number of days it was reserved for, all using a single query.
- The customer can search for a car that is free in a specific time frame, is present in their desired location, and is not marked out of service by the admin, using advanced search filters that consider manufacturer, model year, and price. This is retrieved using 2 queries only.
- The admin can retrieve information about users including their personal information, total number of reservations made, total amount owed to the company, and total amount paid using 2 queries.
- The complete history of the car including the status at any given time can be retrieved by the admin using a single query.


## Error Handling
We wanted to be very neat and organized for generated erros, so we gave each error an error code which describes it.
Some of these codes (definetley not all):
* Error 420
-- Account with this email already exists
* Error 421
-- Account with this national id already exists
* Error 422
-- Wrong email and/or password
* Error 440
-- A car already exist with the same plate
* Error 430
-- No office with such ID
* Error 450
-- An office exists in the same exact country and city and location
## Remote Database
Our system is currently live and up and running all in cloud
MySQL is hosted on the cloud and a custom PHPMyAdmin is also set up just for it.
The website itself the HTML along with the PHP are also live and running.
Also the website has a SSL Certificate for extra security 😉

# User

### Login/Register Page

![](https://i.ibb.co/qRz0rq2/u-login-0.png)

![](https://i.ibb.co/tqW2H8b/u-login-1.png)

### Search Page

![](https://i.ibb.co/pwYyK1s/u-search-0.png)

![](https://i.ibb.co/9h7hjNN/u-search-1.png)

### Results Page

![](https://i.ibb.co/d2VsX8B/a-result-0.png)

![](https://i.ibb.co/GC3ZVYJ/a-result-1.png)

### User reservations page

![](https://i.ibb.co/yRtfQhf/u-reservations-0.png)

![](https://i.ibb.co/X5Krptq/u-reservations-1.png)

![](https://i.ibb.co/h95cDT9/u-reservations-2.png)


# Admin

### Admin login page

![](https://i.ibb.co/5Ty0TTH/image.png)

### Users page

![](https://i.ibb.co/W5jnJkb/a-users-0.png)

### Offices page

![](https://i.ibb.co/YN4BSwb/a-office-0.png)

![](https://i.ibb.co/crY6QVC/a-office-1.png)

### Cars page

![](https://i.ibb.co/znHz350/a-cars-0.png)

![](https://i.ibb.co/Sy3wTQS/a-cars-1.png)

![](https://i.ibb.co/F6jQNqd/a-cars-2.png)

![](https://i.ibb.co/ZxMPJrL/a-cars-3.png)


### Reservations page

![](https://i.ibb.co/8ctdr47/a-reservations-0.png)

![](https://i.ibb.co/h9Mxv83/a-reservations-1.png)

### Payments page

![](https://i.ibb.co/Bg591xK/a-users-1.png)

# ERD

`available in high quality in Car Rental ER Diagram.pdf`

![](https://i.ibb.co/98gj8cm/image.png)


# Thanks
Thanks for this wonderful semester.
We really learnt a lot, and we hope that you find your hard-work reflected in our project!

* Andrew Wahid - 6578
* Ahmed Abdelrahman - 6543
* Karim Sameh - 6169
* Kyrollos Magdy - 6167
