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
`private` 

Is the current player also the local Player

### IsBot - `boolean`
`private` 

Is the player is a bot

### Wins - `int`
`public`

How many wins the Player has

### Name - `String`
`private`

Name of the player

### Team - `String`
`private`

The Team which the player is on


## <span style="color:yellow;">Methods</span>

### createLocal() -> `Player`
`public` | `static`

creates a a new player with isLocalPlayer field set to true 

### Player() -> `Player`

constructs an abstract player

### createBot() -> `player`
`public` | `static`

creates a Player with the bot field set to true

### getBrawler() -> `Brawler`

This will return the current Brawler the person is using

### setBrawler(brawler `Brawler`)

Sets the Brawler and update camera if it a local 

### getName() -> `String`
`public`

returns the name of the Player

### setName() -> `boolean`
`public`

sets the name of the player, returns true if successful

### getTeam() -> `String`
`public`

returns the team of the Player

### setTeam() -> `void`
`public`

sets the team of the player

### isBot() -> `boolean`
`public`

returns if the player is a bot

### isLocal() -> `boolean`
`public`

returns if the player is the local player

