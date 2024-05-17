# IdGenerator
A class that can generate an number thats unique in its state.

#### status: <span style="color:Red;">Not Started</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
Joey
```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### LOWEST_VALUE - `int`
`private` | `static` 

Should hold the lowest value that should be in the Queue until it should be used. Set to 50 for now

### currentIndex - `short`
`private`

Holds the current Index that is available. Should start with the smallest Integer value possible of -2147483648

### holder- `Queue<Integer>`
`private`

Holds all ids that are not being used.

## <span style="color:yellow;">Methods</span>

### push(id `short`)
`public` 

Pushes the id into the queue 


### getNext() -> `short`
`public`

Returns the next Short id that can be used. If the `holder` size is below `LOWEST_VALUE` or the `holder` is empty increment `currentIndex` and return it, else if the `holder` isn't empty and `currentIndex` is above `LOWEST_VALUE` then pop and return the value in `holder`.

