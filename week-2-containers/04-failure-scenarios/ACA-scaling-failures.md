### Failure: Cold Start Latency

Symptoms

### First request takes several seconds

Subsequent requests are fast

### Cause

Container scaled to zero

Image needs to be pulled and started

### Detection

Metrics show replica count scaling from 0 → 1

Latency spike on first request

### Mitigation

Set minimum replicas to 1 for latency-sensitive workloads

Use warm-up endpoints if needed

### Lesson

Scale-to-zero saves cost but increases perceived downtime.