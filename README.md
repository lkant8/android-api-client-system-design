# System Design for software 

## 1 Andrfoid own Api client using okhttp abastraction layer 
```mermaid
flowchart LR
    A[Client Library] -->|Uses| B[HTTP Client]
    B --> C[HttpURLConnection/OkHttp]
    A --> D[Request Model]
    A --> E[Response Model]
    D --> F[Serialization]
    E --> F[Deserialization]
    A --> G[Error Handling]
    A --> H[Interceptors]
    G --> I[Network Errors]
    G --> J[HTTP Errors]
    G --> K[Timeouts]
    H --> L[Logging Interceptor]
    H --> M[Retry Interceptor]
```
