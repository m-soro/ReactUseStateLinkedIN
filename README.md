# React useState

```jsx
/**
 * ---------
 * USESTATE
 * ---------
 */
import "./App.css";
import { useState } from "react";

function App() {
  const [checked, setChecked] = useState(false);

  return (
    <div className="App container">
      <h1>useState</h1>
      <input
        type="checkbox"
        value={checked}
        onChange={() => setChecked((checked) => !checked)}
      />
      <label htmlFor="checked">{checked ? "Checked" : "Not Checked"}</label>
    </div>
  );
}

export default App;
```
