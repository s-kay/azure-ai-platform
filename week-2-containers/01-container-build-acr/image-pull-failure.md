## Failure: Image Pull Denied from Azure Container Registry

### Scenario
Container App failed to start due to denied access when pulling image from ACR.

### Impact
- App failed during startup
- No replicas created

### Detection
- Container App logs showed image pull errors

### Root Cause
- Missing AcrPull role assignment for Managed Identity

### Mitigation
- Assigned AcrPull role
- Redeployed container app

### Lesson
Registry access must be explicitly granted in identity-based designs.
