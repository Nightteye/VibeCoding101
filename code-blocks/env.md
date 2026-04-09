# .env file
VITE_API_KEY=abc123xyz
VITE_API_URL=https://api.example.com

# Using environment variables in your React app
```jsx
import React from 'react';
function App() {       
  const apiKey = import.meta.env.VITE_API_KEY;
  const apiUrl = import.meta.env.VITE_API_URL;
    return (
        <div>
        <h1>API Key: {apiKey}</h1>
        <h2>API URL: {apiUrl}</h2>  
        </div>
    );
}
export default App;
``` 