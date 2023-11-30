In React, handling events is similar to handling events in standard HTML elements but with some differences due to the use of JSX and the synthetic event system provided by React. Below is an example demonstrating how to handle events in React:

```javascript
import React, { useState } from 'react';

const EventHandlingExample = () => {
  const [count, setCount] = useState(0);

  // Event handler function for button click
  const handleClick = () => {
    setCount(count + 1); // Update the count state
  };

  return (
    <div>
      <h2>Event Handling in React</h2>
      <p>Count: {count}</p>
      {/* Button triggering the handleClick function */}
      <button onClick={handleClick}>Increase Count</button>
    </div>
  );
};

export default EventHandlingExample;
```

In this example:

- We use the `useState` hook to initialize and manage the state of `count`.
- There's a `handleClick` function that updates the `count` state when the button is clicked. The `onClick` attribute is used to assign this function to the button's click event.

This is a basic example of handling events in React. React uses synthetic events to wrap the native browser events, providing a consistent interface and handling differences across browsers.

You can handle various events such as `onClick`, `onChange`, `onSubmit`, etc., in a similar manner by providing appropriate event handler functions to the respective event attributes in JSX.

Remember to handle events in React by using camelCase event names (`onClick`, `onChange`) rather than lowercase HTML event names (`onclick`, `onchange`). Also, ensure that event handlers are assigned functions (not function calls) to avoid unintentional invocation.
