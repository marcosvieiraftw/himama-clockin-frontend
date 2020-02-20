
## Clock In / Out

HiMama ClockIn/Out frontend application responsible for managing UI/UX attributes.

## Instructions

Access via cloud by heroku:
1: Access the frontend application: [Frontend](https://himama-clockin-frontend.herokuapp.com/)
2: Login with one of the seeded accounts:
email: <b>marcos@marcos.com</b>
password: <b>123</b>
<i>Or</i>
email: <b>himama@himama.com</b>
password: <b>123</b>
<i>*Each user can only see their registers, so I seeded two accounts to test the data visibility accross access.</i>


To run locally:
1: Clone project
2: go to the project folder and run `npm i`
3: After the install of all dependencies, run `yarn start`
4: Your browser will open automatically on [http://localhost:3000](http://localhost:3000)
<i>* The server will be running in development mode.</i>

## Key features
* React + Redux managing application state.
* Barrel architecture: [A quick overview](https://hackernoon.com/react-project-architecture-using-barrels-d086146eb0f6)
* Fully modular with Layouts, Common components, Views, Helpers, Stores and Theme configurations (Typhografy, Color Pallete and so on)
* Http communication through Axios + JWT Authorization.
* UI validations with friendly visual components reproducing API validation messages.
* What you see is what you get: You can't submit a form if there's an invalid field. The user has visual confirmation by enabling/disabling buttons.
* Requests + Business inside stores = Skinny components responsible only for managing the UI artifacts.
* Functional components + React hooks as much as possible to avoid creating Class components everywhere.
* Beautiful style following HiMama's design patterns.
* It is a small application but it was organized in the way it can grow as much as needed. No cyclic dependency between components.
* .env file configured to make deploys easier.

## Questions
* How did you approach this challenge?
I started by reading the requirements over and over to not make assumptions. Once I understood the requirements I went to HiMama website to gather all visual identity: Colors, Components, Common approaches. With all in hand, I draw the screens in a draft paper to think about the best usability/experience.

* What schema design did you choose and why?
I chose React as Javascript framework because it's more common for HiMama developer team - thinking about future evolution. I first developed the whole visual structure and then I just fit the legos(Components).
For backend, I chose Ruby On Rails API Only + Postgres to quickly develop the endpoints and its constraints. I also dockerized the whole backend to make easier to run in all developers machines (Works not only on my machine :D ) - further information about backend and approach can be accessed here on its [Repository](https://github.com/marcosvieiraftw/himama-clockin-api)

* If you were given another day to work on this, how would you spend it?
<b>Frontend</b>
1: Refine the interface by adding some visual resources.
2: Refine the frontend code by adding PropTypes to all components.
3: Implement automated tests.
4: Evolve the protection of the routes to avoid the blink effect.

   <b>Backend</b>
   1: Create an admin namespace to administrate all users registers.

* What if you were given a month?
1: Implement super admin access.
2: Implement an analytical module to retrieve reports from all users.
3: Implement an hour bank feature according to the country work laws.
4: Implement card components based on days instead of a table with all events.
5: Improve constraints.
6: Gather the needs/requirements by talking to the future users to plan the next sprint/month of work.
