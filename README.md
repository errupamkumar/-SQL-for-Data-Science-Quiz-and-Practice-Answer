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


          @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@    Module 1 Coding Questions  and Answers   @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@  
          
          
          
          
1.
Question 1
For all of the questions in this quiz, we are using the Chinook database. All of the interactive code blocks have been setup to retrieve data only from this database.

Retrieve all the records from the Employees table.


select * from Employees ; 

+------------+----------+-----------+---------------------+-----------+---------------------+---------------------+-----------------------------+------------+-------+---------+------------+-------------------+-------------------+--------------------------+
| EmployeeId | LastName | FirstName | Title               | ReportsTo | BirthDate           | HireDate            | Address                     | City       | State | Country | PostalCode | Phone             | Fax               | Email                    |
+------------+----------+-----------+---------------------+-----------+---------------------+---------------------+-----------------------------+------------+-------+---------+------------+-------------------+-------------------+--------------------------+
|          1 | Adams    | Andrew    | General Manager     |      None | 1962-02-18 00:00:00 | 2002-08-14 00:00:00 | 11120 Jasper Ave NW         | Edmonton   | AB    | Canada  | T5K 2N1    | +1 (780) 428-9482 | +1 (780) 428-3457 | andrew@chinookcorp.com   |
|          2 | Edwards  | Nancy     | Sales Manager       |         1 | 1958-12-08 00:00:00 | 2002-05-01 00:00:00 | 825 8 Ave SW                | Calgary    | AB    | Canada  | T2P 2T3    | +1 (403) 262-3443 | +1 (403) 262-3322 | nancy@chinookcorp.com    |
|          3 | Peacock  | Jane      | Sales Support Agent |         2 | 1973-08-29 00:00:00 | 2002-04-01 00:00:00 | 1111 6 Ave SW               | Calgary    | AB    | Canada  | T2P 5M5    | +1 (403) 262-3443 | +1 (403) 262-6712 | jane@chinookcorp.com     |
|          4 | Park     | Margaret  | Sales Support Agent |         2 | 1947-09-19 00:00:00 | 2003-05-03 00:00:00 | 683 10 Street SW            | Calgary    | AB    | Canada  | T2P 5G3    | +1 (403) 263-4423 | +1 (403) 263-4289 | margaret@chinookcorp.com |
|          5 | Johnson  | Steve     | Sales Support Agent |         2 | 1965-03-03 00:00:00 | 2003-10-17 00:00:00 | 7727B 41 Ave                | Calgary    | AB    | Canada  | T3B 1Y7    | 1 (780) 836-9987  | 1 (780) 836-9543  | steve@chinookcorp.com    |
|          6 | Mitchell | Michael   | IT Manager          |         1 | 1973-07-01 00:00:00 | 2003-10-17 00:00:00 | 5827 Bowness Road NW        | Calgary    | AB    | Canada  | T3B 0C5    | +1 (403) 246-9887 | +1 (403) 246-9899 | michael@chinookcorp.com  |
|          7 | King     | Robert    | IT Staff            |         6 | 1970-05-29 00:00:00 | 2004-01-02 00:00:00 | 590 Columbia Boulevard West | Lethbridge | AB    | Canada  | T1K 5N8    | +1 (403) 456-9986 | +1 (403) 456-8485 | robert@chinookcorp.com   |
|          8 | Callahan | Laura     | IT Staff            |         6 | 1968-01-09 00:00:00 | 2004-03-04 00:00:00 | 923 7 ST NW                 | Lethbridge | AB    | Canada  | T1H 1Y8    | +1 (403) 467-3351 | +1 (403) 467-8772 | laura@chinookcorp.com    |
+------------+----------+-----------+---------------------+-----------+---------------------+---------------------+-----------------------------+------------+-------+---------+------------+-------------------+-------------------+--------------------------+

What is Robert King's mailing address? Note: You will have to scroll to the right in order to see it.


Ans : 590 Columbia Boulevard West, Lethbridge, AB, CANADA T1K 5N8 

2.
Question 2
Retrieve the FirstName, LastName, Birthdate, Address, City, and State from the Employees table.

SELECT FirstName, LastName, Birthdate, Address, City,State from Employees ;

