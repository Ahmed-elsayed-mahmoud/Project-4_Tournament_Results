# Tournament Results

## Project Overview

You will develop a database schema to store the game matches between players. 
You will then write a Python module to rank the players and pair them up in matches in a tournament.


## Why This Project?
Modern data-driven applications require developers that know how to store data and interact programmatically with that data. 
In this project, you’ll design a database based off of a provided specification and use case and then write code that makes use of that data.

## What Will I Learn?
You will learn how to architect and develop a database containing fully normalized data within multiple tables. 
You’ll then learn how to modify this data and query it to meet the demands of a variety of use cases.


## Project Files 

There are three main files:

**tournament.py**  

Contains the implementation for the Swiss tournament  

**tournament.sql**  

Contains the SQL queries to create the database, tables and views   

**tournament_test.py**  

Contains the test cases for tournament.py  

## Prerequisites 

The latest vagrant build for the Udacity tournament project.

## Instructions

1. Start Vagrant
  1. Open Terminal or cmd and browse to the vagrant folder
  2. Type `vagrant up`
2. SSH in to the vagrant VM
  1. In the same terminal type `vagrant ssh`
3. Change to the correct folder
  1. Type `cd /vagrant/tournament`
4. Open PSQL and run the tournament.sql 
  1. type `psql`
  2. copy the contents of tournament.sql and paste in to the terminal window
  3. type `\q` to quit out of PSQL 
5. Run the tests
  1. In the terminal type `python tournament_test.py`

## Expected Outcome

Success!  All tests pass!  
vagrant@vagrant-ubuntu-trusty-32:/vagrant/tournament$ python tournament_test.py  
1. Old matches can be deleted.  
2. Player records can be deleted.  
3. After deleting, countPlayers() returns zero.  
4. After registering a player, countPlayers() returns 1.  
5. Players can be registered and deleted.  
6. Newly registered players appear in the standings with no matches.  
7. After a match, players have updated standings.  
8. After one match, players with one win are paired.  
Success!  All tests pass!  

## Extra Credit

If the top two players have the same won match count, and have won more than 0 games, then 
the standings is ordered by total number of wins by games played in descending order.

## License

The project is licensed under the [Apache License](LICENSE).