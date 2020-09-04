# Spaced Repetition Capstone
A Spaced Repetition App by Seyi and Rebecca

### Live Link: 
[https://spaced-repitition-rebecca-seyi.vercel.app](https://spaced-repitition-rebecca-seyi.vercel.app)

### Client Repo:
[https://github.com/thinkful-ei-panda/Spaced-Repetition-Rebecca-Seyi](https://github.com/thinkful-ei-panda/Spaced-Repetition-Rebecca-Seyi)

### Server Repo
[https://young-caverns-95905.herokuapp.com](https://young-caverns-95905.herokuapp.com)

### Tech Stack
Front-end: React.js, CSS, media queries
Server: PostgreSQL
Hosting/SaaS: Heroku 
Development Environment: Zeit Now
Testing: Cypress, Mocha, Chai

### Summary

The user will have the option to log in or sign up, and then will be directed to a dashboard displaying their total correct answer, a list of French words to memorize, as well as the number of times they got each word wrong or right. 

<br />

![Dashboard](README-asset/PastedGraphic3.png?raw=true)

The app displays a word in French and then asks the user to recall the corresponding word in English.
<br />

![LearnPageFirstView](README-asset/PastedGraphic4.png?raw=true)

<br />


If the user answers incorrectly, that word will be asked again sooner. 

<br />

![LearnPageIncorrectAnswerView](README-asset/PastedGraphic5.png?raw=true)

If the answer is correct, the user will be asked later on.

<br />

![LearnPageCorrectAnswerView](README-asset/PastedGraphic6.png?raw=true)


The user will be able to see their total count of correct guesses as well as the number of times they got each word wrong or right.





<br />


<br />
## Setup

To setup the application
<!-- https://spaced-repitition-rebecca-seyi.vercel.app -->
1. Fork and clone the project to your machine
2. `npm install`. This will also install the application *Cypress.io* for running browser integration tests

The project expects you have the Spaced repetition API project setup and running on http://localhost:8000.

Find instructions to setup the API here https://github.com/Thinkful-Ed/spaced-repetition-api.

## Running project

This is a `create-react-app` project so `npm start` will start the project in development mode with hot reloading by default.

## Running the tests

This project uses [Cypress IO](https://docs.cypress.io) for integration testing using the Chrome browser.

Cypress has the following expectations:

- You have cypress installed (this is a devDependency of the project)
- You have your application running at http://localhost:3000.
  - You can change the address of this expectation in the `./cypress.json` file.
- Your `./src/config.js` is using http://localhost:8000/api as the `API_ENDPOINT`

To start the tests run the command:

```bash
npm run cypress:open
```

On the first run of this command, the cypress application will verify its install. Any other runs after this, the verification will be skipped.

The command will open up the Cypress application which reads tests from the `./cypress/integration/` directory. You can then run individual tests by clicking on the file names or run all tests by clicking the "run all tests" button in the cypress GUI.

Tests will assert against your running localhost client application.

You can also start all of the tests in the command line only (not using the GUI) by running the command:

```bash
npm run cypress:run
```

This will save video recordings of the test runs in the directory `./cypress/videos/`.
