## for...of + .entries()
Returns an array of \[key, value\] pairs arrays
```jsx
for (const [key, value] of Object.entries(obj)) {
    console.log(key, value);
}
```
## for...in

```jsx
for (const key in obj) {
    console.log(key);  // logs the key
    console.log(obj[key]);  // logs the value associated with the key
}
```
## Object.keys()
Returns array of keys
## Object.values()
Returns array of values