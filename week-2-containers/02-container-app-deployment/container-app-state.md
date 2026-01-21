## Failure: Container App Running but Not Reachable

### Scenario
Azure Container App showed "Running" status but could not be accessed via public endpoint.

### Impact
- Application unavailable
- Misleading health status

### Detection
- No response from public URL
- Logs showed container running normally

### Root Cause
- Ingress target port did not match container listening port

### Mitigation
- Aligned container listening port with ACA ingress target port
- Redeployed revision

### Lesson
Platform health ≠ application reachability. Networking alignment is critical.
