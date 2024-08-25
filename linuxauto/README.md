## Invoking another process P2 while the process P1 reaches certain state
This can be used to collect telemetry while a workload reaches its maximum or intented usage

Wait for certain string to be printed in a log file 

**Note: To be explained further**
1. Execute P1
2. Use below command in another teminal for waiting and running P2 on an event

```
tail -n0 -f <log file> | sed '/<String to be logged in in the log file waited upon>/ q' ; <command to execute P2>
```
