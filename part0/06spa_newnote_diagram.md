## 0.6 Carregando nova nota (Página SPA)

```mermaid
    sequenceDiagram
        participant Browser
        participant Server

        Browser->>Server: POST request to url https://fullstack-exampleap.herokuapp.com/new_note_spa
        Server-->>Browser: status code 201 created
        Note right of Server: receives only one request

        Note right of Browser: tag Form has no attributes
        Note right of Server: notes disappear when the server is restarted

```