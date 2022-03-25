# -SQL-for-Data-Science-Quiz-and-Practice-Answer

                   ###################--------------- WEEK - 1 ----------------------##########################################  
1.
Question 1
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement. 

Run query: Retrieve all the data from the tracks table. Who is the composer for track 18 ??

Select *
From Tracks limit 18;

Ans : AC/DC is the composer for track 18

2.
Question 2
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Retrieve all data from the artists table. Look at the list of artists, how many artists are you familiar with (there is no wrong answer here)?

Select count(*)
From Artists;

Ans :  275

3.
Question 3
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Retrieve all data from the invoices table. What is the billing address for customer 31?

Select *
From Invoices;


Ans : 194A Chain Lake Drive, Halifax, NS, CANADA B3S 1C5

4.
Question 4
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Return the playlist id, and name from the playlists table. How many playlists are there? Which would you classify is your favorite from this list?

Select Playlistid,
Name
From Playlists;

Ans : 18


5.
Question 5
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Return the Customer Id, Invoice Date, and Billing City from the Invoices table. What city is associated with Customer ID number 42? What was the invoice date for the customer in Santiago?

Select CustomerId,
InvoiceDate, 
BillingCity 
From Invoices;

Ans : Bordeaux 2009-04-04 

6.
Question 6
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Return the First Name, Last Name, Email, and Phone, from the Customers table. What is the telephone number for Jennifer Peterson?

Select FirstName, 
LastName, 
Email, 
Phone
From Customers;

Ans : Jennifer Peterson's phone number is: +1 (604) 688-2255


7.
Question 7
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Return the Track Id, Genre Id, Composer, Unit Price from the Tracks table. How much do these tracks cost?

Select TrackId, 
GenreId, 
Composer, 
sum(UnitPrice) 
From Tracks;

Ans : 3680.97

8.
Question 8
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Select all the columns from the Playlist Track table and limit the results to 10 records. How might this information be used?

Select *
From Playlist_track 
Limit 10;

Ans : Top 10 result used

9.
Question 9
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Select all the columns from the Media Types table and limit the results to 50 records. What happened when you ran this query? Were you able to get all 50 records?

Select *
From Media_types
Limit 50;

Ans : No

10.
Question 10
To prepare for the graded coding quiz, you will be asked to execute a query, read the results, and select the correct answer you found in the results. This question is for you to practice executing queries. I have provided you the script for this query, a simple select statement. Think of this as a sandbox for you to practice. As you practice executing queries, take time to read the results in order to prepare for the quiz and get comfortable writing a basic select statement.

Run Query: Select all the columns from the Albums table and limit the results to 5 records. How many columns are in the albums table? 

Select *
From Albums;

Ans : 25





