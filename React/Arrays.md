
## Inside JSX
You can insert array of objects in JSX and they will render directly
```jsx
const images = [];

for (const animal in animals) {
  images.push(
    <img
    key={animal}
    className='animal'
    alt={animal}
    src={animals[animal].image}
    aria-label={animal}
    role='button'
    />
  )
}
const animalFacts = 
<div>
  {background}
  <div className='animals'>
  {images}
  </div>
  <h1>{title ? title : 'Click an animal for a fun fact'}</h1>
</div>
```
Or more clearly:
```jsx
let num = 0;
const animals = [<h3 key={num++} >Dog</h3>, <h3 key={num++}>Cat</h3>, <h3 key={num++}>Fish</h3>]

const App () => {
    return <div>{animals}</div>;
}
```
Usually is easier to use .map:
```jsx
class App extends Component {
  render() {
    const list = [
      { breed: "Chihuahua", description: "Small breed of dog." },
      { breed: "Corgi", description: "Cute breed of dog." },
      { breed: "Cumberland Sheepdog", description: "Extinct breed of dog." },
    ];
    return <Breeds list={list} />;
  }
}

class Breeds extends Component {
  render() {
    return (
      <dl>
        {this.props.list.map(({ breed, description }) => (
          <Fragment key={breed}>
            <dt>{breed}</dt>
            <dd>{description}</dd>
          </Fragment>
        ))}
      </dl>
    );
  }
}
```
[[Looping arrays]]