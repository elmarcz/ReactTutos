<p align="center">
<a target="blank"><img src="https://kozub.com.ar/wp-content/uploads/2021/01/What-is-an-API.png" width="360" alt="Dot Logo" /></a>
</a>
<h1 align="center">Make an HTTP request to an api</h1>
<p align="center">Now I am going to show you how to make an http request to an api
</p>

## 🔍 What is an Api?
It is an interface that facilitates communication between two different systems or platforms, allowing the addition of various functions to websites and applications.

## 💻 Code
The variable characters has stored all the content of the response.
```jsx
const [characters, setCharacter] = React.useState([]);

React.useEffect(() => {
    getData('https://rickandmortyapi.com/api/character');
}, []);

async function getData(url) {
    const fetchData = await fetch(url);
    const data = await fetchData.json();
    setCharacter(data.results);
}
```

## ⚡ Example
```jsx
function Characters() {
    const [characters, setCharacter] = React.useState([]);

    React.useEffect(() => {
        getData('https://rickandmortyapi.com/api/character');
    }, []);

    async function getData(url) {
        const fetchData = await fetch(url);
        const data = await fetchData.json();
        setCharacter(data.results);
    }

    return ({
                characters.map(character) => {
                    return (
                        <div key={character.id}>
                            <h2>{character.name}</h2>
                            <img src={character.img} />
                        </div>
                    )
                }
    })
}
```

### 🎈 Return to main page
- [Click](https://github.com/elmarcz/ReactTutos)

