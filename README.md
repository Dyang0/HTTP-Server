# HTTPS-Server
Builds off a simple server implementation in C. I want to create a robust HTTPS server, keeping security in mind. 

[Simple HTTP implementation](https://github.com/hashjaco/C-HTTP-Server)

# Problem Solving

# Learning Objectives
- Understand the differences between HTTP and HTTPS servers. Transition the base HTTP server into a HTTPS server
- Use pentesting/vulnerabilitiy tools to create a robust server
- Find ways to organize my code that reduces complexity
- Connect with [OWASP Top Ten](https://owasp.org/www-project-top-ten/#:~:text=The%20OWASP%20Top%2010%20is,step%20towards%20more%20secure%20coding)
- Document misconceptions and roadblocks. This ties with  

\*DISCLAIMER: This is a developing project so take the information with a grain of salt. The goal is to promote the learning experience rather than getting everything right at the start.

## Server Structure

![image](https://github.com/user-attachments/assets/bbb03718-9f0b-450e-90e0-883fc0d128c4)

This is the basic structure of my HTTP server. The server is run on a localhost using the port 8080 and curl is used to make requests to the server in order to get items in that server.



Future Items
- SQL database (store random data)
- Implement TLS/SSL protocol

## Implementation

![image](https://github.com/user-attachments/assets/67f9e13b-7813-4662-87b5-6754955d6a5c)

![image](https://github.com/user-attachments/assets/5620b80a-9586-4706-8835-88c88e03f31f)

![image](https://github.com/user-attachments/assets/18c5b914-b0aa-48a2-9e59-d6cfac576fad)
It is exciting that I can request items from my server through a web browser by using "http://localhost:[port number]/[item]"
