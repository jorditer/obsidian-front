## [[Components As Functions]]

### Cool AF.

```jsx
const Link = () => {
    return (
      <p>
        <a href="//react.dev">Read more about React</a>
      </p>
    );
}

const App = () => {
    return (
      <Fragment>
        <Link />
        <Link />
        <Link />
      </Fragment>
    );
}


```

## [[Components as Classes]]

### I think deprecated

```jsx
class Link extends Component {
  render() {
    return (
      <p>
        <a href="//react.dev">Read more about React</a>
      </p>
    );
  }
}

class App extends Component {
  render() {
    return (
      <Fragment>
        <Link />
        <Link />
        <Link />
      </Fragment>
    );
  }
}

```
## Using React.createElement

```jsx
	const world = React.createElement("p", {className: paragrah"}, "Hello World");
	const link = React.createElement("a", { href: "//react.dev" }, "Read more");
```
## Keep them in separate files
### Is good practice to put  the `index.js` inside `src` and all components inside `components` or in a single `App.js` file.

```jsx
import React from "react";
import Stats from './Stats';

const Counter = props => {
	const id = props.id;

	return (...);
}

export default Counter;
```

## [[Conditionals]]

## [[Keys]]