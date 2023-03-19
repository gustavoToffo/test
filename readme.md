```mermaid

graph LR;
  Form-->|Click on submit button|Browser;
  Browser-->|POST: Send input|Server;
  Server-->|Respond with 302/URL redirect|Browser;
