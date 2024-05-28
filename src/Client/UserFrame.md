# UserFrame
`Extends Frame`

The frame which displays the Player 

![](https://media.discordapp.net/attachments/558866529253589012/1241228834746142772/image.png?ex=66496fef&is=66481e6f&hm=d47c3986f4a4159efff22d87f307a01cdd0cd16394ffcc961b3b2ca8cb101106&=&format=webp&quality=lossless&width=144&height=107)

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

### selected - `bool`
`private`

if the current Frame is being selected

### player - `Player`
`private`

Holds stuff

### sessionManager - `SessionManager`
`public` | `final`

### Other Frames...
`private`

This is stuff like the image Frame, PlayerName Kick button etc (create a field for each one)

## <span style="color:yellow;">Methods</span>

### UserFrame(sessionManager `SessionManager`)

create a User Frame

### setSelected(selected `bool`)
`public` 

Sets the background to green if it is selected else back to default

### setPlayer(player `Player`)
`public`

Sets the player and Updates the frame

### update()
`public`

Updates the information, If player is Null display the + sign else display the player data.

Method
