# Everything uses React.createElement which is pretty old school.
## Lvl 1

```jsx
class Link extends React.Component {
  render() {
    return React.createElement(
      "p",
      null,
      React.createElement(
        "a",
        { href: "//react.dev" },
        "Read more about React"
      )
    );
  }
}

const link1 = React.createElement(Link);
const link2 = React.createElement(Link);
const link3 = React.createElement(Link);
const group = React.createElement(React.Fragment, null, link1, link2, link3);
const domElement = document.getElementById("root");
ReactDOM.createRoot(domElement).render(group);
```
## Lvl 2

```jsx
class Link extends React.Component {
  render() {
    const link = React.createElement(
      "a",
      { href: this.props.url },
      `Read more about ${this.props.framework}`
    );
    return React.createElement("p", null, link);
  }
}

const link1 = React.createElement(Link, {
  framework: "React",
  url: "//react.dev",
});
const link2 = React.createElement(Link, {
  framework: "Vue",
  url: "//vuejs.org",
});
const link3 = React.createElement(Link, {
  framework: "Angular",
  url: "//angular.io",
});

const group = React.createElement(React.Fragment, null, link1, link2, link3);

const domElement = document.getElementById("root");
ReactDOM.createRoot(domElement).render(group);

```
##  Lvl 3

```jsx
class Link extends Component {
  render() {
    return React.createElement(
      "p",
      null,
      React.createElement(
        "a",
        { href: this.props.url },
        `Read more about ${this.props.framework}`
      )
    );
  }
}

class App extends Component {
  render() {
    const link1 = React.createElement(Link, {
      framework: "React",
      url: "//react.dev",
    });
    const link2 = React.createElement(Link, {
      framework: "Vue",
      url: "//vuejs.org",
    });
    const link3 = React.createElement(Link, {
      framework: "Angular",
      url: "//angular.io",
    });
    return React.createElement(Fragment, null, link1, link2, link3);
  }
}
```
## Lvl 4

```jsx
class Link extends React.Component {
  render() {
    return React.createElement(
      "p",
      null,
      React.createElement("a", { href: this.props.url }, this.props.children)
    );
  }
}
const boldReact = React.createElement("strong", null, "React");
const link1 = React.createElement(Link, { url: "//react.dev" }, boldReact);
const link2 = React.createElement(Link, { url: "//vuejs.org" }, "Vue");
const link3 = React.createElement(Link, { url: "//angular.io" }, "Angular");
const group = React.createElement(React.Fragment, null, link1, link2, link3);
const domElement = document.getElementById("root");
ReactDOM.createRoot(domElement).render(group);
```