## Event listeners
```jsx
useEffect(()=>{
  document.addEventListener('keydown', handleKeyPress);
  // Specify how to clean up after the effect:
  return () => {
    document.removeEventListener('keydown', handleKeyPress);
  };
})
```
\
### Intervals

```jsx
    useEffect(() => {
      const intervalId = setInterval(() => setTime((prevTime) => prevTime + 1), 1000);
      return () =>{
      clearInterval(intervalId)
      } 
    }, [])
```