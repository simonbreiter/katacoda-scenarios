This is your first step.

## Dockerfile

When building Docker containers you define your base image in your `Dockerfile`. The scratch image is the smallest possible image for docker. 

## Compile executable

In order to run binary files on a scratch image, your executables need to be statically compiled and self-contained. This means there is no compiler in the image so you’re left with just system calls.

`gcc -o hello hello.c -static`{{execute}}

## Build image

Now build and tag your image.

`docker build --tag hello .`{{execute}}

## Run container

After you build your image you can ship it, share it with others or run it locally.

`docker run hello`{{execute}}

