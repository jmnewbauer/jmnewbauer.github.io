```mermaid
sequenceDiagram
  participant Attacker
  participant BotNet
  participant Firewall
  participant WebServer
  

    Attacker->>BotNet: Controls the Botnet
    BotNet->>WebServer: Send many Requests
    Firewall->>WebServer: Tries to block as many requests as it can
    WebServer->>WebServer: Overwhelmed by Excessive Traffic and crashes
    

```

The Attacker wants to bring down the WebServer so they send out many requests through a BotNet. The Firewall does what it can to minimize the amount of requests but the WebServer is ultimately overwhelmed and crashes.
