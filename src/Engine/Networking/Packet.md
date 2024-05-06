# Packet
`Implements Serializable` 
Holds data thats being sent from the server/client

#### status: <span style="color:Green;">Done</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    Haotian - Created packet
```
### <span style="color:lightgreen;">Notes:</span>
```diff

```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### Remote - `String`
the name of the remote being used

### UUID - `String`
A unique ID used to determine who sent it

### Payload - `List<Serializable>`
Data thats being sent 

## <span style="color:yellow;">Methods</span>

### Packet() -> `Packet`
creates a packet

### Packet(UUID `String`) -> `Packet`
`Constructor` | `Public`

creates a Packet with the given UUID

### getUUID() -> `String`
`public`

returns the UUID

### addToPayLoad(object `Serializable`) -> `void`
`public`

Adds an object to the payload

### getPayLoad() -> `List<Serializable>`
`public`

returns the payload list

### getRemote() -> `String`
`public`

returns the remote that sent the packet.

### attachInfo() -> `Packet`
`public`

This is used by NetworkHandler
