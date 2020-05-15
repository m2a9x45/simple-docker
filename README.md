# Docker Into 🌍

### Description of project

> This was a simple intro to docker. Using wsl2 as I run windows.

I made a docker file which gets a php-apache image from docker hub and then copies the `/src`
directory to `/var/www/html` and finially exposes port 80

I then built an image with :

```console
docker build -t hello-world .
```

And then started the container with :

```console
docker run -p 80:80 -v /home/lewis/dev/testproject/src:/var/www/html hellow-world
```

- -p binds port 80 of the host to port 80 on the local computer
- -v mounts a volume on the host pc to `/var/www/html`

This was achived by following along with a youtube video [here](https://www.youtube.com/watch?v=Qw9zlE3t8Ko)