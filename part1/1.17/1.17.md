# 1.17 My favorite programming environment

[Link to the Docker Hub](https://hub.docker.com/repository/docker/lukxsx/programming-environment)

This Docker image is using Arch Linux as the base image, because
Arch Linux is my favorite GNU/Linux distribution. It uses the
```base-devel``` tag, which includes some basic C/C++ tools like
GCC

JDK 11 and Python 3 are also installed on the image. It has also some
build and programming tools like Maven, Gradle, Meson and Git. 

The image should be run with 
```docker run -v "$(pwd):/mydir" -it lukxsx/programming-environment```
to bind the programming environment to the filesystem. 
