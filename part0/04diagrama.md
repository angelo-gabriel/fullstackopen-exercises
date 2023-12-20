## 0.4 Carregando nova nota na página

```mermaid
    sequenceDiagram
    Browser->>Server: POST request to url https://fullstack-exampleap.herokuapp.com/new_note
    Server-->>Browser: HTTP 302
    Note right of browser: reloads webpage
    Broser->>Server: Requests CSS, JS and JSON files through HTTP
    Note right of server: notes disappear when the server is restarted

```
