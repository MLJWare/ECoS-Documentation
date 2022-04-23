# Networking Functions

**NOTE**: _These functions are not fully supported yet._

## `UDP (inPort, sendAddress, sendPort)`
Creates a UDP socket, listening to input on port `inPort`,
and sets the default send address and port to `sendAddress` and `sendPort`.

**NOTE**: _Closes any previous connection if called repeatedly._

## `SEND (data)`
Sends a UDP package with the content `data` on a previously opened socket, 
to the default send address and port.

## `SEND (data, address, port)`
Sends a UDP package with the content `data` on a previously opened socket,
to the specified address and port, `address` and `port`.
