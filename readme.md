```mermaid

graph LR;
  Form-->|Click button|Browser;
  Browser-->|Send input|Server;
  Server-->|Respond with 302/URL redirect|Browser;
