# Signal `<T>` 
A simple Signal Class

#### status: <span style="color:Green;">Done</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    Haotian - Finished signal and its sub classes
```
### <span style="color:lightgreen;">Notes:</span>
```diff
    4/12/24 - Finished Signal and Connection
    4/13/24 - await was added
```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### Connections - `List<Connection<T>>`
Contains a List of connections

## <span style="color:yellow;">Methods</span>


### connect(callBack `Consumer <T>`) -> `Connection`
`public`

creates a connection and stores it

### await() -> `T`
`public`

yields until the next time the signal is fired, returns Value.

### fire(value`T`) -> `void`
`public`

invokes all the connections

### fire(value`T`) -> `void`
`public`

invokes all the connections

### disconnectAll() -> `void`
`public`

disconnects All Connections

### disconnectConnection(connection `Connection`)
`private`

disconnects the given Connection

