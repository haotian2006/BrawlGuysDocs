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

### Physics_Components - `LinkedHashSet<PhysicsComponent>`

Used to store physics components of an entity

### Render_Components - `LinkedHashSet<RenderComponent>`

Used to store render components of an entity


## <span style="color:yellow;">Methods</span>

### defaultPhysicsComponents() -> `LinkedHashSet<PhysicsComponent>`
`public`

Used by the entity constructor, should return the base components of an entity 

### defaultRenderComponents() -> `LinkedHashSet<RenderComponent>`
`public`

Used by the entity constructor, should return the base components of an entity 

### addPhysicsComponent(component `PhysicsComponent`) -> `boolean`
`public`

adds a physics component to the entity

### addRenderComponent(component `RenderComponent`) -> `boolean`
`public`

adds a render component to the entity

### removePhysicsComponent(component `PhysicsComponent`) -> `boolean`
`public`

removes a physics component from the entity

### removeRenderComponent(component `RenderComponent`) -> `boolean`
`public`

removes a render component from the entity

### onCollision(other: `Entity`) -> `void`

`public` | `abstract`

what will happen when it collides

### resize(v `Vector2`) -> `void`
`public`

Resizes the hitbox of the entity

### translate(v `Vector2`) -> `void`
`public`

Translates the position of the entity

### setVelocity(v `Vector2`) -> `void`
`public`

Sets the velocity of the entity

### setCenter(v `Vector2`) -> `void`
`public`

Sets the center of the hitbox of the entity

### setPosition(v `Vector2`) -> `void`
`public`

Sets the position of the hitbox of the entity

### setAngle(a `int`) -> `void`
`public`

Sets the angle of the entity

### getCenter() -> `Vector2`
`public`

Gets the center of the hitbox of the entity

### getPosition() -> `Vector2`
`public`

Gets the position of the hitbox of the entity

### getVelocity() -> `Vector2`
`public`

Gets the velocity of the entity

### update(deltaTime `double`) -> `void`

`public` | `abstract`

updates the Entity

### draw(graphics `Graphics2D`,center `Vector2`) -> `void`
`public` | `abstract`

Gives the Graphics and center of the screen for drawing the entity

### destroy() -> `void`
`public`

Removes the entity from the engine 

