# NetworkHandler
Main Class to handle networking

#### status: <span style="color:green;">done</span>
### <span style="color:cyan;">Contributors:</span>
<!--put your names here between the ``` if you worked on it, and put what you did-->
```diff
    Haotian - got a working prototype 
```
### <span style="color:lightgreen;">Notes:</span>
```diff
    4/14/24 Networking works
    4/15/24 Updated docs 
```
### <span style="color:red;">Bugs:</span>
```diff
```
## <span style="color:green;">Fields</span>

### TIMEOUT - `int`
`protected` | `final` | `static`

Used to for  client/server disconnection timers.

### INTERVAL - `int`
`protected` | `final` | `static`

How often should the server/client ping and check

### localClient - `Client`
`protected`

The Client of the machine

### TargetIp - `String`
The IP of the server

### Port - `int`
Port of the Server

### IsServer - `boolean`
Is it the Server or Client 

### Clients - `HashMap<String,Client>`
Clients connected to the Machine

### Remotes - `HashMap<String,Remote>`
Remotes created for the Network

### handleCrashFlag - `boolean`
Used to determine if the Handler already handled a server crash

### ClientAdded - `Event`
`public` | `final`

Fired when a client is added

### ClientRemoved - `Event`
`public` | `final`

Fired when a client is removed

### OnServerClose - `Event`
`public` | `final`

Fired when the server is closing



## <span style="color:yellow;">Methods</span>

### StartServer(port `int` ) -> `void`
`public` | `static`

Starts the Server


### NetworkHandler() -> `void`
`public` | `this`

Constructor, creates NetworkHandler

### getLocal() -> `Client`
`public`

Returns the local client

### getRemote(name `String`) -> `Remote`
`public`

Returns a Remote with the given name

### getNetworkRemote(name `String`) -> `NetworkRemote`
`protected`

Returns a NetworkRemote with the given name

### createRemote(name `String`) -> `Remote`
`public` | `deprecated`

Creates a Remote with the given name

### createRemote(name `String`,isUDP `boolean`) -> `Remote`
`public` | `deprecated`

Creates a Remote with the given name and UDP status

### getTargetIpAddress() -> `String`
`public`

Returns the target IP address

### setPort(port `int`) -> `void`
`public`

Sets the port

### setTargetIpAddress(ip `String`) -> `void`
`public`

Sets the target IP address

### addClient(client `Client`) -> `void`
`protected`

Adds a client to the list of clients and fires ClientAdded event

### removeClient(client `Client`) -> `void`
`public`

Removes a client from the list of clients and fires ClientLeft event

### generateClientName() -> `String`
`protected`

Generates a unique client name

### isValidName(String name) -> `boolean`
`public`

returns true if no other client has that name

### getClient(id `UUID`) -> `Client`
`public`

Returns a client with the given UUID

### getClient(packet `Packet`) -> `Client`
`public`

Returns a client with the given Packet

### getClient(name `String`) -> `Client`
`public`

Returns a client with the given name

### getClients() -> `Client[]`
`public`

Returns all clients

### getPort() -> `int`
`public`

Returns the port

### StartServer() -> `void`
`public` | `throws IOException`

Starts the server

### StopServer() -> `void`
`public`

Stops the server

### StartClient() -> `void`
`public` | `throws IOException`

Starts the client

### StopClient() -> `void`
`public`

Stops the client

### handleServerClose(reason `ServerClosed`) -> `void`
`protected`

Handles a server crash and fires ServerClose event
