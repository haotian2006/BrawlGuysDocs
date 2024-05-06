# UserInputService
A class that handles inputs

#### status: <span style="color:light green;">done</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    haotian 
```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### InputBegan - `Event<KeyEvent>` 
`public` | `final`

Fires when a key is pressed

### InputEnded - `Event<KeyEvent>` 
`public` | `final`

Fires when a key is released

### MouseClick - `Event<MouseEvent>` 
`public` | `final`

Fires when a mouse button is clicked and released

### MouseBegan - `Event<MouseEvent>` 
`public` | `final`

Fires when a mouse button is clicked 

### MouseEnded - `Event<MouseEvent>` 
`public` | `final`

Fires when a mouse button is released

### MouseChanged - `Event<MouseEvent>` 
`public` | `final`

Fires when a mouse moves

### MouseWheelChange - `Event<MouseWheelEvent>` 
`public` | `final`

Fires when a mouse wheel changes



## <span style="color:yellow;">Methods</span>

### isKeyDown(key `KeyEvent`)-> `boolean`
`public` 

returns true if the key is being held


### isButtonDown(key `KeyEvent`)-> `boolean`
`public` 

returns true if the mouse button is being held



