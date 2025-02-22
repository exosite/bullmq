<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bullmq](./bullmq.md) &gt; [Scripts](./bullmq.scripts.md) &gt; [reprocessJob](./bullmq.scripts.reprocessjob.md)

## Scripts.reprocessJob() method

Attempts to reprocess a job

<b>Signature:</b>

```typescript
static reprocessJob(queue: MinimalQueue, job: Job, state: 'failed' | 'completed'): Promise<void>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  queue | [MinimalQueue](./bullmq.minimalqueue.md) |  |
|  job | [Job](./bullmq.job.md) |  |
|  state | 'failed' \| 'completed' |  |

<b>Returns:</b>

Promise&lt;void&gt;

Returns a promise that evaluates to a return code: 1 means the operation was a success 0 means the job does not exist -1 means the job is currently locked and can't be retried. -2 means the job was not found in the expected set

