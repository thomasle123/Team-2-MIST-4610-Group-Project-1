# Group-2-Project-1
 
## **Team Name**
Sp24_61608_Group 2 

## **Team Members:**
1. Dylan Artis (https://github.com/DJA706)
2. Dana Baus (https://github.com/Dananasplitt)
3. Molly Butkovich (https://github.com/mollybutkovich)
4. Connor Coniglio (me)
5. Thomas Le (https://github.com/thomasle123)
6. Alex Quinlan (https://github.com/AlexQuinlan12)

## **Problem Description:**
In our interactions with our client (Atlanta Braves Management), we have decided to make a comprehensive system to manage the teams operations using a relational database model in SQL. In this model, we created many entities that break down the structure of the Atlanta Braves organization. As seen in our model, we have highlighted many key sectors of our client's organizations that require the most focus. For the Atlanta Braves’ organization to be successful and optimize its efficiency and profitability, the management team needs to use these highlighted components to make the right decisions. 

By using our relational database on your baseball operations, our client will be able to see a 360-degree view of the team’s current operations and use that to assess your current strengths and weaknesses. From this assessment, the Braves’ management team will be able to derive key insights and metrics on aspects of their business that they otherwise might have been unaware of. Utilizing this, we are sure that they will make key changes that will thrust the company in the right direction.

Our model and analysis were created to ensure proper integration of all aspects of team management. Due to the dynamic nature of the MLB and the Atlanta Braves position in it, this breakdown of our client’s structure will highlight the organization’s operational needs and allow the company to gain a competitive advantage amongst other teams.

## **Our Data Model:**
Our data model is designed to capture and store valuable information that the Braves’ Manager may need to operate and successfully run a winning organization. The managers want us to tailor the data to focus on the players and what they need to be successful. The Player’s Entity represents the players on the Braves, what position they play, and how they are doing career-wise. Players on the team play many different games throughout the season and each different game includes multiple players on the roster. This is shown by our many-to-many relationship between Players and Games. Our associative entity is GameStats which shows how each player performed during each game and requires a player ID and Game ID to show that player's performance for that particular game. 


Within the Games entity are attributes concerning the game date, location, and opponent score. An opposing team can play many different games versus the Atlanta Braves which is represented by the one-to-many relationship. Additionally, the different games can take place in any season indicating that there are many games in one unique season. This is shown by our one-to-many relationship between Seasons and Games. Furthermore, every player on the Braves either improves or declines in play each season which is shown by our associative table, Scouting Report is a result of the many-to-many relationship between Seasons and Players.


For players to perform at their best, they must practice their craft. Managers would want to keep track of who is practicing and who is not to see who is committed to winning. In order to help track practices, we have created an entity to track practices. The practice entity tracks when, where, and how long to practice. It has a one-to-many relationship with facilities because multiple practices can be held in the same faculty, but a practice can only occur in one faculty at a time. Also, they want to track what players attend what practice to see who is putting in the most work. We made a many-to-many relationship between practices and players because a player can attend multiple practices and practice can include many different players. The associative entity for this relationship is PlayerSchedule and it uses a composite key to track which players participated in a certain practice. Coaches are also involved in practice as they are the ones training the players. Each coach has a specific expertise/role where they are the lead coach of a practice.  We use a one-to-many relationship between coaches and practices because a coach hosts many practices, but only one coach can lead the practice.


A big part of player and staff management is managing their contracts. We made an entity for contracts to store data about the types of contracts it is, how much it is worth, and the duration of the contract. Contracts are a one-to-one relationship with both players and coaches because each player and coach has one specific contract assigned to them. They do not share a contract, nor is a player or coach under multiple contracts at one time.


Returning to the center focus of our data model, the Players, each player has their own equipment as demonstrated by the Equipment entity. Within the Equipment entity attributes are related to the type of equipment the player possesses as well as its condition. Each player can have many pieces of equipment but it only belongs to one player which is shown through the one-to-many relationship between the Players and Equipment entity. 


Additionally, it is natural in high-level sports for players to get injured. The Atlanta Braves prepare for this by having multiple team doctors on staff who are specialized in their field and have many years of experience. Those doctors are shown on the TeamDoctor entity. There is a many-to-many relationship established between the Players and the TeamDoctor entity because the players can experience many injuries and the team doctors can treat many different injuries. The associate entity created is the Injuries entity which describes the injury type and cleared date. It is very important for the Braves’ Manager to be able to keep up with the well-being of their players to ensure a successful season! 

![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/bd288337-f0d9-4fad-aada-b4fcc5ab9587)

## **Data Dictionary:**
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/a24170ae-f1de-43df-81f3-e4d2fb2b336a)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/dbb83533-eff6-4a1a-a0d3-6be9fb00ebf2)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/34b0a113-fc98-4aef-a641-7ecf8d0b840f)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/67f863ce-a0b7-44f1-ba72-eb2626c21965)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/9c2fc2b2-ab81-4639-af3e-7cd19398e400)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/8bb477d6-491c-4d61-81e7-e34983e73c7b)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/5ff033fb-3d68-4ecd-990d-5905c3b1d281)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/208fe698-4e23-4cbd-913b-9d354e3c2cab)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/4dfa8519-31d9-489e-9eb5-dd0eac72161f)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/3b4bbfcf-0e22-48ec-8ce7-262569788db5)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/4ca5c3b3-210d-4b4c-9ff5-1bf3d27a67dd)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/12165e9d-7815-48f4-a1a4-c9ce37fca596)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/52253923-ce33-4771-b26c-fffa3f27d2b9)
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/c6498037-adf4-4fd6-966c-81b86e93deb7)

