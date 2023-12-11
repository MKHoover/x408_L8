# x408_L8
Single Responsibility Architecture

Instructions for setting up docker and getting access to hello_http app.

1. Go to https://github.com/MKHoover/x408\_L8 and clone to your local directory. The app is included.
2. CD into new directory.
3. First create a docker image with `$ docker build -t <image name> hello_http`.
4. Confirm your image was created with `$ docker image ls --all`
5. Instantiate a container based on your image with `$docker run -dp 127.0.0.1:12344:12344 --name=<container name> <image name>`
6. Confirm your container was created with `$docker container ls --all` 
7. If you make changes to the app, in order to save changes, you need to recreate the docker image and deploy(instantiate)a new container (steps 3-6).
