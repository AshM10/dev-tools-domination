# dev-tools-domination

This is a solution to the [14 Must Know Dev Tools Tricks](https://javascript30.com). 30 day vanilla JS coding challenge.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

- learn more about developer tools and console

### Screenshot

### Links

- Solution URL: [GitHub](https://github.com/AshM10/dev-tools-domination)

## My process

### What I learned

- Inspect > Find it in your DOM > Break on > Attribute modifications - this will pop a debugger command and it will post exactly where the line of code that is causing that attribute

```js
// Grouping together
dogs.forEach((dog) => {
  console.groupCollapsed(`${dog.name}`);
  console.log(`This is ${dog.name}`);
  console.log(`${dog.name} is ${dog.age} years old!`);
  console.log(`${dog.name} is ${dog.age * 7} dog years old!`);
  console.groupEnd(`${dog.name}`);
});

// timing
console.time("fetching data");
fetch("https://api.github.com/users/AshM10")
  .then((data) => data.json())
  .then((data) => {
    console.timeEnd("fetching data");
    console.log(data);
  });
```

### Continued development

Continue with the 30 day challenge

## Author

- Website - [Ash Moreno](https://www.ashmoreno.dev)
- Twitter - [@sexy_gravy](https://twitter.com/sexy_gravy)
