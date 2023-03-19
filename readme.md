```mermaid

sequenceDiagram
  participant Form
  participant Browser
  participant Server
  Form->>+Browser: User clicks on "Submit" button
  Browser->>+Server: POST form data 
  Server-->>-Browser: Respond with status 302/URL redirect
