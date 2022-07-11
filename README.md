# Introduction
I recentenly completed SQL courses on data camp from intoduction level to the advanced level. For a personal project, I decided to analyze the database for a DVD rental company. Let’s take a look at a case study detailing my process and output.

# I began by taking a look at the dataset. 
The data set have 15 tables.
Below are the different tables and a brief description of them.

# Schema
![Rental_Schema](https://user-images.githubusercontent.com/78624637/178349512-e5d50905-9b77-4535-819b-a89277ac2a1a.PNG)

* actor — contains actors data including first name and last name.
* film — contains films data such as title, release year, length, rating, etc.
* film_actor — contains the relationships between films and actors.
* category — contains film’s categories data.
* film_category — containing the relationships between films and categories.
* store — contains the store data including manager staff and address.
* inventory — stores inventory data.
* rental — stores rental data.
* payment — stores customer’s payments.
* staff — stores staff data.
* customer — stores customer’s data.
* address — stores address data for staff and customers
* city — stores the city names.
* country — stores the country names.

I analyzed this database using PostgreSQL.

# Objective & Goals
I shall be answering the following question.
1. What is the movie(s) that was rented the most.

![1](https://user-images.githubusercontent.com/78624637/178349823-babcad61-cf31-41d1-9e66-4bf0fca5ee26.PNG)

* Insight

![1r](https://user-images.githubusercontent.com/78624637/178349997-02658143-cfc3-423e-9d5f-853cab8d8f72.PNG)
2. Which movies have been rented so far.

![2](https://user-images.githubusercontent.com/78624637/178350215-bb433c90-59cf-454a-89c4-3ba1534118d7.PNG)

* Insight

![2r](https://user-images.githubusercontent.com/78624637/178350442-4d7e0c45-bb7c-4cdc-b833-85945c82c0c3.PNG)

3. Which customers have not rented any movies so far.
4. Display each movie and the number of times it got rented.
5. Show the first name, last name and the number of movie each actor acted in.
6. Display the names of actors that acted in more than 20 movies.
7. For all the movies rated "PG" show me the movies and the number of times it go rented.
8. Display the movies offered in store 1 and not offered in store 2.
9. Display the movies offered for rent in any of the two store 1 and 2
10. Display the title of the movies offered at both store at same time.
11. Display the most rented movies in the store with store_id 1
12. How many movies are not offered for rent in the stores yet. There are two stores only 1 and 2
13. Show the number of rented movies under each rating.
14. Show the profit of each of the stores 1 and 2.
15. What is the name of the customer who made the highest total payment.
16. Which movies have not been rented so far.

