Database Project 1

Sam is a movie store owner. He currently manages his tock manually.
Sam owns a computer in his store for the sole purpose to play music and watch movies.
Sam is faced with a problem in his business. Clients are not sure of what movie title to buy or rent but would rather ask for a genre, year of release or the most trending movie etc.. You guessed right! Sam is having hard time satisfying his customers.

As a database designer/developer would you assist Sam do the following: 

1. Create a database and name it STORE
 mysql> CREATE DATABASE STORE;
2. Create a table inside the database and name it MOVIES.
mysql> use STORE;
mysql> CREATE TABLE MOVIES (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, MOVIE_TITLE VARCHAR(20), MOVIE_RELEASED_YEAR VARCHAR(20), MOVIE_LENGTH VARCHAR(20)), MOVIE_LANGUAGE VARCHAR(20)); 

3. The table must contain the following columns :
            a. Movie ID
            b. Movie title 
            c. Movie released year 
            d. Movie length (time in minute)
            e. Movie language           
4. Create a script to add the following data inside the table  the table:



mysql> INSERT INTO MOVIES VALUES (NULL,"Vertigo","1958","128","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"The Innocents","1961","100","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"Lawrence of Arabia","1962","216","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"The Deer Hunter","1978","183","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"Amadeus","1984","160","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"Blade Runner","1982","160","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"Eyes Wide Shut","1999","159","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"The Usual Suspects","1995","106","English");
mysql> INSERT INTO MOVIES VALUES (NULL,"Chinatown","1974","130","English");


5. create a script to view all movies
mysql> Select * from MOVIES;

6. Sam would like to update the release year of a movie titled 'Eyes Wide Shut to 1999’. create a script that will update the movie.
mysql> update MOVIES
    -> set MOVIE_RELEASED_YEAR="Not yet set"
    -> where id=7;

7. A movie titled 'Vertigo' is no more in store. Create a script that will remove the movie details from the table.
mysql> delete from MOVIES
    -> where id=1;
 

