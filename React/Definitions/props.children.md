A special property in react that allows components to render the content that is passed between their opening and closing tags


```jsx
function Link(props) {
  return (
    <p>
      <a href={props.url}>{props.children}</a>
    </p>
  );
}
```