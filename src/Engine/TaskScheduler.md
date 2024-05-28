# TaskScheduler Class
The `TaskScheduler` class provides functionality for scheduling tasks to be executed at specified intervals or delays. It manages the execution of tasks in a loop, ensuring that they are performed in a timely manner.

#### status: <span style="color:green;">Completed</span>
### <span style="color:cyan;">Contributors:</span>
<!-- List contributors and their contributions here. For example: -->

```diff
    Haotian - created class and methods
```

## <span style="color:yellow;">Fields</span>
### clockHZ `final int`
Represents the frequency of the task scheduler's clock in Hertz.

### loop `ScheduledExecutorService`
A scheduled executor service used for executing tasks at specified intervals.

### timePassed `long`
Tracks the time passed since the task scheduler started.

### preRenderTime, preSimulationTime, postSimulationTime, simulationTime `long`
Variables used for measuring time intervals during the rendering and simulation phases.

### isLooping `boolean`
Indicates whether the task scheduler is currently executing tasks.

### taskStack `Stack<Task>`
A stack used for temporarily storing tasks while the scheduler is looping.

### tasksPQ `PriorityQueue<SchedulerTask>`
A priority queue used for storing tasks based on their scheduled delay.

### taskList `ArrayList<SchedulerTask>`
`deprecated`

An array list used for storing tasks in order of their scheduled delay.

## <span style="color:yellow;">Methods</span>

### pause()
`public`

Pauses the execution of tasks by setting the `running` flag to `false`.

### resume()
`public`

Resumes the execution of tasks by setting the `running` flag to `true`.

### stop()
`public`

Stops the task scheduler, shutting down the loop executor service.

### scheduleTask(seconds `double`, x `lambda`)
`public`

Schedules a task to be executed after a specified delay in seconds. The `lambda` represents the action to be performed.

### scheduleTask(seconds `double`, x `Consumer<T>`, data `T`)
`public`

Schedules a task to be executed after a specified delay in seconds, passing additional data of type `T` to the consumer function `x`.

### scheduleForEachTask(seconds `double`, data `T[]`, x `Consumer<T>`)
`public`

Schedules a task to iterate over each element in the `data` array, executing the consumer function `x` for each element after a specified delay in seconds.

### scheduleForTask(seconds `double`, iterations `int`, x `Consumer<Integer>`)
`public`

Schedules a task to execute the consumer function `x` for a specified number of iterations after a delay of `seconds` seconds.

