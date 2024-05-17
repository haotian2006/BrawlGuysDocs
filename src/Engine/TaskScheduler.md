
# TaskScheduler
A Task Scheduler for handling game loops

#### status: <span style="color:yellow;">Working On</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    haotian - got a working system
```
### <span style="color:lightgreen;">Notes:</span>
```diff
 3/13/2024 Class was created
```
### <span style="color:red;">Bugs:</span>
```diff
```

# <span style="color:green;">Fields</span>

### clockHZ - `int`
`private` 

how fast should the clock run

### PreRender - `Event<Double>`
`public` | `final`

Event that is triggered before rendering

### PreSimulation - `Event<Double>`
`public` | `final`

Event that is triggered before the simulation loop

### PostSimulation - `Event<Double>`
`public` | `final`

Event that is triggered after the simulation loop

## <span style="color:yellow;">Methods</span>

### TaskScheduler(engine `World`)
`protected`

Creates an initializes the loop for the current engine

### TaskScheduler(Engine engine, int clockHZ)
`public`

Creates an initializes the loop for the current engine with a specified clock rate

### pause()
`public`

Stops the loop from running

### resume()
`public`

Resumes the loop from running

### stop()
`public`

Stops the loop from running and closes the thread

## <span style="color:green;">Constructors</span>

### TaskScheduler(Engine engine)
`protected`

Creates an initializes the loop for the current engine

### TaskScheduler(Engine engine, int clockHZ)
`public`

Creates an initializes the loop for the current engine with a specified clock rate

