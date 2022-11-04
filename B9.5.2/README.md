Dockerize the application that prints "Hello, world!" and quits.  
Since a Docker image will be created based on Alpine linux a binary should be compiled as statically linked because Alpine does not resolve references to dynamic libraries out-of-the-box.  
Use the following command to build a binary:
```
gcc -static -O3 -o hello-world hello.c 
```
The resulting image can be found here:  
[https://hub.docker.com/repository/docker/invokae/skillfactory](https://hub.docker.com/repository/docker/invokae/skillfactory)
