# How to Install Docker on WIndows OS

So you're getting started in web components. Maybe someone you know told you to work in docker. What does that mean? How do you even install it? What should you do with it? I'm going to walk you through an install with Windows 10. Then we'll talk about what to do with docker.

# What is a container based system?

Before you even install and try to run docker, you should probably understand what it is. Docker is a light-weight way of running a program through containers and microservices. Monolith Server Architecture is a thing of the past because we traditionally hosted resources in one environment. This made it versatile, but also heavy and very difficult to update changes. Microservices are used to split up tasks into specific operations. In the picture below, you can see all the small microservices one interface may be running on multiple machines. The whole functionality of a backend is now in thousands of containers all over the world.

![Monolith example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/g8r2lb7qu155x1fndu3q.png)

And now for the most important question...

# Why a container based system?

I could list some classic tech bull about "[insert new technology] is the future". The honest answer is docker is the best tool to run an app in any environment. This is because of the microservice architecture. You can have exactly same setup everywhere and quickly move the whole infrastructure. Containers can be spun up very quickly, which changes the way we look at tech.

## 1: Download Docker

You can use this [link](https://www.docker.com/products/docker-desktop) to download the desktop app. Like any other download once that is complete you should open it up.

## 2: Open Docker

Upon opening it you're probably gonna have a ton of issues. Don't stress, its normal. As soon as it boots it will most likely tell you that you need to do things with the Linux kernel. It's unlikely you already have it and you need it in order to give docker the tooling that it needs.

## 3: Download the Linux kernel

You should click the [link](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package) that it sends you in order to start the download.

## 4: Restart and open

It should be walking you through this but after you download the Linux kernel, restart your computer. When you reboot you can open docker. If you did this right, you'll find a tutorial waiting for you. You are more then welcome to use theirs but after that I would try to finish this tutorial to really get a handle on the useful things docker can help with.

## 5: The Docker GitHub Crossover

Marvel: 'Infinity War' Is The Most Ambitious Crossover Event In History
Me:
![Docker and GitHub](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/j76tww2eo7xg7rljz0al.png)

In all seriousness docker is perfect for running your projects, but how does that happen? Patrick McDowell explains this in his [article](https://developer.okta.com/blog/2018/09/27/test-your-github-repositories-with-docker-in-five-minutes) with a really helpful diagram.

![Docker and GitHub examples](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wg13qs07jcqpye0hlbi2.png)

## 6: Create a Dev Environment

To get started, open a new dev environment. You can find them under the Dev Environment tab on the left. Your screen should look like this.

![Dev Environment Tab](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4xzg283ouhfwj45pk51h.png)

## 7: Link your repository

Once you hit get started you can follow the directions to set it up. I am going to clone an already existing repository to get it running locally on my computer. Choose your repository and open it on GitHub. Below you can see how to get the link. Choose the green Code dropdown, click the SSH tab, and copy the link. You may have to set up an SSH key if you haven't or use the HTTPS link.

![GitHub Cloning Example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/lqjhycra7qx0tm88veka.png)

On docker, input that link. You can see the example below. It may take a minute for docker to prepare it but trust me its much faster than other clones. You should get a success screen afterwards.

![Docker screen with repo link](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/39anrdefwo8iczjkquo7.png)

## 8: Start Coding

Now you should be all good to go and you can open this in VS Code. You may be prompted to add some extensions in in order to do this. No big deal, it should be helpful.

![Success Message](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3dsgv4ybqsd5qq5f6ezb.png)

![Extension](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/my5cc5l6ann5b62zxjz5.png)

Congrats you have successfully connected to a container! Keep coding!
