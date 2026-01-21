### Failure: HTTP 429 Throttling

### Symptoms

Intermittent failures

Latency spikes

Partial responses

### Cause

Token or request rate limits exceeded

### Detection

Application logs show 429 responses

Usage metrics spike

### Mitigation

Implement retries with exponential backoff

Limit concurrency

Gracefully degrade user responses

### Lesson

AI failures propagate fast if not controlled.


### Failure: Cost Amplification

### Symptoms

Unexpected cost increase

### Cause

Retry storms

Over-scaling

Inefficient prompt usage

### Detection

Azure Cost Management alerts

Token usage metrics

### Mitigation

Set budgets and alerts

Cap retries

Monitor token usage per request

### Lesson

Cost is a reliability concern in AI platforms.