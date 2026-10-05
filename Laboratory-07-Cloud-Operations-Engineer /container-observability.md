# Container Observability

## Checkpoint 4: Application Logging

**404 error log line:**

```
172.17.0.1 - - [05/Oct/2026:14:44:32 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs record exactly what a server did and when, including the requested path, the response code, and the client that made the request. This lets an engineer trace a failure back to its cause, such as the missing page above, instead of guessing what went wrong.



## Checkpoint 5: Real-Time Container Metrics

Metrics for the `client-website` container at the time of the screenshot:

| Metric | Value |
|--------|-------|
| CPU % | 0.00% |
| Memory Usage | 2.742MiB (of 1.859GiB limit, 0.14%) |

