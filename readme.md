```mermaid

sequenceDiagram
  participant Form
  participant Browser
  participant Server
  Form->>+Browser: Click "Submit"
  Browser->>+Server: POST form data
  Server-->>-Browser: Respond with 302/URL redirect
