- 👋 Hi, I’m @Uzair-oozy
- 🌱 I’m currently learning C#
- 📫 How to reach me: oozy004@gmail.com


```mermaid
graph TD

    S[Central Server<br>Authentication<br>Message Routing<br>File Management]

    C1[Client 1]
    C2[Client 2]
    C3[Client 3]
    C4[Client 4]

    C1 <-- Chat & File Transfer --> S
    C2 <-- Chat & File Transfer --> S
    C3 <-- Chat & File Transfer --> S
    C4 <-- Chat & File Transfer --> S
```

```mermaid
graph LR

    subgraph Clients
        C1[Client 1]
        C2[Client 2]
        C3[Client 3]
    end

    subgraph Server
        A[Authentication Module]
        M[Message Handling Module]
        F[File Sharing Module]
        DB[(User Records / Logs)]
    end

    C1 --> A
    C2 --> A
    C3 --> A

    A --> M
    A --> F

    M --> DB
    F --> DB
```

```mermaid
flowchart TD

    A([Start])

    B[Server Starts Listening]

    C[Client Connects to Server]

    D[User Authentication]

    E{Authentication Successful?}

    F[Reject Connection]

    G[Client Added to Active Users]

    H{Choose Operation}

    I[Send Chat Message]

    J[Send File]

    K[Server Processes Request]

    L[Deliver Message/File]

    M{Continue Communication?}

    N[Client Disconnects]

    O[Remove Client from Active Users]

    P([End])

    A --> B
    B --> C
    C --> D
    D --> E

    E -- No --> F
    F --> P

    E -- Yes --> G
    G --> H

    H --> I
    H --> J

    I --> K
    J --> K

    K --> L
    L --> M

    M -- Yes --> H
    M -- No --> N

    N --> O
    O --> P
```

```mermaid
graph TB

    Internet[(Network / LAN)]

    Server[Multi-Threaded TCP Server]

    Client1[Client A]
    Client2[Client B]
    Client3[Client C]

    Internet --> Server

    Client1 --> Internet
    Client2 --> Internet
    Client3 --> Internet
```

<!---
Uzair-oozy/Uzair-oozy is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
