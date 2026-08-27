    User->>Browser: Types a note and clicks Save
    Browser->>Server: POST /new_note
    Note right of Browser: The note is sent in the request body

    Server->>Server: Saves the new note
    Server-->>Browser: HTTP 302 Redirect to /notes

    Browser->>Server: GET /notes
    Server-->>Browser: HTML page

    Browser->>Server: GET /main.css
    Server-->>Browser: CSS

    Browser->>Server: GET /main.js
    Server-->>Browser: JavaScript

    Browser->>Server: GET /data.json
    Server-->>Browser: Updated notes

    Browser->>Browser: Displays the new note
