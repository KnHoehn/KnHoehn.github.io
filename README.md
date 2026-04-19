My name is Kayla Hoehn and I am a student at Southern New Hampshire University (SNHU). For the past four years I have been pursuing my bachelor’s degree in computer science with a concentration in software engineering, and am projected to graduate May 1st, 2026.

## Professional Self-Assessment

With each course I’ve taken at SNHU, it has reinforced my career goals of becoming a software engineer while teaching me the concepts and values associated with the occupation. By SNHU supplying me with the foundations, best practices, and advanced concepts of computer science and software engineering, this has prepared me to enter the professional space.

During my time in the computer science program, I have learned how to collaborate in a team environment by taking courses that taught me SCRUM ideology and how to participate in an Agile team. I have also learned how to effectively communicate with stakeholders by taking courses that taught me how to collect requirements from stakeholders, as well as design and build an application from those requirements.

Additionally, I have developed a strong knowledge of data structures and algorithms by taking courses that taught me how to choose and apply algorithmic concepts such as binary search trees, linked-lists, vectors, and hash tables.

I have also gained the necessary software engineering skills and experience by taking courses that taught me both fundamental and advanced concepts in Python, Java, and C++, how to build full stack web applications, mobile applications, and the Software Development Lifecycle. 

Furthermore, I have gained experience with databases by taking courses that taught me how to create and perform basic CRUD operations and advanced querying on both schema-based databases, such as MySQL, and schema-less databases, such as MongoDB. 

Finally, I have developed a strong foundation of software security and testing by taking courses that taught me how to code with a secure mindset, identify and fix vulnerabilities, and perform quality assurance testing on applications.


## ePortfolio Introduction

Ever since my first introduction to the Computer Science program, SNHU has been very forthright that their mission is to not only give us the knowledge and skills to excel in our field, but to also help us build a portfolio that can be shown as an introduction to our work and skills to potential employers. This ePortfolio showcases what I have learned while attending SNHU while also highlighting my strengths and demonstrating my range. Working on this ePortfolio has taught me how to reflect on my strengths and capabilities and come up with and apply my own design plan to enhance an application that showcases my talents.

For this ePortfolio we were tasked with choosing an artifact that we had created for a previous course in the SNHU computer science program and creating enhancements for it. We got to choose the enhancements ourselves as long as they met the criteria and were approved by the professor. The criteria for the enhancements were to reflect three categories: 

1. Software engineering and design 
2. Data structures and algorithms 
3. Databases. 

Through these enhancements we also had to ensure we covered all five course outcomes:

1.	Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.  
2.	Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.  
3.	Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.  
4.	Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.
5.	Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.

For the software engineering and design category, I chose to rewrite the application into Java and modularize it into classes. For the second category of data structures and algorithms, I chose to refactor the code to incorporate Object Oriented Programming, a new scoring system, and the ability to choose the theme of the game by swapping JSON’s. For the last category of databases, I chose to create a database for the game so I could incorporate saving and displaying end game stats as well as a login system.

## Artifact

The artifact I have chosen for all three enhancements is the final project for my introduction to scripting class, which was a text-based game written in Python. The purpose of this assignment was to apply what we had learned throughout the course and demonstrate it in the creation of this text-based game. The objective of the game is to collect the objects in each room before reaching the room where the alien resides. If the player reaches the alien before collecting all of the items, it’s game over. If the player collects all of the items before reaching the alien, the player wins. This artifact was originally created during my first semester in the Computer Science program in 2022. 

I selected this artifact to improve upon because I think it has a lot of potential. With it being a simple text based game, there is so much you could enhance to expand or improve upon, which gave it a lot of potential to be able to add enhancements in the software engineering and design, algorithms and data structures, and databases categories, and I think even past those enhancements the game could become really expansive in areas I haven’t even entertained yet. 

