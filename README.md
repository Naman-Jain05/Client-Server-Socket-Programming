# Client-Server-Socket-Programming
sockets use TCP and IPV4 protocols.

How To Run :
○ Each of the server files can be run using:-> python serverx.py "host" "port"
○ Client files can be run using:-> python client.py "host" "port"

1. server program "server1.py " will be a single process server that canhandle only one client at a time. If a second client tries to chat with the server while some other client's session is already in progress, the second client's socket operations should see an error. After the first client closes the connection, the server should then accept connections from the other client.
2. server program "server2.py " will be a multi-threaded server that will create a new thread for every new client request it receives. Multiple clients should be able to simultaneously chat with the server
3. server program "server3.py " will be a single process server that uses the "select" method to handle multiple clients concurrently
4. server program "server4.py" will be an echo server (that replies the same message to the client that was received from the same client); it will be a single process server that uses the "select" method to handle multiple clients concurrently

Edge cases covered:
Keyboard interrupt ctrl+c
Invalid argument
Connecting to an unopened port
Connecting to an already opened port

