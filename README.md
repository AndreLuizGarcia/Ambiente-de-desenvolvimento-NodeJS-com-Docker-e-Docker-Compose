# Ambiente-de-desenvolvimento-NodeJS-com-Docker-e-Docker-Compose

This is a simple node.js project builded into a container to help a understanding the concepts and see how it's works and help the development environment a lot.

## What is Docker?

Docker is an open platform for developing, shipping, and running applications. Docker enables you to separate your applications from your infrastructure so you can deliver software quickly. With Docker, you can manage your infrastructure in the same ways you manage your applications. By taking advantage of Docker’s methodologies for shipping, testing, and deploying code quickly, you can significantly reduce the delay between writing code and running it in production.

You can see more in documentation and Getting Starting page:

- [Docker Overview](https://docs.docker.com/engine/docker-overview/)
- [Docker Install](https://docs.docker.com/install/)

```bash
pip install foobar
```

## Commands

To this project I just used a express library to create a little server HTTP to make a "Hello World Docker :)"

If you don't know much things a lot express you can see more and build a little server by the documentation.

- [Express Guide](https://expressjs.com/en/guide/routing.html)

In my terminal I used this commands to build, run and see my containers running:

This command is to build my docker image and "andre/dockernode" was the name of image.

```
docker build -t andre/dockernode .
```
Here I runned the image and set the port was used, in this case from port 3000 to port 3000, in relation with the computer and container.

```
docker run -p 3000:3000 -d andre/dockernode
```

To see the images witch is running just run:

```
docker ps
```

If you are using the compose, to run it run in your terminal:

```
docker-compose up
```

And to see the ip of your machine it's simple:

```
docker-machine ip
```
