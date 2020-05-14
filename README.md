# sample_stats
File for stat illustrations 

CREATE TABLE players ( 
id INTEGER PRIMARY KEY, 
name TEXT, 
position TEXT, 
hometown TEXT); 

CREATE TABLE team (
player_id INTEGER PRIMARY KEY, 
team_name TEXT, 
wins INTEGER, 
loses INTEGER); 

CREATE TABLE statistics (
team_id INTEGER PRIMARY KEY, 
player_id INTEGER UNIQUE, 
ppg REAL, 
apg REAL, 
rpg REAL); 

INSERT INTO players VALUES (1, 'Lebron James', 'SF/PF', 'Akron, Ohio'); 
INSERT INTO players VALUES (2, 'Kevin Durant', 'SF/PF', 'Largo, Maryland'); 
INSERT INTO players VALUES (3, 'Michael Beasley', 'PF', 'Washington DC'); 
INSERT INTO players VALUES (4, 'Ty Lawson', 'PG', 'Forestville, Maryland'); 
INSERT INTO players VALUES (5, 'Sam Young', 'SF', 'Fort Washington, Maryland'); 
INSERT INTO players VALUES (6, 'Michael Jordan', 'SG', 'Charlotte, North Carolina'); 
INSERT INTO players VALUES (7, 'Allen Iverson', 'PG/SG', 'Newport News, Virginia'); 
INSERT INTO players VALUES (8, 'Rod Strickland', 'PG', 'St. Louis, Missouri'); 
INSERT INTO players VALUES (9, 'Rasheed Wallace', 'PF', 'Detroit, Michigan'); 
INSERT INTO players VALUES (10, 'Antoine Smitty', 'PG', 'Fort Washington, Maryland'); 

INSERT INTO team VALUES (1, 'Los Angeles Lakers', 78, 20);
INSERT INTO team VALUES (2, 'Brooklyn Nets', 75, 24); 
INSERT INTO team VALUES (3, 'Miami Heat', 34, 89); 
INSERT INTO team VALUES (4, 'Denver Nuggets', 43, 73); 
INSERT INTO team VALUES (5, 'Friendly Patriots', 50, 72); 
INSERT INTO team VALUES (6, 'Chicago Bulls', 123, 4); 
INSERT INTO team VALUES (7, 'Philadelphia 76ers', 100, 23); 
INSERT INTO team VALUES (8, 'Washington Bullets', 55, 32); 
INSERT INTO team VALUES (9, 'Portland TrailBlazers', 70, 43); 
INSERT INTO team VALUES (10, 'Breath Of Life Bulldogs', 99, 33); 

INSERT INTO statistics VALUES (1, 1, 29.5, 11.5, 10.5); 
INSERT INTO statistics VALUES (2, 2, 33.4, 5.2, 7.1); 
INSERT INTO statistics VALUES (3, 3, 8.7, 3.2, 4.8); 
INSERT INTO statistics VALUES (4, 4, 10.2, 10, 2.1); 
INSERT INTO statistics VALUES (5, 5, 14.6, 6.2, 7.2); 
INSERT INTO statistics VALUES (6, 6, 35.6, 8.3, 8.2); 
INSERT INTO statistics VALUES (7, 7, 31.3, 5.5, 4.3); 
INSERT INTO statistics VALUES (8, 8, 20.3, 10.2, 4.3); 
INSERT INTO statistics VALUES (9, 9, 23.5, 5.3, 13.3);
INSERT INTO statistics VALUES (10, 10, 15.3, 8.3, 5.3); 
