# UiTween 
A Class for creating UI Tween Objects

#### status: <span style="color:green;">done</span>
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


### component - `JComponent`
`private`

The component to apply the tween to

### info - `UiTweenInfo`
`private`

The tween information

### goal - `HashMap<UiTweenMethods,Object>`
`private`

The goal of the tween

### isPlaying - `boolean`
`private`

If the tween is currently playing

### tween - `Tween`
`private`

The tween object

### completedSignal - `Signal<Boolean>`
`private`

Signal when the tween is completed

### completed - `Event<Boolean>`
`public`

Event when the tween is completed

### cancelledSignal - `Signal<Void>`
`private`

Signal when the tween is cancelled

### cancelled - `Event<Void>`
`public`

Event when the tween is cancelled

## <span style="color:yellow;">Methods</span>

### parseGoal(goal `HashMap<UiTweenMethods,Object>`)
`private`

Parses the goal of the tween so that if object is just equals to goal then object will turn into {start,goal}

### UiTween(component `JComponent`, info `UiTweenInfo`, goal `HashMap<UiTweenMethods,Object>`)
`public`

Creates a new UI tween with the given component, information, and goal. For goal Object can either be {start,goal} or just goal

### stop()
`public`

Stops the tween from playing

### play()
`public`

Plays the tween

### TweenLocation(Start `Point`, goal `Point`, time `float`)-> `Point`
`private`

Tweens the location of the component to the goal at the given time

### TweenSize(Start `Dimension`, goal `Dimension`, time `float`)-> `Dimension`
`private`

Tweens the size of the component to the goal at the given time

### TweenSizeFromCenter(Start `Dimension`, goal `Dimension`, time `float`)-> `Dimension`
`private`

Tweens the size of the component from the center to the goal at the given time

### TweenColor(Start `Color`, goal `Color`, time `float`)-> `Color`
`private`

Tweens the color of the component to the goal at the given time
