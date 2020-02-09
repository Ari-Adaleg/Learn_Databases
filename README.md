# Into_to_sql

Login to psql



1. Find all the robots from Star Wars.
select * from robots where source = 'Star Wars';

2. Find the robot with an "anxious" personality.
select * from robots where source = 'Star Wars' and personality = 'anxious';

3. Find all recipes that are nut free.
-----

4. Count the number of recipes that are gluten free but not vegetarian.
-----

5. Find the animal with the most legs.
select name from animals where number_of_legs = (select max(number_of_legs) from animals);

6. Find the board game that takes the least amount of time to play.
select name from board_games where mins_to_play = (select min(mins_to_play) from board_games);
     
7. Find the recipe that takes the most time to prepare.
-----

8. Find all the robots whose name starts with the letter M.
select name from robots where name like 'M%';
     
9. Count the number of board games that can be played by 8 people.
select count('star') from board_games where max_players = 8;

10. Find all animals that are swimming and egg-laying.
select name from animals where swimming = true and egg_laying = true;
      
11. Find all animals that are swimming and egg-laying but not flying.
select name from animals where swimming = true and egg_laying = true and flying = false;
     
12. Find the board game that supports the largest number of people.
select name from board_games where max_players = (select max(max_players) from board_games);
     
