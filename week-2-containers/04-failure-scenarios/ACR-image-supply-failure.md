### Failure: Image Pull Fails

### Symptoms

Container App revision stuck in Failed

No application startup logs

### Common Causes

Missing AcrPull role assignment

Managed Identity not enabled

Incorrect image tag

### Detection

ACA revision events show image pull errors

Logs indicate authentication failure

### Mitigation

Use Managed Identity instead of admin credentials

Assign AcrPull role at registry scope

Pin known-good image tags

### Lesson

Most startup failures are identity problems, not container problems.