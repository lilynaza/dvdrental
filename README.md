# Introduction
I recentenly completed SQL courses on data camp from intoduction level to the advanced level. For a personal project, I decided to analyze the database for a DVD rental company. Let’s take a look at a case study detailing my process and output.

# Problem statement

I went to conduct exploratory data analysis using sql to know the renting attitude of the customers who rent movies from the company

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

![3](https://user-images.githubusercontent.com/78624637/178354380-2a6a6a6c-c0c5-4ba2-892e-2c350a23eb16.PNG)

* Insight

All customer have rented a movie.
4. Display each movie and the number of times it got rented.

![4](https://user-images.githubusercontent.com/78624637/178350687-2b5a8311-f803-4556-bd4c-787197bf199d.PNG)

 * Insight
 
 ![4r](https://user-images.githubusercontent.com/78624637/178350939-c4a86894-c1b9-4117-b875-91ef5ff199e3.PNG)
 
5. Show the first name, last name and the number of movie each actor acted in.

![5](https://user-images.githubusercontent.com/78624637/178351171-68b4a092-17a8-4462-a6e5-d9c45f06ddfd.PNG)

* Insight

![5r](https://user-images.githubusercontent.com/78624637/178351460-4237f14e-04e5-40b7-88c3-8290be9680c3.PNG)


6. Display the names of actors that acted in more than 20 movies.

![6](https://user-images.githubusercontent.com/78624637/178351934-db7ba275-9030-4a24-a636-a296b5582474.PNG)


* Insight

![6r](https://user-images.githubusercontent.com/78624637/178351702-5ce4dbef-6786-45de-9d2d-41f92f1b95b0.PNG)


7. For all the movies rated "PG" show me the movies and the number of times it go rented.

![7](https://user-images.githubusercontent.com/78624637/178351956-c65c151f-e9b7-4871-abfe-911df53ec336.PNG)

* Insight

![7r](https://user-images.githubusercontent.com/78624637/178351990-1fff9665-8cac-4fa6-893e-814d80dbcf3b.PNG)

8. Display the movies offered in store 1 and not offered in store 2.

![8](https://user-images.githubusercontent.com/78624637/178352028-1034a355-e6bd-41db-a5dd-64bdb68bd921.PNG)

* Insight

![8r](https://user-images.githubusercontent.com/78624637/178352055-ff4a6c54-cb03-4da3-acea-6c93df5a9926.PNG)

9. Display the movies offered for rent in any of the two store 1 and 2

![9](https://user-images.githubusercontent.com/78624637/178352080-71f428a0-af42-4106-b21b-7f510eed6197.PNG)

* Insight

![9r](https://user-images.githubusercontent.com/78624637/178352101-90a62eb8-a69c-44b3-900a-a1e37e3d36b2.PNG)

10. Display the title of the movies offered at both store at same time.

![10](https://user-images.githubusercontent.com/78624637/178352126-1d7d061c-dfbe-46e4-83d8-bcc513739b90.PNG)

* Insight


![10r](https://user-images.githubusercontent.com/78624637/178352174-08168fe7-3e52-4fef-80df-db1791acad3d.PNG)


11. Display the most rented movies in the store with store_id 1


![11](https://user-images.githubusercontent.com/78624637/178352724-7573ba90-21f3-4a5f-99bd-e4d8c005861a.PNG)
 
 * Insight 
 
 ![11r](https://user-images.githubusercontent.com/78624637/178352765-2243b0c7-5fc3-460f-87dd-ea3c84fa553c.PNG)


12. How many movies are not offered for rent in the stores yet. There are two stores only 1 and 2

![12](https://user-images.githubusercontent.com/78624637/178352788-fc6c06c1-411b-496a-af09-a2338d123170.PNG)


* Insight


![12r](https://user-images.githubusercontent.com/78624637/178352842-d8d7b357-3548-4473-aa9b-c429fe56a902.PNG)

13. Show the number of rented movies under each rating.

![13](https://user-images.githubusercontent.com/78624637/178352880-94f8ae45-6171-4856-8f2a-8086b679c3b4.PNG)


* Insight


![13r](https://user-images.githubusercontent.com/78624637/178352903-83b7f27d-23c1-4587-a4ee-7bdd39bea884.PNG)

PG-13 movie were the most rented movie.

14. Show the profit of each of the stores 1 and 2.


![14](https://user-images.githubusercontent.com/78624637/178352935-0bed37a3-2e37-44ae-bb85-53af81b12912.PNG)

* Insight


![14r](https://user-images.githubusercontent.com/78624637/178352964-2eeae562-a110-41b8-8165-e1ff470bd63d.PNG)


15. What is the name of the customer who made the highest total payment.

![15](https://user-images.githubusercontent.com/78624637/178352993-42767559-807b-42a0-930a-d716434a9927.PNG)

* Insight


![15r](https://user-images.githubusercontent.com/78624637/178353029-f2eab501-5d8e-4176-a638-14d1cf55654a.PNG)

16. Which movies have not been rented so far.


![16](https://user-images.githubusercontent.com/78624637/178353061-c476f874-f325-443f-897e-435a0b1b962c.PNG)

* Insight


![16r](https://user-images.githubusercontent.com/78624637/178353077-ebbecc4b-0db0-465c-a1c0-9d4d85e1a89f.PNG)

# Conclusion

In this project, I analyzed data from a DVD rental company. To find insights about the customers and their preference

