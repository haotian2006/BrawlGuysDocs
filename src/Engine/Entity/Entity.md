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

