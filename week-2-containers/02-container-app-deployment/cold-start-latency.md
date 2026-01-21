## Failure: Cold Start Latency

### Scenario
First request to container app after idle period experienced high latency.

### Impact
- Poor user experience
- Perceived outage

### Root Cause
- Container App scaled to zero
- Dependency initialization delay

### Mitigation
- Configured minimum replicas for latency-sensitive workloads
- Documented trade-off between cost and responsiveness

### Lesson
Serverless convenience requires conscious latency trade-offs.
