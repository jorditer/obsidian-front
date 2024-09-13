## for...of "+ .entries() 

```jsx

for (const [index, value] of arr.entries()) {
    console.log(`Index: ${index}, Value: ${value}`);
}
```
## .forEach()

```jsx
arr.forEach((value, index) => {console.log(`Index: ${index}, Value: ${value}`);});
```
## for...of

```jsx
for (const value of arr) {
    console.log(value);
}
```