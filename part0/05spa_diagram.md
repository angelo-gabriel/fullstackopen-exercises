## 0.5 Página SPA (Single page app)

```mermaid
    sequenceDiagram
        participant Browser
        participant Server
        Note left of Browser: only renders HTML. Executes JavaScript code       

        Browser->>Server: fetches JSON data and adds HTML elements, using DOM-API
        Server-->>Browser: content is manipulated through JS code on the Browser 
        Note right of Server: receives only one request

```