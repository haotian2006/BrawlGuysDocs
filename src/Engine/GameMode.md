# GameMode
`abstract`

This handles the game during runtime


#### status: <span style="color:Red;">Not Started</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff

```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```


## <span style="color:green;">Fields</span>

### engine - `Engine`
`public` | `final`

The current Engine

### scoreBoard - `String`
`public`

What should the score board say

## <span style="color:yellow;">Methods</span>

### GameMode(Engine engine)

Initializes the Entities.

### setScoreBoard(String s)
`public`

Sets the score board 

### update(float delta) -> `void`
`public`

Defines what should be happing during the game

### destroy() -> `void`
`public`

Destroys the game mode