## Kayla Hoehn CS-499 ePortfolio

[Code Review](https://www.youtube.com/watch?v=kRiUtRzsGTI)

The artifact I have chosen for all three enhancements is the final project for my introduction to scripting class, which was a text-based game written in Python. The purpose of this assignment was to apply what we had learned throughout the course and demonstrate it in the creation of this text-based game. The objective of the game is to collect the objects in each room before reaching the room where the alien resides. If the player reaches the alien before collecting all of the items, it’s game over. If the player collects all of the items before reaching the alien, the player wins. This artifact was originally created during my first semester in the Computer Science program in 2022. 

[Link to the original artifact](https://github.com/KnHoehn/Python-Text-Based-Game)

I selected this item because I think it has a lot of potential. With it being a simple text based game, there is so much you could enhance to expand or improve upon, which gave it a lot of potential to be able to add enhancements in the software engineering and design, algorithms and data structures, and databases categories, and I think even past those enhancements the game could become really expansive in areas I haven’t even entertained yet. 

The artifact was improved by porting it from Python to Java and modularizing it into classes. This made the code more clean, reusable, maintainable, and readable. This showcases my skills of being able to determine how to maintain the same functionality from one language to another while also incorporating logic and design improvements and fixing bugs. 
Through the incorporation of these enhancements, I have met the following course outcomes:

Rewriting the code into Java and modularizing the code demonstrated the ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.

By rewriting by code into Java, following best practices, and modularizing the code into classes, making the code more readable, maintainable, and easier to debug, this satisfied the course outcome of design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts.

By modularizing the code into classes, this made the code more organized for a collaborative environment and easier to expand upon. Therefore, I believe this enhancement also satisfies the course outcome of employing strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.  
So far, there are no further updates to my outcome-coverage plan.

One thing I knew I had to do to make this project work for all three enhancements was to create it as a Maven project so I will be able to easily add dependencies in later enhancements such as adding the database feature. I researched Maven and learned how to make a Java Maven project and how the file tree structure worked because it differs from a regular Java project. I already even added a dependency already during this enhancement because I found out that I could use a library from Apache Commons to easily capitalize the first letter of each word which is used when receiving the input from the user. 

A challenge I faced was when I refactored the command processing logic in the Command class and inventory item logic in the InventoryManagement class. I initially had trouble getting the output to say anything except “Invalid Move!” I realized my if-else structure wasn’t quite set up correctly and I had to make sure I was ensuring proper checks when splitting the user input to avoid errors.

I initially wanted to process all possible user commands in the Command class including if the user types “Exit”, but realized I could not return both the hashmap of  currentRoom if the user moved rooms or a Boolean value if the user typed “exit”, which was going to be my solution to not being able to break out of a while loop within a separate class was to instead send a Boolean value to tell the main class to break out of the loop. Therefore, I ended up having to check if the user input “Exit” first and then move on to calling the Command class if they did not.

[Text Based Game Enhancement One](https://github.com/KnHoehn/JavaTextBasedGameEnhancementOne)
