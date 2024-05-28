# PlayScreen 
`Extends Frame`

The screen which you chose to either join a lobby or create a lobby

![play screen image](https://media.discordapp.net/attachments/558866529253589012/1241228603304312892/image.png?ex=66496fb7&is=66481e37&hm=67e73d7ee489a8109e333af2c994a77b2775b9f04b1b5a71cef270db96e8967e&=&format=webp&quality=lossless&width=767&height=469)

#### status: <span style="color:yellow;">In progress</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    Woojin
```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### client - `Client`
`public` | `final`

this is the client that is being used

### OriginalFrame - `Frame`
`private`

this is the Frame that holds the buttons Create Lobby, Join Lobby

### JoinFrame - `Frame`
`private`

this is the Frame that holds the Join lobby Frame

### CreateFrame - `Frame`
`private`

this is the Frame that holds the Create lobby Frame

## <span style="color:yellow;">Methods</span>

### PlayScreen(Client client)

Create the ui for OriginalFrame, join lobby, create lobby and display originalFrame. And add them to the display, make sure to call Frame.setVisible(false) for the Join and Create frame. Also connect the button events for the buttons.


###  hide() -> `void`
`public` 

Sets all the frames visible to false.