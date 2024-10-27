Volleyball fantasy App: 
list of things the project has to be able to do: 
1- login page For regular users and admin
 1a- a create an account button for regular users
 2- for the admin : 
2a- have access to and be able to edit the “draft list” which is a list of players who will be participating in the volleyball games each player will have information such as “name” “fantasy points” “wins” “losses” “number of MVP’s” “overall player value” . The fantasy points will have a further break down into categories that will be listed later.
 2b- the admin will be able to edit the “tournament” page that shows: the current tournament bracket that details which teams are going up against each other, a number that represents odds for that team to win the whole tournament which is based upon each players total amount of wins/loses combined for each team, which team won previous games, game times, on this page the admin will be able to input final game scores and update matchups. Also on the tournament page there is a list of the teams detailing which players are on which teams but not showing any fantasy points or other information besides names. 
3- for the regular user 
3a- they will be able to see the draft list
 3b- they will be able to put together a team of 8 players from the draft list listing these players into the different positions in volleyball
 3c- they will have access to a “edit my team” page where they will be able to create and edit their draft team.
 3D- 
they will have access to a “view my team page” where they can view their fantasy team that displays the full information on each of their players such as name” “fantasy points” “wins” “losses” “number of MVP’s”. And a total score of their fantasy points.
 4- there has to be a “tournament history” page that displays all previous tournaments and their brackets 
5- there has to be a way to create a new tournament that includes new brackets etc
 6- after the admin designates that a tournament has ended use each players fantasy points to update their “overall player value” on the draft list 


 point system as follows:
 Scoring any point “ _I “= 1 point 
Part of Point “ _I “= 1 point 
Losing any point “ _X “= -1 point 
Kill “ _K” = 2 points
 “_KS “if assisted from the setter
. Ace “ _A “= 2 points 
No-touch Ace “ _NA “= 3 points
 Dig “ _D “= 1 points 
MVP “ _MVP “= 3 points
Key Functional Areas and Suggested Tech Stack
Authentication System
Login and Account Creation: Use JWT for authentication and Bcrypt for password hashing to secure user data.
User Roles: Implement role-based access to separate admin and regular user privileges.
Admin Features
Draft List Management: Create a CRUD interface (Create, Read, Update, Delete) where the admin can manage player details like fantasy points, wins, losses, MVPs, and overall player value.
Fantasy Points Breakdown: Include categories for different types of points (e.g., kills, assists).
Backend Models: Use a database like MongoDB or PostgreSQL with models for Player, Stats, Tournament, and Team.
Tournament Page:
Tournament Bracket: Implement a dynamic bracket that can be updated with game results and show odds. Use a charting library like D3.js or Chart.js.
Odds Calculation: You can calculate odds based on the combined win/loss ratios of each team.
Match and Score Editing: Allow admins to input final scores and update upcoming matchups.
Team Rosters: Display team rosters with basic info without fantasy points.
User Features
Draft List Viewing: Let users view all available players with their stats.
Fantasy Team Creation and Editing:
Allow users to select 8 players and assign them to volleyball positions. Use a drag-and-drop library (e.g., React DnD) for an intuitive team-building experience.
Use an API endpoint to update and store user team selections.
View My Team: Create a summary page that shows each team member’s detailed stats and the team’s total fantasy points.
Tournament History Page
Display previous tournament brackets and scores, using a database query to retrieve archived data.
Tournament Creation
Design an interface for admins to create a new tournament, including brackets, team assignments, and scheduling.
Player Value Update System
Automate the calculation and updating of each player’s overall value once a tournament ends, based on accumulated fantasy points.
