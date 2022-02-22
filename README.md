# ParallelAndDistributedProject

How to run:

filesToSend.txt contains a list of the files that the client will send to the server. Each file is separated by a newline character.

In TCPServer.java, line 20 is a for loop. This loop accepts a connection for every new file in filesToSend. 
The number in the for loop should correspond to the number of files in filesToSend.txt. 
I have not found a way to automate this yet, so that is why it is hard coded. For instance, if there are 3 files in filesToSend.txt:

for (int i = 0; i < 3; i++)

Each of the 3 programs should be run on their own machine. This way, each of the socket connections have their own IP address.

Start TCPServerRouter.java. This will facilitate connections between the server and the router
Start TCPServer.java. This will accept connection from TCPClient.java through TCPServerRouter.javva
Start TCPClient.java. This will send data to TCPServer.java through TCPServerRouter.java.


