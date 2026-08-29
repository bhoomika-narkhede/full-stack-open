```mermaid
    sequenceDiagram
    participant User
    participant Browser
    participant Server

    User->>Browser: Enter note text
    User->>Browser: Click Save
    Browser->>Server: POST /new_note_spa
    Server-->>Browser: 201 Created
    Browser->>Browser: Add the new note to the page
    Browser-->>User: Display the new note
```
