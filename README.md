# web39project

http :4000/ --verbose

CD into folder
[x] cd 

Create Directory
[x] mkdir web-39-project

Open in VSCode
[x] code .

Make .gitignore 
[x] npx gitignore node

Create new Repo
[x] git init 
[x] git status 
[x] git add .
[x] git commit 
[x] git push 

Find out if git is working
[x] git status 

Reveal files 
[x] ls -lah

Create package.json
[x]npm init -y

Add eslint
[x]npx eslint --init

Options after installing eslint
[x] Common JS
[x] None of These
[x] No 
[x] TypeScript
[x] Node
[x] JSON
[x] YES

Install Nodemon
[x] npm i -D nodemon

Install Other Dependencies 
[x] npm i express cors dotenv 

Create a start script in package.json
[x] "start": "node index.js"
[x] "server": "nodemon index.js"

[x] Create an index.js

[x] npm start
[x] npm run server

[x] make .env file
    NODE_ENV=development
    PORT=5000

[Heroku] 
Connect Github
Search for Repo
Look for Manual deploy
Click deploy
Wait a couple seconds 
It should start deploying

[x] create folder called client
[x] cd into client
[x] npx create-react-app .
[x] npm run build

Add the following to [server.js]
const express = require('express')
server.use(express.static(path.join(__dirname, 'client/build')))

Add the following to [index.js] 
server.get('*', (req, res) => {
    res.sendFile(path.join(__dirname, 'client/build', 'index.html'))
})

[package.json]
under scripts
"heroku-postbuild": "cd client && npm i & npm run build"

Optional in [package.json]
"engines": {
    "node": "14.15.4",
    "npm": "6.14.11"
},
