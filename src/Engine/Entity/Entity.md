# Entity
Base Entity Class

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

### **box** - `AABB`
`public`

AABB of the entity

###  guid - `UUID`
`public` | `final`

the unique id of the entity


## <span style="color:yellow;">Methods</span>

### onCollision(other: `Entity`) -> `void`

`public` | `abstract`

what will happen when it collides

### canCollideWith(other: `Entity`) -> `boolean`

`public` | `abstract`

if the entity can collide with the other Entity

### update(deltaTime `double`) -> `void`

`public` | `abstract`

updates the Entity

### draw(graphics `Graphics2D`,center `Vector2`) -> `void`
`public` | `abstract`

Gives the Graphics and center of the screen for drawing the entity

### destroy() -> `void`
`public`

Removes the entity from the world 

