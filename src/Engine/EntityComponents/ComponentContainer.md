# ComponentContainer
A class representing a container for abstract components.

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

### components - `ArrayList<AbstractComponent>`
`private`

List to store abstract components.

## <span style="color:yellow;">Methods</span>

### ComponentContainer()
`public` | `constructor`

Constructor for ComponentContainer.

### iterator() -> `Iterator<AbstractComponent>`
`public`

Returns an iterator over the components.

### foundType(AbstractComponent c) -> `AbstractComponent`
`public`

Finds a component of the same type as the provided component.

### get(Class<? extends AbstractComponent> c) -> `AbstractComponent`
`public`

Gets a component based on its class.

### add(AbstractComponent c) -> `boolean`
`public`

Adds a component to the container if not already present.

### clear()
`public`

Clears all components from the container.

### add(AbstractComponent c, int index) -> `AbstractComponent`
`public`

Adds a component to the container at a specified index.

### remove(AbstractComponent c) -> `boolean`
`public`

Removes a component from the container.

### remove(Class<? extends AbstractComponent> c) -> `boolean`
`public`

Removes a component based on its class.

### remove(int index) -> `AbstractComponent`
`public`

Removes a component at a specified index from the container.
