# Docker Gimp - GUI application (X11 DISPLAY sharing)

## Links
- https://www.youtube.com/watch?v=cMsIT2otEjA

## Verify that the socket exists and is available
~~~shell
ls -l /tmp/.X11-unix/
~~~

## Granting access rights for the X server
~~~shell
xhost +local:docker
~~~

This command allows the Docker container to communicate with your X server.

Note that this command weakens the security of your X server,
by allowing access to all local clients.

If necessary, you can restrict access to a specific user or container.

## Run
~~~shell
make init
~~~

## Show logs:
~~~shell
make logs
~~~