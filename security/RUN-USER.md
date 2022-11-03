# RUN - USER

When building docker containers, we should always aim to run the process in our container as a non-root user.
This is according to PoLP (Principle of Least Privilege).

To do so you can add the following before you run your application in the container:

```Dockerfile
RUN useradd -u 8877 john 
USER john
```

