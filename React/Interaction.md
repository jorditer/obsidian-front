## Text-fields

```jsx
const AddPlayer = () => {
	const [value, setValue] = useState("");
	
	return (
	<input
		onChange = {event => setValue(event.target.value)} 
		value = {value}
	/>
	)
}
```

## Submit buttons

```jsx
const handleAddPlayer = (name) => {
	setPlayers([
	{
		name: player.name,
		score: player.score + delta,
		id: player.id
	}])
}
<AddPlayer addPlayer={handleAddPlayer};
const AddPlayer = (props) => {
	const [value, setValue] = useState("");

	const handleSubmit = (event) => {
	event.preventDefault(); // If not the submit button would submit the form and reload the page
	props.addPlayer(value);
	}
	
	return (
	<form onSubmit = {(event) => handleSubmit(event)}
	<input
		onChange = {event => setValue(event.target.value)} 
		value = {value}
	/>
	)
}
```

## Truthy conditionals for display

When the user .isVerified, it shows <Checkmark /> if it's not it doesn't show anything as it would be false
```jsx
class UserName extends Component {
	render() {
		return (
			<p>
				{this.props.username}
				{this.props.isVerified && <Checkmark />}
			</p>
		);
	}
}
```
## Using objects to limit options

```jsx
const status2icon = {
	draft: <DraftIcon />,
	published: <PublishedIcon />,
	deleted: <TrashIcon />,
};
class PostStatus extends Component {
	render() {
	return status2icon[this.props.status] || status2icon.deleted;
	}
}
```

## Stack Ternary conditionals

```jsx
class PostStatus extends Component {
	render() {
		return this.props.status === "draft" ?
			<DraftIcon /> :
			this.props.status === "published" ?
			<PublishedIcon /> :
			<TrashIcon />;
	}
}
```