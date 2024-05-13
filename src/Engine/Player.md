# Player


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

### Brawler - `Brawler`

What brawler is the Player controlling 

### IsLocalPlayer - `boolean`
`public` | `final`

Is the current player also the local Player


### Name - `String`
`private`

Name of the player


## <span style="color:yellow;">Methods</span>

### Player(IsLocal `boolean`) -> `Player`

creates a new Abstract player and set IsLocal

### Player() -> `Player`

constructs an abstract player

### getBrawler() -> `Brawler`

This will return the current Brawler the person is using

### setBrawler(brawler `Brawler`)

Sets the Brawler and update camera if it a local 

### getName() -> `String`
`public`

returns the name of the Player

### setName() -> `Boolean`
`public`

sets the name of the player, returns true if successful