# Create A DockerFile

So you're interested in Docker? You came to the right spot. Today I'm going through what it is, a video tutorial on how to get started, and a tutorial on how to create a DockerFile.

## What is Docker

Before you even install and try to run docker, you should probably understand what it is. Docker is a light-weight way of running a program through containers and microservices. Monolith Server Architecture is a thing of the past because we traditionally hosted resources in one environment. This made it versatile, but also heavy and very difficult to update changes. Microservices are used to split up tasks into specific operations. In the picture below, you can see all the small microservices one interface may be running on multiple machines. The whole functionality of a backend is now in thousands of containers all over the world.

![Docker Image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/q483pnmlbt8321ekuitl.png)

## Get started

You can follow this [tutorial](https://youtu.be/UOC5hksJoSM) to learn more about how to run docker on your browser. Remember when copying and pasting into docker you may have to use `ctrl` `shift` `p`.

## Create a DockerFile

1. Run your GitHub repo in the [docker playground](https://labs.play-with-docker.com/).
2. Run `touch Dockerfile`
3. Select `Editor` to open the file system. You should see your file.
   ![Editor showing Dockerfile](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/iq408hdikhprtv01uhxy.png)
4. Double click on the Dockerfile in order to edit its contents.
5. Paste in the basic information shown below.

```
# syntax=docker/dockerfile:1
FROM node:12-alpine
RUN apk add --no-cache python2 g++ make
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
```

6. Run `docker build -t getting-started .`
7. Start the app with `docker run -dp 3000:3000 getting-started`
8. Open [http://localhost:3000/](http://localhost:3000/). You should see a running app.

You now have a working Dockerfile! Congrats and keep coding!
