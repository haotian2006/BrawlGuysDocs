# CollisionHandler Class
The CollisionHandler is responsible for managing collisions between entities and tiles in the game environment. It uses axis-aligned bounding boxes (AABB) to detect and handle these interactions.

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
+ Collisions break when an axis is -1 
    Fixed by limiting the range from 1<x<maxX
```
## <span style="color:green;">Fields</span>



### tileHandler - `TileHandler`
`private`

Reference to the `TileHandler` responsible for managing tiles in the game.

### world - `Engine`
`private`

Reference to the main `Engine` instance which contains game logic and manages game state.

### EPSILON - `float`
`public` | `static` | `final`

A small epsilon value used in collision resolution to avoid floating-point precision issues.

## <span style="color:yellow;">Methods</span>

### CollisionHandler(world `Engine`)
`public`

Constructor for initializing a new instance of `CollisionHandler` with a reference to the main game engine.

### entityVsTileLoop(entity `Entity`, modifiedAABB `AABB`) -> `Tuple2<Float, Vector2>`
`private`

Calculates the collision response between an entity and tile objects within the game world, returning the earliest collision time and normal.

### getEntityInBounds(aabb `AABB`) -> `Entity[]`
`public`

Overloaded method that retrieves all entities within a specified axis-aligned bounding box without additional parameters.

### entityVsTile(entity `Entity`, dt `double`) -> `Vector2`
`public`

Calculates and resolves collisions between an entity and tiles within the game world for a given time step, returning the new position of the entity after collision resolution.
