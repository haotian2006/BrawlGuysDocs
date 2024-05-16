# Client
A Client 

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

### isLocal - `boolean`
`private`

Is the client also the server

### ipAddress - `String`
`private`

The Ip of the client

### id - `Short`
`private`

Short of the client

### name - `String`
`private`

name of the client

### in - `ObjectInputStream`
InputStream of the client

### out - `ObjectOutputStream`
OutputStream of the client

### tcpConnection - `Socket`
TCPconnection with the server



## <span style="color:yellow;">Methods</span>

### Client(connection `Socket`)-> `Client`
`protected` | `constructor`

creates the client with the given socket

### setName(name `String`)-> `void`
`public`

sets the name of the client

### getIpAddress()-> `String`
`public`

gets the Ip address of the client
### getName()-> `String`
`public`

Get the name of the client

### getId()-> `Short`
`public`

Get the name of the client

### getIn()-> `ObjectInputStream`
`protected`

Get the InputStream of the client

### getOut()-> `ObjectOutputStream`
`protected`

Get the OutputStream of the client

### getConnection()-> `Socket`
`protected`

Get the TCPconnection with the server

### toString()-> `String`
`public`

returns the string of the client in the format of "name | isLocal | Short"


