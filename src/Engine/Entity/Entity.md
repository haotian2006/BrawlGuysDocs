# Entity
Base Entity Class

#### status: <span style="color:yellow;">In progress</span>
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

### Grid_Scale - `int`
`public` | `static` | `final`

The grid scale of the entity, retrieved from the TileHandler.

### HitBox - `AABB`
`public`

The axis-aligned bounding box representing the entity's hitbox.

### Angle - `int`
`public`

The angle of the entity.

### Scale - `double`
`public`

The scale of the entity.

### EntityID - `short`
`public` | `final`

The ID of the entity.

### ID - `UUID`
`public` | `final`

The UUID of the entity.

### engine - `Engine`
`public` | `final`

Reference to the engine associated with this entity.

### entityHandler - `EntityHandler`
`public` | `final`

Reference to the entity handler associated with this entity's engine.

### Destroyed - `boolean`
`public`

Flag indicating if the entity is destroyed.

### Image - `BufferedImage`
`private`

The image associated with the entity.

### Variant - `String`
`private`

The variant of the entity.

### Components - `ComponentContainer`
`private`

The container for the entity's components.

## <span style="color:yellow;">Methods</span>

### Entity(Engine engine)
`public` | `constructor`

Constructor for Entity.

### addComponent(AbstractComponent c)
`public`

Adds a component to the entity.

### addComponent(AbstractComponent c, int index)
`public`

Adds a component to the entity at a specified index.

### getComponent(Class<? extends AbstractComponent> c) -> `T`
`public`

Gets a component from the entity based on its class.

### hasComponent(Class<? extends AbstractComponent> c) -> `boolean`
`public`

Checks if the entity has a component of the specified class.

### updateImage(String path)
`private`

Updates the entity's image based on the provided path.

### getImagePathFromVariant() -> `String`
`public`

Gets the image path based on the entity's variant.

### setVariant(String v)
`public`

Sets the variant of the entity.

### getImage() -> `BufferedImage`
`public`

Gets the image associated with the entity.

### setScale(double s)
`public`

Sets the scale of the entity.

### hashCode() -> `int`
`@Override` | `public`

Returns the hash code of the entity.

### equals(Object obj) -> `boolean`
`@Override` | `public`

Checks if two entities are equal.

### resize(Vector2 v)
`public`

Resizes the entity.

### translate(Vector2 v)
`public`

Translates the entity.

### setVelocity(Vector2 v)
`public`

Sets the velocity of the entity.

### setCenter(Vector2 v)
`public`

Sets the center of the entity.

### setPosition(Vector2 v)
`public`

Sets the position of the entity.

### setAngle(int a)
`public`

Sets the angle of the entity.

### getCenter() -> `Vector2`
`public`

Gets the center of the entity.

### getPosition() -> `Vector2`
`public`

Gets the position of the entity.

### getVelocity() -> `Vector2`
`public`

Gets the velocity of the entity.

### onCollision(Object o) -> `boolean`
`public`

Checks if the entity collides with an object.

### update(double dt)
`public`

Updates the entity.

### getDisplayCoords(Vector2 center) -> `Vector2`
`public`

Gets the display coordinates of the entity.

### getDisplaySize() -> `int`
`public`

Gets the display size of the entity.

### draw(Graphics2D g, Vector2 center)
`public`

Draws the entity.

### destroy()
`public`

Destroys the entity.
