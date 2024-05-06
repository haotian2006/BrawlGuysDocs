# Remote
`Abstract`
Used to for communications 
#### status: <span style="color:green;">Done</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    haotian - created Remote
```
### <span style="color:lightgreen;">Notes:</span>
```diff
    4/14/24 - class done
```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### name - `String`
`final`

Name of the remote

### onMessage - `Event<Packet>`
`public` | `final`

a event that is fired when a message is retrieved 


## <span style="color:yellow;">Methods</span>

### Remote(name `String`) -> `Remote`
`constructor` | `protected`

This is used by the handler

### fireServer(data `Packet`) -> `void`
`public` 

Sends a message to the Server

### fireClient(client `Client`, data `Packet`) -> `void`
`public` | `overload`

Sends a message to the given Client

### fireAllClients(data `Packet`) -> `void`
`public` 

Sends a message to all the Clients

### fireAllClientsExcept(exclude `Client`, data `Packet`) -> `void`
`public` 

Sends a message to all the Clients except the given Client

