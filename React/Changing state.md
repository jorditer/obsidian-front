## Changing arrays

Use spread syntax and add the item
```jsx
  const [cart, setCart] = useState([]);
  const addItem = (item) => {
    setCart(() => [item, ...cart])
   };
```

## Changing objects

To be used as a variable instead of a regular key name, `name` must be inside brackets [];
```jsx
  const [formState, setFormState] = useState({});
  const handleChange = ({ target }) => {
    const { name, value } = target;
    setFormState((prev) => ({
      ...prev,
      [name]: value
    }));
  };
```

## [[Effects]]