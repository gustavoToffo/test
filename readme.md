```mermaid

sequenceDiagram
    participant browser
    participant server
    participant form

    browser->>form: Click "Submit" button
    activate form
    form->>browser: Send user input
    deactivate form
    browser->>server: HTTP POST request to new_note
    activate browser
    server->>browser: HTTP 302/URL redirect to notes
    deactivate browser
    browser->>server: HTTP GET request for main.css
    activate browser
    server->>browser: main.css file
    deactivate browser
    browser->>server: HTTP GET request for main.js
    activate browser
    server->>browser: main.js file
    deactivate browser
    browser->>server: HTTP GET request for data.json
    activate browser
    server->>browser: data.json file
    deactivate browser
