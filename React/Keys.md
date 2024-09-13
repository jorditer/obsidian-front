## Using .map()
When using .map() and an i parameter so that you can access each element unique index.
```jsx
const peopleList = people.map((person,i) =>
  // expression goes here:
  <li key={'person_' + i}>{person}</li>
);
```