## &&
If the expression on the left is true the JSX on the right will be rendered. If not it will be ignored
```jsx
  <ul>
    <li>Applesauce</li>
    { !baby && <li>Pizza</li> }
    { age > 15 && <li>Brussels Sprouts</li> }
    { age > 20 && <li>Oysters</li> }
    { age > 25 && <li>Grappa</li> }
  </ul>
);
```
## Ternary

```jsx
const img = <img src={pics[coinToss() === 'heads' ? 'kitty' : 'doggy']} />;
```

## ||
If the expression on the left is not rendered (in this case because it may call a key value that doesn't exist) it renders the expression on the right.

```jsx
const status2icon = {
draft: <DraftIcon />,
published: <PublishedIcon />,
};

function Component(props) {
return status2icon[props.status] || status2icon.deleted; 
} 
```