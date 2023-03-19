```mermaid

graph LR;
  Form-->|Click button|Browser;
  Browser-->|POST: Send input|Server;
  Server-->|Respond with 302/URL redirect|Browser;
