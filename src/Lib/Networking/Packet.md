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

### RemoteID - `Byte`
`protected`

The ID of the remote being used

### clientID - `Short`
`protected`

A unique ID used to determine who sent the packet

### Payload - `List<Serializable>`
`protected`

Data that is being sent

## <span style="color:yellow;">Methods</span>

### Packet() -> `Packet`
`public`

Creates a new Packet object

### Packet(Short `clientId`) -> `Packet`
`protected`

Creates a Packet object with the given client ID

### getClientID() -> `Short`
`public`

Returns the client ID associated with the packet

### addToPayLoad(Serializable `object`) -> `void`
`public`

Adds an object to the packet's payload list

### getPayLoad() -> `List<Serializable>`
`public`

Returns the list of objects in the packet's payload

### attachInfo(Byte `remoteId`, Short `clientId`) -> `Packet`
`protected`

Creates a new Packet object with additional information about the remote and client IDs

### attachInfo(Byte `remoteId`) -> `Packet`
`protected`

Creates a new Packet object with additional information about the remote ID

