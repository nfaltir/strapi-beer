# Frontend

<br>

- create a react app in root folder `create-react-app frontend`
- install `npm i react-router-dom`
- rm App.css, App.test.js, logo.svg, reportWebVitals.js, setupTests.js

<br>

#### inside index.js

<br>

-rm `import reportWebVitals from './reportWebVitals';`

<br>

#### inside App.js

- rm `import logo from './logo.svg';`
  `import './App.css';`
- rm everything inside `App div`

## Create Routes

```
  There is a new version of react-router-dom and code in the tutorial doesn't work. Install older version:
npm uninstall react-router-dom
npm install react-router-dom@5.2.0

 or change Switch to Routes and Route declarations to this:
 <Route path='/details/:id' element={<ReviewDetails />} />

```

<br>

## Hooks

<br>

- reuseable components

## After Setup and Tests

install graphql in strapi admin panel inside marketplace

<br>

## Enable permissions to display Categories data

<br>

- inside content manager folder, enable unathenticated user to `find` and `findone` inside `Category` collection

<br>

## Install Markdown to enable Rich text functionalities

<br>

- `npm i react-markdown`
