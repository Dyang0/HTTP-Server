# HTTPS-Server
Builds off a simple HTTP server implementation in C. The goal is to convert the HTTP server into a robust HTTPS server, keeping security in mind.

# Problem Solving

# Learning Objectives
- Understand the differences between HTTP and HTTPS servers. Transition the base HTTP server into a HTTPS server
- Use pentesting/vulnerabilitiy tools to create a robust server
- Find ways to organize my code that reduces complexity
- Connect with [OWASP Top Ten](https://owasp.org/www-project-top-ten/#:~:text=The%20OWASP%20Top%2010%20is,step%20towards%20more%20secure%20coding)
- Document misconceptions and roadblocks. This ties with  

\*DISCLAIMER: This is a developing project so take the information with a grain of salt. The goal is to promote the learning experience rather than getting everything right at the start.

# Helpful Commands

General
- rm -rf [directory name]

Git
- git status
- git add --all
- git commit -m "[comment]"
- git push

Curl
- curl -v localhost:8080/home.html

gdb
- [Look up later]

## Server Structure

![image](https://github.com/user-attachments/assets/bbb03718-9f0b-450e-90e0-883fc0d128c4)

![image](https://github.com/user-attachments/assets/03af26e8-f605-4d6d-8df4-6c8b3f0e5cf4)

This is the basic structure of my HTTP server. The server is run on a localhost using the port 8080 and curl is used to make requests to the server in order to get items in that server.

Future Items
- SQL database (store random data)
- Implement TLS/SSL protocol

## Documentation
### All Methods
- const char *get_file_extension(const char *filename)
- const char *get_mime_type(const char *file_ext)
- bool case_insensitive_compare(const char *s1, const char *s2)
- char *get_file_case_insensitive(const char *file_name)
- char *url_decode(const char *src)
- void build_http_response(const char *file_name, const char *file_ext, char *response, size_t *response_len)
- void *handle_client(void *arg)
- int main(int argc, char *argv[])

### Sorted Methods
![Sketch 7-23-2024 839 PM](https://github.com/user-attachments/assets/fd36b4b0-ba81-4067-b7cf-64a62c895200)

I have created a diagram to visualize what methods call others. This helps me see and understand the components of a client/server interaction.


## Implementation

![image](https://github.com/user-attachments/assets/5620b80a-9586-4706-8835-88c88e03f31f)

![image](https://github.com/user-attachments/assets/18c5b914-b0aa-48a2-9e59-d6cfac576fad)

It is exciting that I can request items from my server through a web browser by using "http://localhost:[port number]/[item]"

## Roadblocks

![image](https://github.com/user-attachments/assets/779b29b6-25ad-4a76-9902-74159aa6dfaf)
-

## Helpful Resources

- [Understanding Client-Server Architecture in System Design](https://medium.com/@nirajranasinghe/understanding-client-server-architecture-in-system-design-9da079efde60)
  
