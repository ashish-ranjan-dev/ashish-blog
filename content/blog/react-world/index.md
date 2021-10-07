---
title: React
date: "2021-10-06T23:46:37.121Z"
---

## First lets see a code in react

```js
import React, { useState } from "react"

export default function App() {
  const [clicked, setclicked] = useState(0)
  function ButtonClickHandlerAdd() {
    setclicked(clicked + 1)
  }
  function ButtonClickHandlerSub() {
    setclicked(clicked - 1)
  }
  return (
    <div className="App">
      <div className="Clicks">
        <div>{clicked}</div>
        <button onClick={ButtonClickHandlerAdd}>Add</button>
        <button onClick={ButtonClickHandlerSub}>Subtract</button>
      </div>
    </div>
  )
}
```

> in the above code we used states to update the value of **clicked** variable.

## Lets add some css to our code

```css
.App {
  font-family: sans-serif;
  text-align: center;
}

* {
  margin: 0;
}

.Clicks {
  margin: 30%;
}

button {
  width: 5rem;
}
```

> You can see the current progress [here](https://codesandbox.io/s/react-1-ridyc?file=/src/App.js)
