Since a Docker image is created based on Alpine linux a binary should be compiled as statically linked because Alpine does not resolve references to dynamic libraries out-of-the-box.  
Use the following command to build a binary:
```
gcc -static -O3 -o hello-world hello.c 
```
Use Dockerfile to build an image.  
The application prints "Hello, world!" and quits.
