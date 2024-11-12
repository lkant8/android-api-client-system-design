# System Design for software 

## 1 Andrfoid own Api client using okhttp abastraction layer 
```
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
Ui path 
<img src="https://raw.githubusercontent.com/lkant8/android-api-client-system-design/main/assets/System Design for Android API Client.drawio.png" width="360" height="640">
