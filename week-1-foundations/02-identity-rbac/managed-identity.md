## Failure: Managed Identity Auth Error

### Scenario
Containerized workload failed to authenticate to Azure OpenAI using Managed Identity.

### Impact
- Application startup failure
- API calls blocked

### Detection
- Logs showed token acquisition errors
- No requests reached Azure OpenAI

### Root Cause
- Missing RBAC role: Cognitive Services OpenAI User

### Mitigation
- Assigned correct RBAC role at resource scope
- Verified identity via Azure CLI

### Lesson
Identity-first design eliminates secrets but requires precise RBAC configuration.
