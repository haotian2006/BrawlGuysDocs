# Vector2  
Vector2 represents a two-dimensional vector with X and Y components

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

### X - `float`
`public`

Holds the X component of the vector.

### Y - `float`
`public`

Holds the Y component of the vector.

## <span style="color:yellow;">Methods</span>

### Vector2(`float` x, `float` y)-> `Vector2`
`public` 

Constructor which initializes the vector with given X and Y components.

### Vector2()-> `Vector2`
`public` 

### fromAngle(angle `float`) -> `Vector2`
`public` | `static`

Constructs a normalized Vector2 in the given angle in degrees

### fromPoint(p `Point`) -> `Vector2`
`public` | `static`

Constructs a vector2 from the given point from awt

Default constructor which initializes the vector with X and Y components set to 0.

### toTuple()-> `Tuple2`
`public` 

Converts the vector to a Tuple2 object.

### magnitude()-> `float`
`public` 

Calculates the magnitude of the vector.

### add(v `Vector2`)-> `Vector2`
`public` 

Adds another vector to this vector.

### sub(v `Vector2`)-> `Vector2`
`public` 

Subtracts another vector from this vector.

### mul(s `float`)-> `Vector2`
`public`  

Multiplies this vector by a scalar value.

### div(s `float`)-> `Vector2`
`public` 

Divides this vector by a scalar value.

### dot(v `Vector2`)-> `float`
`public` 

Calculates the dot product of this vector and another vector.

### cross(v `Vector2`)-> `float`
`public` 

Calculates the cross product of this vector and another vector.

### normalize()-> `Vector2`
`public` 

Normalizes this vector.

### angleTo(v `Vector2`)-> `float`
`public` 

Calculates the angle between this vector and another vector.

### distanceTo(v `Vector2`)-> `float`
`public` 

Calculates the distance between this vector and another vector.

### relativeTo(v `Vector2`)-> `Vector2`
`public` 

Calculates the relative position of this vector to another vector.

### hashCode()-> `int`
`public` 

Overrides the default hashCode method.

### equals(obj `Object`)-> `boolean`
`public` 

Overrides the default equals method.

### toString()-> `String`
`public` 

Overrides the default toString method.

