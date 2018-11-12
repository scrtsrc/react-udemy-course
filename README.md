﻿This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.

## Missing Firebase endpoint

Will need to create own on [Google Firebase Realtime DB endpoint](https://firebase.google.com/) and add it to a File called axios.js (under a newly created Folder in src)

```
src
└───assets
│  	└─── ...
└───axios
│   └───axios.js
│ 
└─── ...
```

```javascript
import axios from 'axios';

const instance = axios.create({
    baseURL: 'insert-own-endpoint'
});

export default instance;
```