## **Queries:**

![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/c9d27f2b-1a37-4bf3-b611-2efdee3d12b3)

#1. List the first name and last name of the players who were not injured last season (assuming no one was injured this season). 
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/ce7ae985-5456-4583-a697-db187ae5a4b3)

Description: This query would be used by coaches to determine which players need to be watched more closely to prevent  recurring injuries. This query returns player names who had an injury in the previous season. Our client could use this information to monitor rehabilitation health for injury-prone players and make informed decisions on player usage rate (i.e. - don't play injury-prone players too much every game and give them more time for rehabilitation to preserve them throughout the season).

#2. List the names of all coaches, their roles, and the date of the practices they attend. Order the practice dates chronologically. 
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/9e1d0324-b643-4cf8-8962-5971590db0da)

Description: This query will result in showing which practices coaches are involved in and what their role is. This query would be used to develop coach schedules and potentially weed out errors. This query is especially useful for team managers or owners who want to have available coaches for press conferences or meetings outside of practice. As a result of our client using this, they can maximize coach efficiency and make sure players are getting optimal instructions from all the coaches they need it from.

#3.List out player name, contract salary and endDate for all players whose strength on their scouting report is pitching
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/af988b13-41f7-481d-88d9-3d354618e683)

Description: The query will print player names, their salary, and the end date of their current contract for players with the scouting strength pitching. This query is useful to coaches and team owners who want to evaluate player’s performance and compare their initial scouting strengths to current performance. They can also use this information when making new contracts and potentially give raises to players with high-performance metrics.

#4. Count the number of equipment items where the type is a bat and the item is broken. 
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/c49e6c59-df90-49a3-8429-6f2d2d7d1d89)

Description: The purpose of this query is to provide a count of how many bats are broken. This query is useful to coaches so they know how many bats need to be replaced and the amount of players who need new equipment. They can use the query to determine how many new bats need to be ordered. By doing this, our client will be able to ensure players have their needed equipment and it will allow for maximum practice and player improvement efficiency.

#5. List the gameID, score of the opponent with the opponent name, and the score of the Braves for every game the braves won in the 2023 season.
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/0a30b85a-44c6-4f86-a226-4c1e8400e359)

Description: Query 5 is useful to players and coaches, informing them of the games where they performed well. They can use the information from the query to determine factors that contributed to their success and try to replicate these conditions in future games. It does this by filtering and aggregating the team's scores vs the opponent's scores to highlight their success.

#6. List players names, their types of injuries, and the doctor that treats them. Do this for players who have scored more than one run in a game.
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/4aa75b3f-f69f-4bb8-bc01-29e211841306)

Description: This query outputs players who have scored more than one run in a game; returning their name, type of injuries, and doctor name. It groups the results by player name, injury type, and doctor name. The point of using this query would be to track how players are performing and weather or not injuries might be affecting player statistics. By tracking these metrics, our client can make informed decisions on whether to keep underperforming players on the roster if they are injured and seeing if certain player slumps are a result of injury. Additionally, if there are players that are injured while also not putting up numbers (runs), management could decide it would be worth it to give them time to recover as they are currently not vital to team success.

#7. List the total score, the amount of homeruns included in the total score, and the location for all games played in the 2023 season
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/82db9444-b458-426e-961a-015576b7693e)

Description: The purpose of this query is to count up the total Braves scores across all games in a season while also counting up the sum of home runs made and giving the locations of where the games were played. This query could be used as a tool indicating performance evaluation for the team across the season. Based on this, our client can see multiple trends such as player development, what locations the team excels at, etc.

#8. List out the location and game score of all games whos average score is greater than the average score of all games played in the 2023 season
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/dfe947ca-48aa-47c2-8b64-047b948e47a8)

Description: This query sees which games our clients team played exceptionally well in. From the results of this query, our client will be able to see times of success and use that information to improve upon strategic decisions. For example, if this query shows the Braves excel in games where they have one practice and one rehab pre-game, management could adjust their training schedule to try and replicate the results. It could also be used to see if we perform better at home vs. away, on far away road games or closer games, and if they excel when they follow certain strategies. 

#9. List out the names of coaches and their salary who make more than the average salary of all coaches. Order the salaries from highest to lowest. 
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/0cadb998-7302-4d4c-86ce-216c917d80ed)

Description: The purpose of this query to see which coaches are making more than the average coaching salary within the organization. It provides insight into the teams salary distribution, and our client could use this to solidify their exceptional coaches, see if there are coaches that are overpaid, and overall make sure all their money is being used in a beneficial way rather than being wasted. If our client noticed a coach that is being overpaid and does the same thing as other coaches and they don't determine that they are absolutely essential, they could rework their contract to free up some money.

#10. List out first and last name of the player and type of equipment for players who have equipment with the condition broken. Additionally list out the practice duration for practices between 2 and 3 hours and the facility name and facility type that the practices took place in. Order by the practice duration. 
![image](https://github.com/ConnorConiglio/Group-2-Project-1/assets/163012186/c8306e66-60b1-4a7f-a938-03ed74ae0a69)

Description: The purpose of this query is to narrow in on 2-3 hour practices and see which players have broken equipment (bats, in this case). Furthermore, it will also show the type of facility and which facility the noted practice takes place in. This query is valuable to our client because it allows them to optimize facility use, ensure player safety (i.e. - stop them from using faulty equipment, and also allow players to get the most out of their practices. 

## **Database Information:**
Name of the database: ns_Sp24_61608_Group2
Additional information: Each query listed above is marked in the database using stored procedures which can be called using the following format: CALL TP_Qx();




