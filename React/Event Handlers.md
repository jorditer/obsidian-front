`onHover`
`onClick`

## Always use arrow functions

If not the function will be called when the component renders instead of when the event is called.
```jsx
onClick={() => setToggle("On")};
```
