# Match SoC

![Screenshot 2021-02-11 at 17 09 04](https://user-images.githubusercontent.com/70659641/107671562-de412f80-6c8b-11eb-84eb-dce062189c78.png)

This project is the result of a week project in an agile tech team of 4 individuals responding to our brief - 'How to improve bootcamper and mentor relationship.'

## Details

The app consists of a frontend written in React and a backend written in Node.js, Express and PostgreSQL. The aim was to imporve the relationship between bootcampers and mentors by guaging how closely linked the two parties are. The application does this by comparing both parties based on their industry and interests.

## Built With

- React
- JSX
- HTML
- CSS
- JavaScript
- React Router DOM
- Node.js
- Express
- PostgreSQL
- Nodemon
- Cors
- dotenv

## Prerequisites
You will need a Postgres table to utilise the repo.

You will also need to create a .env file in the root folder containing:
- HOST
- DATABASE
- USER
- PORT
- PASSWORD

These can be obtained from where you host your database.

## Installation

1. Clone down both the front and backend repos using the following commands:
```
git clone https://github.com/brsm019/bootcamper-mentor-matcher.git
```
2. Install the npm modules for both the front and backend repos using the following command:
```
npm i
```
3. Add a .env file in the root folder of the frontend folder with the entry:
```
REACT_APP_BACKEND_URL=http://localhost:5000
```
4. Add a .env file in the root of the frontend folder with the entry:
```
DATABASE_URL= enter your postgres database uri here
```
5. Create and populate the tables in the backend with the following commands:
```
npm run createTable
```
```
npm run populateTable
```
6. Finally, run both the frontend and backend repos:
```
npm start
```

## Usage

#### Search Page
This page is used to locate bootcampers and their information, use the search bar at the top to specify a bootcamper you are looking for. You can also delete bootcampers on this page.
#### Add User
In order to add a new user, navigate to the Add User page and fill in the form, make sure to specify whether they are a bootcamper or mentor. You also have the option to add additional information here or reset the form.
#### Compare
The compare page is used to assign a mentor to a bootcamper based on common interests and industries. Click on the bootcamper you want to find a match for and a matching score, as a percentage, will be generated with the assigned mentor.
