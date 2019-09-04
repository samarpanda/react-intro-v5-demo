# React Demo App

## Steps

1. Starting React with basic UMD build using from unpkg

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>React Intro</title>
  </head>
  <body>
    <div id="root">Not rendered</div>
    <script src="https://unpkg.com/react@16.8.4/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16.8.4/umd/react-dom.development.js"></script>
    <script>
      const App = () => {
        return React.createElement(
          "div",
          {},
          React.createElement("h1", {}, "React Intro v5")
        );
      };

      ReactDOM.render(
        React.createElement(App),
        document.getElementById("root")
      );
    </script>
  </body>
</html>
```

2. Create a component & reuse component to create multiple instances

3. Passing in props to component & destructuring props

4. Install and setup Prettier

```cmd
npm i -D prettier
```

Install prettier plugin & user setting to configure

- Install plugin Prettier - Code formatter By Esben Petersen
- check the option "Format On Save"
- Prettier: Require Config - Requires a prettier config to format. Pretty useful as this auto format is not activated if the config file is not available.

5. Configure ESLint

```cmd
npm i -D eslint eslint-config-prettier
```

ESlint plugin & user settings to configure

- Install eslint plugin by Dirk Baeumer
- check the option "Eslint> Lint Task: Enable"
