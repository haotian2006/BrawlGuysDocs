# Camera
Handles Camera Position

#### status: <span style="color:Red;">Not Started</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
Woojin

```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```

## <span style="color:green;">Fields</span>

### Position - `Vector2`
`public`

The Position Of the camera

### Subject -`Entity`
`public`

### Mode - `CameraMode`

Which Entity is the Camera Spectating, Should be Normal by default

## <span style="color:yellow;">Methods</span>

### setEntity(Entity subject) -> `void` 
`public`

This will set the interpolate the camera towards that entity's position and set Entity. (for now just make it set the Subject if you want)

### getPosition() -> `Vector2`
`public` 

Gets the Position of the camera, return the center of the Entity if `mode` is set to `Normal` and Subject isn't `null` else return the `Position`


