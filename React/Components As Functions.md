# Considerations:
## return statements need to be in between () if it doesn't appear in the same line as the return call

```jsx
const App = () => {
    return (
      <Fragment>
        <Link />
        <Link />
        <Link />
      </Fragment>
    );
}

const App = () => {
    return <Fragment> // Easier to write but now the first Fragment is harder to read
        <Link />
        <Link />
        <Link />
      </Fragment>;
}

const message = ( // Same use with variables
	<main>
	<h1>Hello world</h1>
	</main>
);
```