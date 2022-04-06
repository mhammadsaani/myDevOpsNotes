<h1 align="center"> Networking </h1>

<h3 align="center"> The Internet: A Network of Networks </h3>

### Computer Network & Internet
In simple term (layman term), computer network means computer connected to each other with cables or wireless radio and a sort of group of computers is formed and 
these different groups(network of computers) are connected and are termed as Internet(a network of computer networks) .


### ***Protocols***
A set of rules governing the exchange or transmission of data between devices Or
The rules for exchange of data are called ***Protocols*** . 
Here a question may arise in your mind, why we need protocols?. If yes, then here is the **answer**. 
Suppose, you made an application and set some rules for communicating this application with other application but some other person made other rules for communicating.
So, due to this issue, communication is not feasible. Therefore, a set of standerd rules is important to have, which is written by 
[***Internet Society Organization***](https://www.internetsociety.org/learning/?gclid=CjwKCAiA55mPBhBOEiwANmzoQollWESh4rtBH7KNA-VvlJ5_f0RZ4ukLkznK23Y2R-RWM4DOYvlT8BoCj10QAvD_BwE).

Some common Protocols are 
 - TCP (Transmission Control Protocol)
 - UDP (User Datagram Protocol)
 - HTTP (Hyper Text Transfer Protocol)
 
 ### ***TCP***
 The Transmission Control Protocol is a protocol that ensures that **100%** of data reaches the intended destination and
is not corrupted along the way
So, if you want a person to get something completely, then you are going to use this protocol.
 
 ### ***UDP*** 
 User Datagram Protocol (UDP) does not ensure that data reaches the destination or not and that it remains incorrupt.
 When you do not care if **100%** data is reaching to your friend or not, you use UDP like in case of **Video Conferencing**.
 
 ### ***HTTP***
 HTTP is a client-server protocol that determines how web clients requests web pages from web servers and how web servers send them.
 
  - World Wide Web is collection of all the information/pages/documents which are interlinked meaning 
    we can go from one page to second, second to third and so on.
 
 Following protocols, we have established a communication system. Computers send messages to one another. (These messages are made up of ones and zeros, bits). However, instead of sending the whole message (that could be more than trillion bits) at once, information/message is broken down into smaller units called ***Packets***
 Now, Packet is ready for sending and packet(smaller unit of message) has to be addressed to a certain application on a certain end system (Devices connected to Internet also called as Edge Systems like Mobile Phone, Desktop Computers etc). So, here comes the role of **Addressing**. 
 
 One more thing to mention here is ***Network Edge*** which is collection of end systems. Note, devices that relay messages like router are not part of Network Edge.
 
 ### ***IP Address***
 Every device that is connected to the Internet has an address called an ‘IP
Address’ which is much like a mailing address means a 
unique address of the modem (provided by your Internet service provider) called **Global IP** .
You can check your computer *IP address* using ``` curl ifconfig.me -s ``` in your command line interface. 
There can be multiple devices connected to the modem. Modem will give IP address to each of device which is connected to that modem,
using DHCP (Dynamic Host Configration Protocal). Each device can have lot of applications, so exactly which application is requesting the data is determined by ***PORTS***
<h3 align="center"> IP addresses identify end systems but ports identify an application on the end system </h3>
 
 How we will get the searched file in laymans term. 
 Device Made a request, it will go to the router.
 
 From ***Router --> Inter Service Provider --> Internet***
 
Data needs to be transmitted from one end system to another over a medium. 
There are two kinds of media
 - Guided
 - Unguided
 
1- Guided: A medium in which the signal is transported on a
defined pathway is called guided like Fibre Optics

2- Unguided: Means of transmission that are not bound by a confined pathway are called
unguided media, such as radio waves.

### ***Socket***
Socket is the combination of IP address and Port

### ***Switch***
It is used to help communication of devices within LAN. It knows the IP address of all the devices. 

### ***Router***
Sits between LAN and WAN. It helps communication of devices outside of LAN.



## OSI Model

### Application Layer
It reads data from the user and write off the data (send date) to transport layer. The application layer completely resides on End Systems. These end systems can be any internet device.

All the text-based network apps (email),  voice over IP, (WhatsApp calls), video chat (Skype), and video streaming (YouTube) runs on application layer protocols. 

#### Client Server Model

***Server*** work is to control the access to a centralized resource like website.
For this .Two important things are needed:
1- They should be online 24/7
2- They should have a reliable IP through which they can be accessed/reached

***Client*** process usually initiate the connection to access centralized resource which is on the internet.

Server wait for the requests from client

#### Program Vs Process Vs Thread

A program is simply an executable file. An application such as MS Word is one example.
A process is any currently running instance of a program. So one program can have several copies of it running at once. One MS Word program can have multiple open windows.
A thread is a lightweight process. One process can have multiple running threads. The difference between threads and processes is that threads do lightweight singular jobs.

Microsoft Docs is a program, Editing a docs is Process, Saving an image/setting a font,  is a thread.

IP address determines which end system to send data, ports determines which application on that end system to send data and ***Ephemeral Ports*** are used to determine which instance (process) to send data. 

### HTTP Basics

Web pages are objects that consists of other objects. Object is basically a file like HTML, PNG, MP3 etc.
and *HTTP* , as already mentioned, is a web protocol which defines how web clients requests web pages from web servers and how web servers responds them. 
HTTP is a ***stateless protocol*** meaning that it does not store data of clients by default

Application Layer protocols rely/depend on TCP and UDP which lies on lower layer. HTTP which is an application layer protocol relies on TCP. Relying on lower layer is the key feature in Layer architecture models. 

TCP is connection oriented, meaning a connection has to be initiated in order to start communication of client with server.  
There are two types of HTTP connections
- Persistent (Use One TCP connection to serve all HTTP requests)
- Non Persistent (Used one TCP connection to serve one request)




