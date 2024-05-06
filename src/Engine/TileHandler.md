# TileHandler Class
TileHandler manages a grid of Tile objects within a defined area.

#### status: <span style="color:Green;">Done</span>
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

### Tile_Lookup - `HashMap<Character, Tile>`
`public` | `static` | `final`

Maps characters to Tile objects for easy lookup and tile instantiation.

### Grid_Scale - `int`
`public` | `static` | `final`

Defines the scale of the grid, used for rendering tiles in proportion to screen space.

## <span style="color:yellow;">Methods</span>

### setup()
`protected` | `static`

Initializes the Tile_Lookup with tiles corresponding to different character keys.

### TileHandler(x `int`, y `int`)
`protected`

Constructor that initializes the tile grid with specified dimensions x and y.

### setTile(x `int`, y `int`, t `Tile`)
`public`

Sets a tile at the specified grid location.

### getTile(x `int`, y `int`) -> `Tile`
`public`

Retrieves the tile at the specified grid coordinates. Returns null if coordinates are out of bounds.

### getTile(v `Vector2`) -> `Tile`
`public`

Overloaded method to retrieve a tile based on a Vector2 position.

### update(dt `double`)
`protected`

Updates the state of the tile handler, typically called every frame.

### draw(g `Graphics2D`, center `Vector2`)
`protected`

Renders the grid of tiles to the screen, adjusted for the camera position and centering relative to the provided Graphics2D context.
