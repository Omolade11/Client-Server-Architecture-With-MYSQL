# CLIENT-SERVER ARCHITECTURE WITH MYSQL

Understanding Client-Server Architecture
As you proceed with your journey into the world of IT, you will begin to realise that certain concepts apply to many other areas. One of such concepts is – Client-Server architecture.
Client-Server refers to an architecture in which two or more computers are connected together over a network to send and receive requests between one another.
In their communication, each machine has its own role: the machine sending requests is usually referred as "Client" and the machine responding (serving) is called "Server".
A simple diagram of Web Client-Server architecture is presented below:
![](https://github.com/TobiOlajumoke/DevOps-Projects/blob/main/Project_5/Images/P5S1.png)

In the example above, a machine that is trying to access a Web site using a Web browser or simply ‘curl’ command is a client and it sends HTTP requests to a Web server (Apache, Nginx, IIS or any other) over the Internet.

If we extend this concept further and add a Database Server to our architecture, we can get this picture:
![](https://github.com/TobiOlajumoke/DevOps-Projects/blob/main/Project_5/Images/P5S1.1.png)

In this case, our Web Server has a role of a "Client" that connects and reads/writes to/from a Database (DB) Server (MySQL, MongoDB, Oracle, SQL Server or any other), and the communication between them happens over a Local Network (it can also be an Internet connection, but it is a common practice to place Web Server and DB Server close to each other in a local network). The setup on the diagram above is a typical generic Web Stack architecture that you have already implemented in previous projects (LAMP, LEMP, MEAN, MERN), this architecture can be implemented with many other technologies – various Web and DB servers, from small Single-page applications SPA to large and complex portals.

This LAMP website server(s) can be located anywhere in the world and you can reach it also from any part of the globe over global network- Internet. Assuming that you go on your browser, and typed in there www.propitixhomes.com. It means that your browser is considered the "Client". Essentially, it is sending requests to the remote server, and in turn, would be expecting some kind of response from the remote server. Let’s take a very quick example and see Client-Server communicatation in action. Open up your Ubuntu or Windows terminal and run the curl command:

```
curl -Iv www.google.com
```
Note: If your Ubuntu does not have ‘curl’, you can install it by running ```sudo apt install curl``` In this example, your terminal will be the client, while www.google.com will be the server.

See the response from the remote server in the image below. You can also see that the requests from the URL are being served by a computer with an IP address 142.251.16.103 on port 80. More on IP addresses and ports when we get to Networking related projects
![](https://github.com/Omolade11/Client-Server-Architecture-With-MYSQL/blob/main/Images/Screenshot%202022-12-20%20at%2022.36.10.png)