- [Link to the original artifact](https://github.com/KnHoehn/Python-Text-Based-Game)

## Code Review

Before we started on our enhancements, we conducted a code review of the artifact to explain its functionality, the planned enhancements, as well as going through a checklist to review the code through a critical lens and point out any weaknesses or areas of improvement.

- [Link to the Code Review](https://www.youtube.com/watch?v=kRiUtRzsGTI)

## Enhancement One

For the first enhancement category, Software Engineering and Design, The artifact was improved by porting it from Python to Java and modularizing it into classes. This made the code more clean, reusable, maintainable, and readable. This showcases my skills of being able to determine how to maintain the same functionality from one language to another while also incorporating logic and design improvements and fixing bugs. 

Through the incorporation of these enhancements, I have met the following course outcomes:

Rewriting the code into Java and modularizing the code demonstrated the ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.

By rewriting by code into Java, following best practices, and modularizing the code into classes, making the code more readable, maintainable, and easier to debug, this satisfied the course outcome of design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.

By modularizing the code into classes, this made the code more organized for a collaborative environment and easier to expand upon. Therefore, I believe this enhancement also satisfies the course outcome of employing strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.  
So far, there are no further updates to my outcome-coverage plan.

One thing I knew I had to do to make this project work for all three enhancements was to create it as a Maven project so I will be able to easily add dependencies in later enhancements such as adding the database feature. I researched Maven and learned how to make a Java Maven project and how the file tree structure worked because it differs from a regular Java project. I already even added a dependency already during this enhancement because I found out that I could use a library from Apache Commons to easily capitalize the first letter of each word which is used when receiving the input from the user. 

A challenge I faced was when I refactored the command processing logic in the Command class and inventory item logic in the InventoryManagement class. I initially had trouble getting the output to say anything except “Invalid Move!” I realized my if-else structure wasn’t quite set up correctly and I had to make sure I was ensuring proper checks when splitting the user input to avoid errors.

I initially wanted to process all possible user commands in the Command class including if the user types “Exit”, but realized I could not return both the hashmap of  currentRoom if the user moved rooms or a Boolean value if the user typed “exit”, which was going to be my solution to not being able to break out of a while loop within a separate class was to instead send a Boolean value to tell the main class to break out of the loop. Therefore, I ended up having to check if the user input “Exit” first and then move on to calling the Command class if they did not.

- [Link to Text Based Game Enhancement One Repository](https://github.com/KnHoehn/JavaTextBasedGameEnhancementOne)

## Enhancement Two

For the second enhancement category, Algorithms and Data Structures, the artifact was improved by implementing algorithms to create a scoring system and refactoring data structures to utilize JSON files and Object-Oriented Programming to allow the user to choose the theme of the game, creating a customized experience for the user. Utilizing JSON files and Object-Oriented Programming also allows software developers to easily add or edit themes to the game. This showcases my skills of being able to create and utilize algorithms to incorporate features that rely on them as well as the ability to incorporate Object-Oriented Design principles to improve data structures.

Through the incorporation of these enhancements, I have met the following course outcomes:

implementing an algorithm for computing the players score satisfies the course outcome of design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.

Using Object Oriented Design programming satisfies the course outcome of demonstrating an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.

I hadn’t worked with JSON files much before this, so I learned how to make a JSON file and parse it into objects using the Gson library from Google.
I also learned how to use the Date library so I can retrieve the total time it took the user to beat the game and factor that into scoring.

A challenge I initially faced was having to move a lot of the command processing logic from the Command class back into main. I wanted to keep this separate but there are too many variables I needed to keep track of when processing the user’s command. To implement my scoring logic, I would need to be able to return a Room object to set the current room, an int to keep track of the user’s moves, and another int to the keep track of their move score. With Java only allowing one return type, this made keeping the command processing separate entirely too complicated. During my initial submission I opted to just keep the room movement logic in the command class and move everything else back into main, but later on during my work on enhancement three I had the thought to include a Player object class and incorporate the scoring variables with the Player object. This way I was able to update the variables without having to return them in a method and only having to pass in the Player object as a parameter.

Another challenge was when creating the JSON files, I decided to also make the boss room and the starting room different for each theme. This meant that for some maps the minimum amount of moves the user can take to collect all items and defeat the boss is now more than ten. My original proposal was to only allow a -10 to their moves score if the user took more than 10 moves, but because of the new maps I decided to include a -10 to the move score for every move they take from the start of the game.

- [Link to Text Based Game Enhancement Two Repository](https://github.com/KnHoehn/JavaTextBasedGameEnhancementTwo)

## Enhancement Three

For the third enhancement category, Algorithms and Data Structures, the artifact was improved by incorporating a database which allowed for the creation of a user account creation and log in system. The incorporation of a database also allowed for the user’s score to be saved at the end of the game and display to the user their top ten scores as well as a leaderboard of the top ten scores of all time by pulling the user and scoring data from the database. This showcases my skills of being able to create and connect to a database as well as successfully insert and retrieve data from it while following best practices such as incorporating prepared statements to avoid the possibility of SQL injection and hashing and salting the user’s password to avoid storing sensitive data to the database. 

Through the incorporation of these enhancements, I have met the following course outcomes:

By demonstrating that I can securely store and retrieve data from the database satisfies the course outcome of develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.  

During my feedback for my enhancement one, my professor mentioned I should look into tools to make sure I am following proper styling conventions. Because of this, I switched my IDE from using Eclipse to IntelliJ per my instructor’s recommendation and learned how to install plugins for it. I installed the plugins for SonarQube and CheckStyle and learned how to use those and refactored my code accordingly to make sure I am following the proper Java style conventions and best practices. 

Afterwards, I went back and improved my first and second enhancements following the suggestions from SonarQube and Checkstyle, which are reflected in the versions used in this ePortfolio. I had already known my main method was getting too complicated again and SonarQube solidified this thought by telling me I needed to reduce my cognitive complexity in main from 18 to the 15 allowed. As previously mentioned during enhancement two, I initially shifted a lot of the user input logic from the command class back to the main method to account for scoring logic and not being able to return everything I needed too. During my work on this enhancement is when I had the thought to make a Player object class and incorporate the scoring variables there so I can update the variables without having to return them in a method only having to pass in the Player object as a parameter. This helped me reduce my main method and move the command processing logic back to the Command class.

My professor also suggested I incorporate JUNIT testing, so I implemented that as well and it lead me to refactor some of the code because I realized some of the methods were entirely too complicated when writing the tests. This lead me to go back to my previous two enhancements and write JUNIT tests for them as well and refactor accordingly, which are reflected in the versions used in this ePortfolio as well.

I also learned how to connect to an external database via the MySql connector dependency and researched how to properly hash and salt a user’s password.

My database consists of a users table and a score_board table. The users table has a schema of user_id, user_name, user_password (Which is hashed and salted), and the salt used. The score_board table has a schema of score_id, user_name (which is a foreign key to reference the user_name in user_table), score (The user’s final score), moves (The user’s total moves), time (The time it took them to beat the game), and theme (The theme played when the score was recorded). A screenshot of the schema can be found in the repositories README file.

- [Link to Text Based Game Enhancement Three Repository](https://github.com/KnHoehn/JavaTextBasedGameEnhancementThree)
