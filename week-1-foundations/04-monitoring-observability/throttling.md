## Failure: Azure OpenAI 429 Throttling

### Scenario
When sending multiple concurrent requests to Azure OpenAI, the service returned HTTP 429 (Too Many Requests).

### Impact
- Increased latency
- Partial request failures
- Potential cascading retries

### Detection
- Azure Monitor metrics showed request spikes
- Application logs captured repeated 429 responses

### Root Cause
- Token throughput limits exceeded
- No client-side backoff logic

### Mitigation
- Implemented exponential backoff
- Limited concurrent requests
- Monitored usage via Azure Monitor metrics

### Lesson
AI services behave like shared platforms. Throttling must be expected and designed for.
