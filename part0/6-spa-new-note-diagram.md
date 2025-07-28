# 0.6: New note in Single page app diagram

```mermaid
sequenceDiagram
    autonumber
    participant browser
    participant server

    browser ->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    Note right of browser: {content: "test1", date: "2025-07-28T21:23:26.168Z"}
    Note left of server: {"message":"note created"}
    server -->> browser: 201 Created
    deactivate server
```
