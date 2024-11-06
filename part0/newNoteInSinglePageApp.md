```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server

    User->>Browser: Enter note and click Save
    Browser->>Server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa with note data
    activate Server
    Server-->>Browser: 201 Created
    deactivate Server
    Browser->>User: Add new note to page without reloading
```


