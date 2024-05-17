# AbstractComponent
An abstract class representing a component attached to an entity.

#### status: <span style="color:done;">green</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    haotian - created class and methods
```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### updatable - `boolean`
`public` | `final`

Flag indicating whether the component is updatable.

### drawable - `boolean`
`public` | `final`

Flag indicating whether the component is drawable.

### entity - `Entity`
`public` | `final`

Reference to the entity this component belongs to.

### engine - `Engine`
`public` | `final`

Reference to the engine associated with this component.

### entityHandler - `EntityHandler`
`public` | `final`

Reference to the entity handler associated with this component's engine.

## <span style="color:yellow;">Methods</span>

### AbstractComponent(Entity entity, boolean updatable, boolean drawable)
`public` | `constructor`

Constructor for AbstractComponent.

### hashCode() -> `int`
`public`

Returns the hash code of the class.

### equals(Object obj) -> `boolean`
`public`

Checks if two objects are equal based on their classes.

### update(double dt)
`public`

Method to update the component.

### draw(Graphics2D g, Vector2 center, Vector2 displayCoords)
`public`

Method to draw the component.
