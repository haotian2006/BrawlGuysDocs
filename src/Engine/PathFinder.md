# PathFinder Class
The `PathFinder` class in the `Engine` package facilitates pathfinding within a grid-based map using the A* (A-star) algorithm. It calculates the shortest path between two points while avoiding obstacles based on tile properties.

#### status: <span style="color:green;">done</span>
### <span style="color:cyan;">Contributors:</span>
<!-- List contributors and their contributions here. For example: -->
```diff
 Haotian - created and implemented the A* algorithm
```
### <span style="color:red;">Bugs:</span>
```diff

```
## <span style="color:green;">Fields</span>

### handler - `TileHandler`
`private`

Holds the reference to the `TileHandler` that manages tiles which the pathfinder uses to determine walkable paths.

## <span style="color:yellow;">Methods</span>

### PathFinder(handler `TileHandler`)
`public`

Constructor for initializing a `PathFinder` with a given `TileHandler`.

### findPath(startPosition `Vector2`, endPosition `Vector2`) -> `List<Vector2>`
`public`

Calculates the shortest path from the start to the end position using the A* algorithm. It returns a list of `Vector2` points representing the path.

### reconstructPath(endNode `Node`) -> `List<Vector2>`
`private`

Reconstructs the path from the end node to the start node using backtracking from parent references in nodes.

### getNeighbors(position `Vector2`) -> `List<Vector2>`
`private`

Returns a list of valid adjacent positions (neighbors) around a given position that can be navigated to.

## <span style="color:magenta;">Inner Classes</span>

### Node
Represents a node in the pathfinding context, holding position, cost metrics (g, h, f), and parent node information.

#### Fields:
- position - `Vector2`: The position of the node in the grid.
- parent - `Node`: Reference to the parent node in the path.
- g - `double`: Cost from the start node to this node.
- h - `double`: Heuristic cost estimate from this node to the end node.
- f - `double`: Total cost (g + h) used to prioritize node processing.

#### Methods:
- compareTo(other `Node`) -> `int`: Compares nodes based on their total cost `f` for prioritizing in the pathfinding queue.
- equals(obj `Object`) -> `boolean`: Determines equality based on node position.
- hashCode() -> `int`: Provides a hash code based on node position for use in collections.
