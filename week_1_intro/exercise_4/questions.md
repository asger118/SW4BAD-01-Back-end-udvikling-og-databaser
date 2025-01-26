<h3>Reflect and write short sentences on the following</h3>

1. **What is a docker image?** <br>
   The docker container image specifies how the file system on the docker container should look. Container image is a standardized package that includes all of the files, binaries, libraries, and configurations to run a container. Docker images are designed to work with different types of applications, such as a web app built using ASP.NET Core. By packaging everything together, Docker images ensure that applications can run consistently across different environments, whether it's a developer's laptop, a testing server, or a production environment. <br>
   **There are two important principles of images**<br>
    Images are immutable. Once an image is created, it can't be modified. You can only make a new image or add changes on top of it.

    Container images are composed of layers. Each layer represents a set of file system changes that add, remove, or modify files.
2. **What is a docker container?**<br>
   A docker container is unit that holds an application and everything that it needs to run such as code, runtime, libraries, and system dependencies. Essentially, containers are a way to package software in a way that allows it to run consistently on any machine, regardless of the environment or operating system it’s running on. Under here in some key features. <br>
    **Self-contained** <br>
    Each container has everything it needs to function with no reliance on any pre-installed dependencies on the host machine. <br>
    **Isolated**<br>
    Since containers are run in isolation, they have minimal influence on the host and other containers, increasing the security of your applications. <br>
    **Independent** <br>
     Each container is independently managed. Deleting one container won't affect any others. <br>
    **Portable**<br>
    Containers can run anywhere! The container that runs on your development machine will work the same way in a data center or anywhere in the cloud!
3. **What is the relation between an image and a container?**<br>
   Images are used to create containers: A Docker container is created by running an image. You can think of the image as a template, and the container as an instantiation of that template. One image can create multiple containers: Multiple containers can be created from the same image. These containers are isolated from one another, even though they share the same image.
4. **What is a port mapping? Illustrate a port mapping by drawing a system sequence diagram describing the flow when you invoke localhost:3000 in your browser.** <br>
   Port mapping (also called port forwarding) in the context of Docker refers to the process of connecting a port on your local machine (the host) to a port on a container. This allows services running inside the container to be accessible from outside the container, typically from your local machine, other containers, or even the public internet (if properly configured).
   