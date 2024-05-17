
# EntityHandler
A class responsible for managing entities within the engine.

#### status: <span style="color:green;">Done</span>
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

### INIT_SIZE - `int`
`private` | `final`

The initial size of the entity maps. Set to 500.

### entities - `HashMap<UUID, Entity>`
`private`

A map of entities indexed by their UUID.

### entitiesById - `HashMap<Short, Entity>`
`private`

A map of entities indexed by their short ID.

### removePool - `Stack<UUID>`
`private`

A stack to hold UUIDs of entities to be removed.

### addPool - `Stack<Entity>`
`private`

A stack to hold entities to be added.

### isIterating - `boolean`
`private`

Flag to indicate if the handler is currently iterating over entities.

### idGenerator - `IdGenerator`
`private`

An instance of the IdGenerator class to manage entity IDs.

### currentComponentData - `ComponentMap`
`private`

A map to hold component data for entities.

### engine - `Engine`
`public` | `final`

A reference to the engine associated with this handler.

## <span style="color:yellow;">Methods</span>

### getNextId() -> `short`
`public`

Returns the next available short ID using the IdGenerator.

### registerMethod(int id, BiConsumer<Entity, Serializable> m)
`public` | `static`

Registers a method to handle entity components.

### registerComponent(int id, Class<? extends AbstractComponent> c, BiConsumer<? extends AbstractComponent, Serializable> method)
`public` | `static`

Registers a component and its handling method.

### parseData(ComponentMap map)
`protected`

Parses component data and applies it to entities.

### setComponent(Entity entity, int id, Serializable value)
`public`

Sets a component for an entity.

### add(Entity entity)
`public`

Adds an entity to the handler.

### remove(UUID id) -> `Entity`
`public`

Removes an entity from the handler given its UUID.

### remove(Entity e) -> `Entity`
`public`

Overloaded method to remove an entity from the handler.

### get(UUID id) -> `Entity`
`public`

Gets an entity from the handler given its UUID.

### get(short id) -> `Entity`
`public`

Gets an entity from the handler given its short ID.

### contains(UUID id) -> `boolean`
`public`

Checks if the handler contains an entity with the given UUID.

### contains(Entity e) -> `boolean`
`public`

Overloaded method to check if the handler contains the given entity.

### size() -> `int`
`public`

Returns the number of entities in the handler.

### getAllEntities() -> `Collection<Entity>`
`public`

Returns a collection of all entities in the handler.

### update(double dt)
`protected`

Updates entities within the handler.

### draw(Graphics2D g, Vector2 center)
`protected`

Draws entities within the handler.
