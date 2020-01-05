# React-development

Install Create React App, it is an officially supported package/way to create single-page React applications

```python
npm install -g create-react-app
```

Then you are able to create a React application, let's create one called myfirstreact.

Run this command to create a React application named myfirstreact:

```python
npx create-react-app myfirstreact
```

Then

```python
cd myfirstreact

npm start
```

Go to myfirstreact\src\App.js

```javascript
import React from 'react';
import logo from './logo.svg';
import './App.css';

function App() {
  return (
    <div className="App">
      <header className="App-header">
        <img src={logo} className="App-logo" alt="logo" />
        <p>
          Edit <code>src/App.js</code> and save to reload.
        </p>
        <a
          className="App-link"
          href="https://reactjs.org"
          target="_blank"
          rel="noopener noreferrer"
        >
          Hi Siddharth !
        </a>
      </header>
    </div>
  );
}

export default App;
```

Change any parts and save file. The server updates automatically

Replace all the content inside the ```<div className="App">``` with a ```<h1>``` element.

See the changes in the browser when you click Save.

```javascript
import React from 'react';
import logo from './logo.svg';
import './App.css';

function App() {
  return (
   <div className="App">
        <h1>Hello World!</h1>
      </div>
  );
}

export default App;
```

Now you have a React Environment on your computer, and you are ready to learn more about React.

Now start by stripping down the src folder to only contain two files: index.js and index.html. Put the rest in a backup folder. You'll have to create index.html

index.js:

```javascript
import React from 'react';
import ReactDOM from 'react-dom';

const myfirstelement = <h1>Hello React!</h1>

ReactDOM.render(myfirstelement, document.getElementById('root'));
```
index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>React App</title>
  </head>
  <body>

    <div id="root"></div>

  </body>
</html>
```

Update index.html 

```html
<!DOCTYPE html>
<html>

<body>
  
<script>
class Car {
  constructor(name) {
    this.brand = name;
  }
}

mycar = new Car("Ford");

document.write(mycar.brand);
</script>

</body>
</html>
```
