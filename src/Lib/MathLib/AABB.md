# AABB Class
AABB (Axis-Aligned Bounding Box) represents a rectangular bounding volume defined by its position and size.

#### status: <span style="color:green;">done</span>
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

### Position - `Vector2`
`public`

Represents the position of the AABB.

### Size - `Vector2`
`public`

Represents the size of the AABB.

### Velocity - `Vector2`
`public`

Represents the velocity of the AABB.

## <span style="color:yellow;">Methods</span>

### AABB(Position `Vector2`, Size `Vector2`)
`public`

Constructor for AABB class. Initializes the AABB with the given position and size.

### copy() -> `AABB`
`public`

creates a copy of the current AABB

### translate(v `Vector2`)
`public`

Translates the AABB by the given vector.

### resize(v `Vector2`)
`public`

Resizes the AABB to the given size, maintaining its center.

### setCenter(center `Vector2`)
`public`

Sets the center of the AABB to the specified position.

### getCenter() -> `Vector2`
`public`

Returns the center of the AABB.

### overlaps(other `AABB`) -> `boolean`
`public`

Checks if this AABB overlaps with another AABB.

### containsPoint(point `Vector2`) -> `boolean`
`public`

Checks if the AABB contains the specified point.

### getBroadphase() -> `AABB`
`public`

Returns a broad-phase AABB based on the AABB's velocity.

### SweptAABB(other `AABB`, entryTime `float`, normal `int[]`) -> `float`
`public`

Calculates the time of impact between this AABB and another AABB, and returns the entry time.

