# Whiteboard Server - Node.js

This is a Node.js server for the Whiteboard web app. It provides RESTful web services for the Whiteboard clients to retrieve quizz questions and submit quiz attemps.

Whiteboard is a simple learning management platform where faculty can create courses and learning materials for students with various types of widgets, and students can take, submit and get scores for quizzes.

*MongoDB is needed for running the server locally.*

## RESTful API

Live API endpoint: https://wbdv-sp20-siyan-he-server-node.herokuapp.com/api

Please note that the services are hosted on Heroku so it may take few minutes to start when you access it.

| HTTP Method | URL Pattern                    | Description                                                  |
| ----------- | ------------------------------ | ------------------------------------------------------------ |
| GET         | `/api/quizzes`                 | Retrieves all the quizzes.                                   |
| GET         | `/api/quizzes/:qzid`           | Retrieves a quiz whose `_id` is `qzid`.                      |
| GET         | `/api/quizzes/:qzid/questions` | Retrieves the questions for a quiz whose `_id` is `qzid`.    |
| GET         | `/api/quizzes/:qzid/attempts`  | Retrieves all the attempts for a quiz whose `_id` is `qzid`. |
| POST        | `/api/quizzes/:qzid/attempts`  | Creates a new attempt for a quiz whose `_id` is `qzid`.      |
| GET         | `/api/questions`               | Retrieves all the questions.                                 |
| GET         | `/api/questions/:qid`          | Retrieves a question whose `_id` is `qid`.                   |

## Disclaimer

This is a personal project for CS5610 Web Development and the repository was migrated from GitHub Enterprise. For maintaining academic intergity, please do NOT reuse any code in this repository if you are working on your project for a related course.
