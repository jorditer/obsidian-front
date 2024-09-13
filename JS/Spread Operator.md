
## Arrays

```jsx
const arr1 = [1, 2, 3];
const arr2 = [0, ...arr1, 4]; // [0, 1, 2, 3, 4]
const arr3 = [...arr1] // Duplicates arr1
```

## Objects

```jsx
const obj1 = {a: 1, b: 2};
const obj2 = {c: 3, d: 4};
const obj3 = {...obj1, ...obj2}; //merges obj1 & obj2 into obj3
const obj4 = {...obj1, a: 0} //
```
