## 0.4 Carregando nova nota na página

```mermaid
    sequenceDiagram
        participant Browser
        participant Server

        Browser->>Server: POST request to url https://fullstack-exampleap.herokuapp.com/new_note
        Server-->>Browser: HTTP 302

        Note right of Browser: reloads webpage

        Browser->>Server: Requests CSS, JS and JSON files through HTTP

        Note right of Server: notes disappear when the server is restarted

```
