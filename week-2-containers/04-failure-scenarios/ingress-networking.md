## Failure: Requests Hang or Time Out

### Symptoms

Client requests never complete

No application logs are generated

Container appears healthy

### Common Causes

DNS resolution issues

Misconfigured ingress

Wrong container port exposed

### Detection

ACA revision shows Running

No incoming request logs

Azure Monitor shows zero request metrics

### Mitigation

Validate container listening port matches ACA configuration

Explicitly expose the correct target port

Test locally before deployment

### Lesson

A healthy container does not guarantee a reachable service.