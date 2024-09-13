## First set the state in the parent component
```jsx
const [items, setItems] = useState([
	{name: "Apple", id: 1, num: 0},
	{name: "Pear", id: 2, num: 0},
	{name: "Peach", id: 3, num: 0},
])
const handleRemoveItems = id => {
	setItems => previous.filter(i => i.id !== id)
}
const handleNumChange = (id, delta) => {
	setItems(items.filter(prevItems => prevItems.map(items = {
		if (items.id === id) {
			return {// if id matches return the same component but with num + delta 
				name: item.name,
				num: item.num + delta,
				id: item.id
			}
		}
		return player; // like an else
	})))
}
return (
{items.map() => {
	<Button handleRemove={handleRemoveItems} id={item.id} butName={item.name} />
})}
```
## Then call the function as a prop in the children using an anonymous function
```jsx
const Children = (props) => {
	return (
		<button onClick={() => props.handleRemove(props.id)} />
		<button onClick={() => props.changeScore(props.id, -1)} />
		<button onClick={() => props.changeScore(props.id, 1)} />
		<Counter id = props.id />
	)
}
```

## [[Hooks]]

## [[Changing state]]