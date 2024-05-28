# Coroutine Class

A failed attempt at creating a Coroutine class. Went for taskScheduler.sleep() utilizing method chaining instead.

#### status: <span style="color:green;">done</span>
### <span style="color:cyan;">Contributors:</span>
<!-- List contributors and their contributions here. For example: -->

```diff
    Haotian - created class and methods
```

## <span style="color:yellow;">Fields</span>

### func `Consumer<Void>`
Represents the function to be executed by the coroutine.

### running `boolean`
Indicates whether the coroutine is currently running.

### paused `boolean`
Indicates whether the coroutine is currently paused.

### pauseSignal `Signal<Void>`
A signal used for pausing and resuming the coroutine.

### scheduler `TaskScheduler`
The task scheduler used for scheduling coroutine operations.

## <span style="color:yellow;">Methods</span>

### run()
`public`

Starts the execution of the coroutine by invoking the function provided in the constructor.

### pause()
`public`

Pauses the execution of the coroutine. If the coroutine is already paused, an `IllegalStateException` is thrown.

### pauseFor(time `double`)
`public`

Pauses the execution of the coroutine for a specified duration `time` in seconds.

### resume()
`public`

Resumes the execution of the coroutine. If the coroutine is already running or not paused, an `IllegalStateException` is thrown.

### close()
`public`

Closes the coroutine, stopping its execution.

### isPaused()
`public`

Returns `true` if the coroutine is currently paused; otherwise, returns `false`.

### isRunning()
`public`

Returns `true` if the coroutine is currently running; otherwise, returns `false`.

