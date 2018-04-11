# Intro to Express

## Implement a basic web server using Express.js

### Setup Instructions

###### In terminal

```
# (1) navigate to your activities directory
$ cd ~/Documents/muktek/activities

# (2) Create a activity--intro-to-express project
$ mkdir activity--intro-to-express

$ cd activity--intro-to-express

# (3) Create the main file (`server.js`)
$ touch server.js

# (4) Install express dependency
$ npm install --save express
```

###### In file


#### (1) Import ExpressJS

#### (2) Initialize the app

#### (3) Setup the PORT, use process.env to check if we have a PORT in use

#### (4) Create four routes

```
/                  : 'Home page'
/api/courses       : courses (in JSON format)
/api/courses/:id   : individual course (in JSON format)
/api/courses/all   : this should a redirect to /courses
```

###### Courses
```js
const courses = [{
  id: 1,
  name: 'Terminal and UNIX',
  length: '15 hours'
}, {
  id: 2,
  name: 'Git and GitHub',
  length: '15 hours'
}, {
  id: 3,
  name: 'HTML + CSS Basics',
  length: '10 hours'
}, {
  id: 4,
  name: 'Introduction to JavaScript',
  length: '15 hours'
}, {
  id: 5,
  name: 'Intermediate JavaScript I',
  length: '20 hours'
}, {
  id: 6,
  name: 'Intermediate JavaScript II',
  length: '25 hours'
}, {
  id: 7,
  name: 'Node and Express.js Fundamentals',
  length: '15 hours'
}, {
  id: 8,
  name: 'React.js Fundamentals',
  length: '25 hours'
}];
```

## Explorer Mode

+ Use a filter over `courses` data to render an individual item when user is visiting `/api/courses/:id`. Make sure that you compare information based on `id` property.
