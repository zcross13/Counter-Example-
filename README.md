# Counter-Example-
Markdown for explaining react counter logic


# State 
we have a state which is storing the count 

# Functions
we have a function called handleclick with add 1 to our state value 

# Action
when a user clicks the button the state is updated by one each time 
the counter update separately 

```js 
import { useState } from 'react';

function MyButton() {
  const [count, setCount] = useState(0);

  function handleClick() {
    setCount(count + 1);
  }

  return (
    <button onClick={handleClick}>
      Clicked {count} times
    </button>
  );
}

export default function MyApp() {
  return (
    <div>
      <h1>Counters that update separately</h1>
      <MyButton />
      <MyButton />
    </div>
  );
}
```
