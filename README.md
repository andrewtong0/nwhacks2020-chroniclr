# Chroniclr

Chroniclr was my team's submission to the nwHacks 2020 Hackathon. This web application served as a way for users to gamify their life, earning points for completing their goals and leveling up in the process.

![Chroniclr Screenshot](https://i.imgur.com/yUOEKt2.png)

How It Works:

Client
- The user inputs tasks or goals that they want to accomplish.
- Using NLP and keyword detection, we categorize the user's goal and automatically assign it a point value based on its difficulty.
- The user gains experience and levels up as they complete their tasks.

Server
- When the user submits a task, we use NLP and keyword detection to determine which category to place the task in (fitness, academics, career, social).
- We assign an experience (XP) value to the task, and update the database.
- When the user completes the task, it sends a POST request to our server, where we clear the quest and update the XP values based on the completed task.

Dependencies
- Python 3: Runs and hosts server for backend
- Node JS: Runs web server for frontend