+-----------+----------+---------------------+-----------------------------+------------+-------+
| FirstName | LastName | BirthDate           | Address                     | City       | State |
+-----------+----------+---------------------+-----------------------------+------------+-------+
| Andrew    | Adams    | 1962-02-18 00:00:00 | 11120 Jasper Ave NW         | Edmonton   | AB    |
| Nancy     | Edwards  | 1958-12-08 00:00:00 | 825 8 Ave SW                | Calgary    | AB    |
| Jane      | Peacock  | 1973-08-29 00:00:00 | 1111 6 Ave SW               | Calgary    | AB    |
| Margaret  | Park     | 1947-09-19 00:00:00 | 683 10 Street SW            | Calgary    | AB    |
| Steve     | Johnson  | 1965-03-03 00:00:00 | 7727B 41 Ave                | Calgary    | AB    |
| Michael   | Mitchell | 1973-07-01 00:00:00 | 5827 Bowness Road NW        | Calgary    | AB    |
| Robert    | King     | 1970-05-29 00:00:00 | 590 Columbia Boulevard West | Lethbridge | AB    |
| Laura     | Callahan | 1968-01-09 00:00:00 | 923 7 ST NW                 | Lethbridge | AB    |
+-----------+----------+---------------------+-----------------------------+------------+-------+

 Which of the employees listed below has a birthdate of 3-3-1965?
 
Ans : Steve


3.
Question 3
Retrieve all the columns from the Tracks table, but only return 20 rows.

SELECT * FROM Tracks limit 20 ; 

+---------+-----------------------------------------+---------+-------------+---------+------------------------------------------------------------------------+--------------+----------+-----------+
| TrackId | Name                                    | AlbumId | MediaTypeId | GenreId | Composer                                                               | Milliseconds |    Bytes | UnitPrice |
+---------+-----------------------------------------+---------+-------------+---------+------------------------------------------------------------------------+--------------+----------+-----------+
|       1 | For Those About To Rock (We Salute You) |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       343719 | 11170334 |      0.99 |
|       2 | Balls to the Wall                       |       2 |           2 |       1 | None                                                                   |       342562 |  5510424 |      0.99 |
|       3 | Fast As a Shark                         |       3 |           2 |       1 | F. Baltes, S. Kaufman, U. Dirkscneider & W. Hoffman                    |       230619 |  3990994 |      0.99 |
|       4 | Restless and Wild                       |       3 |           2 |       1 | F. Baltes, R.A. Smith-Diesel, S. Kaufman, U. Dirkscneider & W. Hoffman |       252051 |  4331779 |      0.99 |
|       5 | Princess of the Dawn                    |       3 |           2 |       1 | Deaffy & R.A. Smith-Diesel                                             |       375418 |  6290521 |      0.99 |
|       6 | Put The Finger On You                   |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       205662 |  6713451 |      0.99 |
|       7 | Let's Get It Up                         |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       233926 |  7636561 |      0.99 |
|       8 | Inject The Venom                        |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       210834 |  6852860 |      0.99 |
|       9 | Snowballed                              |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       203102 |  6599424 |      0.99 |
|      10 | Evil Walks                              |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       263497 |  8611245 |      0.99 |
|      11 | C.O.D.                                  |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       199836 |  6566314 |      0.99 |
|      12 | Breaking The Rules                      |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       263288 |  8596840 |      0.99 |
|      13 | Night Of The Long Knives                |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       205688 |  6706347 |      0.99 |
|      14 | Spellbound                              |       1 |           1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |       270863 |  8817038 |      0.99 |
|      15 | Go Down                                 |       4 |           1 |       1 | AC/DC                                                                  |       331180 | 10847611 |      0.99 |
|      16 | Dog Eat Dog                             |       4 |           1 |       1 | AC/DC                                                                  |       215196 |  7032162 |      0.99 |
|      17 | Let There Be Rock                       |       4 |           1 |       1 | AC/DC                                                                  |       366654 | 12021261 |      0.99 |
|      18 | Bad Boy Boogie                          |       4 |           1 |       1 | AC/DC                                                                  |       267728 |  8776140 |      0.99 |
|      19 | Problem Child                           |       4 |           1 |       1 | AC/DC                                                                  |       325041 | 10617116 |      0.99 |
|      20 | Overdose                                |       4 |           1 |       1 | AC/DC                                                                  |       369319 | 12066294 |      0.99 |
+---------+-----------------------------------------+---------+-------------+---------+------------------------------------------------------------------------+--------------+----------+-----------+

What is the runtime in milliseconds for the 5th track, entitled "Princess of the Dawn"? Note: You will need to scroll to the right to see it, and you may want to copy and paste the number to ensure it is entered correctly.

ANs :  375418




