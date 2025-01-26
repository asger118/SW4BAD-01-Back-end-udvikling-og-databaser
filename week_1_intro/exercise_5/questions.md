**Write down an answer to the following questions:**<br>
- What is the difference between the two docker files? One is in section Build and deploy manually  and the other in the section The Dockerfile...
  
- **Is it possible to have multiple Dockerfiles in one project?**<br>
  Yes, it is possible to have multiple Dockerfiles in one project. You can create multiple Dockerfiles to accommodate different needs or environments (e.g., one Dockerfile for development, another for production). You can name them differently (e.g., Dockerfile.dev, Dockerfile.prod) and specify which one to use with the -f option when building the image
- **What are the benefits of using a multi-stage build strategy when building .NET images?**<br>
    **Smaller Final Image Size:**
    Multi-stage builds remove unnecessary files, dependencies, and build tools from the final image, resulting in smaller images that are faster to download and deploy.


    **Better Separation of Concerns:**
    The build and runtime environments are separated, ensuring that the final image only contains what is required to run the application (e.g., runtime dependencies for .NET).


    **Improved Security:**
    By excluding build tools and temporary files from the final image, you reduce the attack surface area, making the image more secure.


    **Portability Across Environments:**
    Multi-stage builds allow you to use specific images for different stages (e.g., an SDK image for building and a runtime image for deployment), ensuring that the app runs consistently across environments.
  

    **Faster Deployment:**
    Smaller and optimized images reduce the time needed for deployment, especially in containerized environments like Kubernetes or cloud platforms.