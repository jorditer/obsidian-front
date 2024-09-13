## Default values

You can put them inside the function arguments:

```jsx
function Example({text='This is default text'}) {
   return <h1>{text}</h1>
}
```
Or in the body
```jsx
function Example(props) {
  const {text = 'This is default text'} = props;
  return <h1>{text}</h1>
}
```
Or static properties
```jsx
function Example(props) {  
  return <h1>{props.text}</h1>  
}  
  
Example.defaultProps = {  
  text: 'This is default text',  
};
```