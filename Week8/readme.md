# Week 8: Understanding `useEffect` and Fetch API in React

## Overview

This week, we focus on two key concepts in React:

1. `useEffect` hook for handling side effects.
2. Fetch API for making HTTP requests.

## 1. The `useEffect` Hook

### What is `useEffect`?

The `useEffect` hook allows you to perform side effects in functional components. Common side effects include fetching data, updating the DOM, setting up subscriptions, or performing cleanup.

### Basic Syntax

```javascript
import { useEffect } from 'react';

useEffect(() => {
  // Your side effect logic here
}, [dependencies]);
```

### Key Points

- **Callback Function**: Runs every time the component renders.
- **Dependencies Array**: Controls when the effect should run.
  - Empty `[]`: Runs only once after the initial render.
  - With dependencies `[value]`: Runs on the initial render and whenever `value` changes.
  - No dependencies: Runs after every render.

### Example

```javascript
import { useEffect, useState } from 'react';

function ExampleComponent() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log("Effect runs on every count update.");
  }, [count]);

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </div>
  );
}
```

## 2. Fetch API for HTTP Requests

### What is the Fetch API?

The Fetch API is a modern, promise-based tool for making HTTP requests, built directly into JavaScript. It is commonly used for basic data fetching.

### Basic Syntax

```javascript
fetch(url)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error("Error:", error));
```

### Fetching Data with `useEffect`

`useEffect` is often used to fetch data when a component loads.

#### Example: Fetching Pokémon Data with an Input Parameter

Using the PokeAPI, we can fetch data for a Pokémon based on its ID provided as an input:

```javascript
import { useEffect, useState } from 'react';

function PokemonFetcher() {
  const [id, setId] = useState(1);
  const [pokemonData, setPokemonData] = useState(null);

  useEffect(() => {
    if (id) {
      fetch(`https://pokeapi.co/api/v2/pokemon/${id}`)
        .then(response => response.json())
        .then(data => setPokemonData(data))
        .catch(error => console.error("Error fetching data:", error));
    }
  }, [id]); // Runs whenever the id changes

  return (
    <div>
      <h1>Pokémon Data for ID "{id}":</h1>
      <input
        type="number"
        value={id}
        onChange={(e) => setId(e.target.value)}
        placeholder="Enter Pokémon ID"
      />
      {pokemonData ? (
        <div>
          <p>Name: {pokemonData.name}</p>
          <img src={pokemonData.sprites.other["official-artwork"].front_default} alt={pokemonData.name} />
        </div>
      ) : (
        <p>Enter a Pokémon ID to get data!</p>
      )}
    </div>
  );
}
```

### Fetching with Async/Await in `useEffect`

Using async/await can improve readability when working with `useEffect`.

```javascript
useEffect(() => {
  const fetchData = async () => {
    try {
      const response = await fetch(`https://pokeapi.co/api/v2/pokemon/${id}`);
      const data = await response.json();
      setPokemonData(data);
    } catch (error) {
      console.error("Error:", error);
    }
  };
  if (id) {
    fetchData();
  }
}, [id]);
```

## Tips for Using `useEffect` and Fetch API Together

- **Avoid Infinite Loops**: Ensure dependencies are set correctly to prevent continuous re-rendering.
- **Handle Cleanup**: Always return a cleanup function when using subscriptions or intervals.
- **Error Handling**: Use `.catch()` for handling errors in promises or try/catch with async/await.

---

By integrating `useEffect` with the Fetch API, you can effectively manage side effects and handle data fetching in your React applications.

