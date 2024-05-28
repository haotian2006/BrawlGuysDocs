
# Task
`Interface`

The `Task` interface defines methods for scheduling tasks to be executed at a later time or in a specific manner. It provides flexibility in task execution, allowing for delays, iteration over collections, and custom actions. Used by TaskScheduler to schedule tasks for execution.

#### status: <span style="color:green;">done</span>
### <span style="color:cyan;">Contributors:</span>
<!-- List contributors and their contributions here. For example: -->
```
    Haotian - created class and methods
```
## <span style="color:yellow;">Methods</span>

### sleep(seconds `double`, x `lambda`)
`public`

Schedules a task to be executed after a specified delay in seconds. The `lambda` represents the action to be performed.

### sleep(seconds `double`, x `Consumer<T>`, data `T`)
`public`

Schedules a task to be executed after a specified delay in seconds, passing additional data of type `T` to the consumer function `x`.

### forEach(seconds `double`, data `T[]`, x `Consumer<T>`)
`public`

Schedules a task to iterate over each element in the `data` array, executing the consumer function `x` for each element after a specified delay in seconds.

### forIter(seconds `double`, iterations `int`, x `Consumer<Integer>`)
`public`

Schedules a task to execute the consumer function `x` for a specified number of iterations after a delay of `seconds` seconds.


