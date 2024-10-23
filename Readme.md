# Python Backend Engineer Take-Home Task

## Objective:
You are required to build a Django-based backend application that integrates with a third-party API, exposes RESTful endpoints, and supports user interactions with the data. Additionally, you will be required to write unit tests, to deploy the application, and to document the project.

## Expected deliverables and evaluation criteria
* Have a working prototype of the task described below. It is fine if your prototype's performance does not match the quality you may have in mind. We value a prototype showcasing all the required tasks moderately well over a prototype which solves just a few of the required tasks very well.
* (We will) assess how well you scope and assess the different components involved which will solve this problem
* Assess how you divide your labor into the components you identify, and how quickly you're able to prototype and finish implementing those components. Remember, there's a time budget of a few days.
* Assess your attention to little details. This is important for us--how much you care for details shows us how much you can own any work assigned to you.
* Assess how you resolve situations when you're stuck.
* Assess how well you communicate and let all stakeholders know of your progress. We emphasize constant communication over receiving no communication for days, and just seeing a dump of the results on the day of your submission. This has multiple drawbacks: (1) it gives us no insight into the process you employ to evaluate a problem and come up with a solution. (2) it gives us no room to help you in case you're stuck on any step. Consider this to be a task you will receive on your job - demonstrate to us how you will work on the task in such a setting.

## Task Description:
You will build a simple application that interacts with a weather API and allows users to search for weather conditions based on a city's name. The application should have a database to store search history and allow users to view the search history.

### Requirements:

**API Integration:**
* Use the OpenWeather API (or any other weather API of your choice).
* Create a Django view that accepts a city name, fetches the weather data for that city from the API, and returns relevant weather information (temperature, weather conditions, etc.).

## Django RESTful API:
* Implement the following RESTful API endpoints using Django and Django REST Framework (DRF):
* GET /weather?city={city_name}: Fetches weather details for the provided city name using the third-party API.
* GET /history: Returns a list of recent searches from the database, including city names and timestamps.
* DELETE /history: Clears all search history from the database.

## Database (Django ORM):
1. Use Django ORM to create a model that stores the search history.
2. The model should contain the following fields: city_name (CharField), timestamp (DateTimeField)
3. Store the city name and timestamp for each search in the database.


## Deployment:
* Deploy the Django application on a cloud platform of your choice (e.g., Heroku, AWS, etc.).
* Provide the link to your deployed application in the README.

## Unit Tests:
Write unit tests for your API endpoints using any suitable testing framework.

## Documentation:
Include a README.md that provides:
1. A brief description of the project.
2. Instructions on how to set up the project locally.
3. Steps to run tests.
4. The API documentation (i.e., list the available endpoints and expected input/output).
5. Link to the deployed version of the application.


## Evaluation Criteria:
**API Integration:** How well you understood the third-party API documentation and integrated it into your app.
**Code Quality:** Clarity, organization, and structure of your code (including adherence to Python best practices).
**Database Management:** Correct use of a relational database for storing and retrieving data.
**Testing:** Unit tests and test coverage, along with the correct use of testing libraries.
**Deployment:** Successful deployment and functionality of the application on a cloud platform.
**Documentation:** Clear and concise documentation in the README.md, covering setup, usage, and API details.

## Expected Time:
This task should take 12-14 hours to complete, including time to understand the third-party API, coding, testing, deployment, and documentation.


## Instructions to submit your work
* Do not fork this repo. Work on a local copy, and ensure this is a private repository. Add the username sachin-ramailo as a collaborator, so that Sachin can access the repo as well.
* Make it a habit to push changes upstream to your repo as frequently as feasible.
* Use Python3.8+ for this work.
* We greatly value reproducability of results. Use conda to create an environment and set up your repository.
* Use a .gitignore file to ensure you are not adding junk files to the repo.
* Have a ./src/ folder containing the source.
* Have a ./env/ folder containing the Conda environment file you create for this project.
* Have a ./data/ folder containing all the data your source accesses.
* Have a ./tests/ folder to write out unit tests for key functions. Look up the unittest package in Python if you haven't used it before. Also, not every function you write needs to be tested---exercise your judgement and prioritize which function you want tested.
* Keep updating this README with instructions which will help with the reproducability of your work/results.
* The topmost section of your readme file should be titled Approach. In this section, concisely describe the overeall approach you considered to solve this problem. Describe the general strategy you used, the key tools you considered, the different metrics you considered to evaluate your work, and any other detail relevant to the task goals and the evaluation criteria mentioned above.
* Communication: Write an email to jobs@mlexperts.ai with the subject "Python BE Exercise evaluation: [your full name]". We will acknowledge your email.
* Please then constantly communicate on the mail thread on how you are approaching the problem, how you are thinking about the solution, progress made, etc. The more updates you share, the more clarity we have on your thought process in solving a problem.
* This task is expected to take a maximum of 1 week of your time. It is possible to write this up in two full days over a weekend. If it is taking you longer, please write to jobs@mlexperts.ai explaining your situation.
* Focus on getting the core functionality right first, and have a working prototype of your solution.
* For any questions, write to jobs@mlexperts.ai with subject: "Query on Python BE Exercise"
* All the best!