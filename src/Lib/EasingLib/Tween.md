# Tween Class
Tween handles interpolation between values over time using various easing functions.

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

### LookUpTable - `HashMap<EasingFunction, HashMap<EasingType, Method>>`
`private` | `static`

A lookup table mapping easing functions and types to their corresponding methods.

## <span style="color:yellow;">Methods</span>

### Tween(func `EasingFunction`, type `EasingType`)
`public`

Constructor for the Tween class. Initializes a tween with the specified easing function and type.

### getValue(start `float`, goal `float`, alpha `float`, duration `float`) -> `float`
`public` | `static`

Calculates the interpolated value between start and goal based on alpha (progress) and duration.

### getValue(start `float`, goal `float`, alpha `float`) -> `float`
`public`

Overloaded method that calculates the interpolated value between start and goal based on alpha (progress) with a default duration of 1.

### getMethod(func `EasingFunction`, type_ `EasingType`) -> `Method`
`private` | `static`

Retrieves the easing method corresponding to the given function and type from the lookup table.

### getValue(func `EasingFunction`, type `EasingType`, start `float`, goal `float`, alpha `float`, duration `float`) -> `float`
`public` | `static`

Static method that calculates the interpolated value between start and goal based on alpha (progress) and duration using the specified easing function and type.

