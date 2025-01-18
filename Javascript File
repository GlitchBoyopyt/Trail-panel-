import React, { useEffect, useState } from 'react';

function App() {
    const [servers, setServers] = useState([]);

    useEffect(() => {
        fetch('http://localhost:8000/api/servers') // Adjust the URL as needed
            .then(response => response.json())
            .then(data => setServers(data.servers));
    }, []);

    return (
        <div>
            <h1>Game Servers</h1>
            <ul>
                {servers.map((server, index) => (
                    <li key={index}>{server}</li>
                ))}
            </ul>
        </div>
    );
}

export default App;
