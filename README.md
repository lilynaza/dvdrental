# Introduction
I recentenly completed SQL courses on data camp from intoduction level to the advanced level. For a personal project, I decided to analyze the database for a DVD rental company. Let’s take a look at a case study detailing my process and output.

# I began by taking a look at the dataset. 
The data set have 15 tables.
Below are the different tables and a brief description of them.

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
2. Which movies have been rented so far.
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

