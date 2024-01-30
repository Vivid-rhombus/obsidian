Length: Month, month and a half (net, not bruto) - 35 days

#TODO Discuss use of ChatGPT - Maybe ask to explain verbally logic behind their functions.

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
		- Use keyboard for stuff 
	- Add button that checks for palindrome
- Docker + Openshift + CI/CD - 2 days

- Per team
	- FS, Mounts, PVCs, etc
- RabbitMQ?


- Basic hooks (useEffect, useMemo, useState)
	- MUI and correct styling (default props -> sx)
	- Project:
		- Calculator?
		- Prebuilt API to connect to?
	- Good utils
	- Unit tests - Jest
	- Asynchronisity 
	- Project:
		- Call of Duty?
		- Task list
		- MongoDB
Working with configs - env files

צריך פק"ל התקנות מוכן ומעודכן מראש






Project: Calculator
Pre made backend
- Front
	- Calculator front that is connected to some backend
	- 
- Back
	- 

## Linux
Commands from Omer Chen
## Git
Learn the basics of Git. What is it, what is it used for as well as common commands and what they do. Emphasize work with rebases and not merges. 
_Sources:_
![Learn Git with Mosh - video](https://www.youtube.com/watch?v=8JJ101D3knE&ab_channel=ProgrammingwithMosh)

![Git crash course - Video](https://www.youtube.com/watch?v=SWYqp7iY_Tc&ab_channel=TraversyMedia)

[Atlassian embed - read](https://www.atlassian.com/git)

## Node
Get a basic understanding of what Node/JS is, get a basic familiarity with the language, syntax and data types in it. 

#TODO Need to figure out how to teach them to run their JS in node not browser or whatever

Sources:
[JS video - watch to 1:10:30](https://www.youtube.com/watch?v=hdI2bqOjy3c&t=2s&ab_channel=TraversyMedia)
[Node - watch to 33:00](https://www.youtube.com/watch?v=TlB_eWDSMt4&ab_channel=ProgrammingwithMosh)

## Project
The project will be split into three-ish parts:
- Back
- Front
- CI/CD

### Back
Create a backend server capable of supporting your project :)
#### Step 1: 
Create an Express server that only has a health route and runs off of a port given to it from a config file.
#### Step 2: 
Create the basic operation route that can do the following:
- Receive a string
- Parse that string into a series of mathematical operations - Using (https://mathjs.org/docs/expressions/parsing.html)
- Return the result
#### Step 3:
Add validations and testing
Validations - very basic Joi, like only string or smth
#### Step 4:
Save every successful operation and it's result in the DB

### Front
Create a front for the project 

#TODO Split into steps in Figma + add sources to learn it from
### CI/CD
Run your project with CI/CD workflow on openshit
