# DownloadAccelerator
A program in JAVA that acts as the download accelerator tool using TCP Server and TCP client.

<b>Analysis:</b><br>
To begin working on the program, first I had to get the basic understanding of the requirements and functionalities of the application. I analyzed the program by stating the purpose of the application in a simple flow diagram and specifications.

So, basically I have a file which I partition into 5 smaller parts. I created a server class with five sockets which is open and sends the partitioned file to the client. Then, I made the client server with five sockets open and capable of receiving the file sent from the server. The connection is hard coded with the respective IP and port number. Finally, the five partitioned files received from the server are merged into one single file and saved to the disk.

Next, I understand what kind of information (data analysis) my classes would operate on. I have a clear understanding about what are the required resources that need to be gathered to finish the program. By using Use cases, I represented the tasks that needed to be performed by the program. The basic use case of this project is to send and receive files through server and clients using threads. As a whole, this program is a download accelerator, where a file is downloaded by being partitioned into smaller files and later joined to make a whole file.


<b>Design:</b><br>
Designing the program is all about identifying states and behaviour of the classes while considering their relationships with each other. I created a figurative diagram of the program specifying the tasks of each class and its corresponding components. In the End, I created two classes “TCPServer” and “TCPClient”, where TCP server would partition a file into five parts and send each file through five individual sockets. The partitioning was done by a different class called “FileManagerDriver” and “CustomFileManager”. To test the efficiency of the program each thread had a timer that was started as the thread started.
