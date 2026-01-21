### Failure: Token Acquisition Fails

### Symptoms

Requests fail immediately

Errors when calling Azure OpenAI

### Common Causes

Managed Identity missing role assignment

Wrong scope or resource configuration

### Detection

Application logs show authentication or token errors

### Mitigation

Assign Cognitive Services OpenAI User role

Validate identity at runtime using test calls

### Lesson

Identity failures look like application bugs unless logged clearly.