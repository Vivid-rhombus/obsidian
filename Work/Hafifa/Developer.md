Length: Month, month and a half (net, not bruto) - 35 days

ChatGPT: Minimize usage, and if you do, make sure to understand what the code does and why.

Deadlines: PR per topic with a deadline.

Agenda:
- [[#Linux]] - 1 day
- [[#Git]] - 2 days
	- Focus on good Git behavior
	- Focus on working with rebase and rebase interactive
- Basic JS - 3 days
- Project - 24 days
	- Basic Express server - 2 days
		- Health route
		- Port from .env config file
	- Route - 8 Days
		- Add basic math route ( + - * / ^ sqrt mod )
		- Validation + Joi
		- Tests - 
			- Supertest, Jest
	- MongoDB - History/Undo - 4 Days
		- Add routes
	- React - 10 Days
		- Create the UI
		- Hook up to backend
		- Bonus - Use keyboard for stuff 
- Docker + Openshift + CI/CD - 2 days

## Linux
Acquire a basic familiarity with the following linux commands:
- cd
- pwd
- cp
- echo
- rm
- ls
- mkdir
- nano/vim - how to edit / save / exit
- touch
- chmod
- ssh
- grep
- pipe (`|`) and redirect operator (`>`, `>>`)
## Git
Learn the basics of Git. What is it, what is it used for as well as common commands and what they do. Emphasize work with rebases and not merges. 
_Sources:_
![Learn Git with Mosh - video](https://www.youtube.com/watch?v=8JJ101D3knE&ab_channel=ProgrammingwithMosh)

![Git crash course - Video](https://www.youtube.com/watch?v=SWYqp7iY_Tc&ab_channel=TraversyMedia)

[Atlassian embed - read](https://www.atlassian.com/git)

## Node
Get a basic understanding of what Node/JS is, get a basic familiarity with the language, syntax and data types in it. Make sure to cover the concepts of `async/await` and `promises`!

Sources:
[JS video - watch to 1:10:30](https://www.youtube.com/watch?v=hdI2bqOjy3c&t=2s&ab_channel=TraversyMedia)
[Node - watch to 33:00](https://www.youtube.com/watch?v=TlB_eWDSMt4&ab_channel=ProgrammingwithMosh)

## Project
The project will be split into three parts:
- Back
- Front
- CI/CD

### Back
Create a backend server capable of supporting your project :)
#### Beginning the project
This will be the beginning of the project:
- Create a git project.
- Create an `npm` project.
- Create an express server that has a health route.
- Load the starting port for your server from a `.env` file.

What technologies to use: 
- Use [express](https://www.npmjs.com/package/express) to create the server, read more about it [here](https://expressjs.com/).
- Use [dotenv](https://www.npmjs.com/package/dotenv) to load the `.env` file.
#### Developing the basics
This will add some features to your server, making it useful:
- Add a route that receives a string, will parse the string and then return the results.
- Add validation to your route
- Add tests to your routes

What technologies to use: 
- Use [math.js](https://mathjs.org/docs/expressions/parsing.html) for parsing and evaluating the math.
- Use [joi](https://www.npmjs.com/package/joi) for validation and [express-joi-validation](https://www.npmjs.com/package/express-joi-validation) as middleware.
- Use [jest](https://www.npmjs.com/package/jest) and [supertest](https://www.npmjs.com/package/supertest).
#### Expanding features
This will add additional features.
- Add routes that can do the following:
	- Receive a number, return if part of Fibonacci series.
	- Receive a number, return if an Armstrong number.
	- Receive a number, return if a Palindrome.
- Add validation for all your routes.
- Add tests for all your new routes.

#### Storing results
Now, to add some additional stability to your project:
- Add a MongoDB connection singleton, that gets its connection string from environment variables.
- Store the query and the result from the basic math operations in the DB. (not fib, armstrong or palindrom functions)
Interacting with the stored results:
- Add a route that allows a user to get the stored results and another that allows a user to delete a stored result by its generated UUID.
- Add validations to the `DELETE` route
- Add tests to the new features

What technologies to use:
- Use the [MongoDB](https://www.npmjs.com/package/mongodb) driver to create the singleton. Example [here](https://www.mongodb.com/languages/express-mongodb-rest-api-tutorial). Do **not** use `mongoose`. Look for tutorials, like [here](https://learn.mongodb.com/learning-paths/introduction-to-mongodb).

### Front
Create a front for the project. Link to the [figma](https://www.figma.com/file/r5XwxgAitKLAlXPOv7ZUX5/Hafifa-Calculator?type=design&node-id=0%3A1&mode=design&t=Le7WHmXQDFwIYdfn-1)

Try and keep up with the backend. Once you finish a feature for the back, add the relevant button/functions in the front.

Use [vite](https://vitejs.dev/guide/) to create a `vite` & `react` project, use [material-ui](https://mui.com/) (also known as `mui`) wherever you can, and use [useSWR](https://swr.vercel.app/) for data fetching.
### CI/CD
Containerize your application by adding a `Dockerfile` and running it locally.
Finally, add CI/CD and deploy your app to Openshift.
