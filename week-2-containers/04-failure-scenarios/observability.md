### Failure: Logs or Metrics Missing

### Symptoms

No data in Log Analytics

### Cause

Diagnostics not enabled

Logs not written to stdout/stderr

### Mitigation

Enable diagnostics explicitly

Log structured messages at startup and dependency calls

### Lesson

If you can’t observe failure, you can’t fix it.