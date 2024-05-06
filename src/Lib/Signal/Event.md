# Event
`Interface`
A helper class for signal
## <span style="color:green;">Fields</span>

## <span style="color:yellow;">Methods</span>

### connect(callBack `Consumer<T>`) -> `connection`
`public`

Connects the lambda to the signal

### await() -> `T`
`public`

yields until the next time the signal is fired, returns Value.

### once(callBack `Consumer<T>`) -> `connection`
`public`

Fires the call back once and disconnects