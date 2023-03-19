```mermaid

sequenceDiagram
    participant browser
    participant server
    participant form

    browser->>server: Click "Submit" button
    activate browser
    server->>browser: HTTP 302/URL redirect
    deactivate browser
    browser->>server: POST form data
    activate browser
    server->>browser: HTTP response
    deactivate browser
