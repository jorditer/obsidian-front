## useEffect()

### Array whith dependencies
The dependency array (\[count\]) makes the effect only take place when there are changes in the variable.
```jsx
useEffect(() => {
  alert(count);
}, [count]);
```

### Empty Array 
Forces useEfect to only render the effect once
```jsx
    useEffect(() => {
      const intervalId = setInterval(() => setTime((prevTime) => prevTime + 1), 1000);
      return () =>{
      clearInterval(intervalId)
      } 
    }, [])
```
## [[Cleanup]]