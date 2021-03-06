PHP WebSockets
==============
PHP WebSockets is a PHP library that implements the latest version of
the WebSockets protocol. The [WebSockets protocol](http://www.rfc-editor.org/rfc/rfc6455.txt) (RFC6455) is currently being
standardized by the IETF. With WebSockets, a client (e.g.: a browser) and
a server can set up a two-way communication channel with little overhead
compared to a XMLHttpRequest or long polling.

Usage
-----
The demo can be started by starting the `Demo/run.php` file from the command-
line. You might need to edit the file to change the servers IP and/or port.

The `ChatServer` demo is a basic chatserver that has little functionality. You
can use it as a basis to build more complex `WebSocketServers` using this library.

The basic idea is that your `WebSocketServer` should implement the `ServerObserver`
interface and subscribe to (or observe) a `WebSocketServer` instance. If you want to
observer or subscribe to events that accur on the incomming `WebSocketConnections` too,
you should implement the `ConnectionObserver` interface too and subscribe to the
incomming connections in the `ServerObserver :: onNewConnection()` method.

License
-------
This library is licensed under the terms of the MIT license which
can be found in the LICENSE file.

Acknowledgements
----------------
Thanks to Peter Beverloo for his support and advice.