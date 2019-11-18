+++
author = "Vipul Jha"
categories = ["Go", "Guide"]
date = 2019-11-18T20:12:00Z
description = "A post about installing Go Programming Language or GoLang in LInux."
draft = true
image = "/blog/uploads/golang1.jpg"
title = "How to install Go Programming Language (GoLang) in Linux"
type = "post"

+++
Go is a programming language developed by Robert Griesemer, Rob Pike, and Ken Thompson. Go shares a lot of similarities with C programming language. But it has obviously more features than C. Go has garbage collection, structural typing, memory safety etc. Go is really a fast and flexible programming language. In this post I'll guide you through the complete installation of Go programming language in Linux. This guide should work on all Linux distributions (Ubuntu, Arch etc). In case if it doesn't work you can comment down below, I would love to help you out. We'll also write our first Go program. So let's get started.

## **Prerequisites**

* Any Linux distribution
* Internet
* Love for programming

## **Installation**

1\. Open this [URL](https://golang.org/dl/ "Go website") in favourite browser and download the file for Linux. It will start downloading a .tar file.

![](/blog/uploads/golang11.jpg)

2. Open your terminal and change your directory to the one where you've downloaded the tar file.

       cd your_directory

   ![](/blog/uploads/golang2.png)
3. Now we have to extract and install the .tar file of Go. Just enter the below command and it will do the job.

       sudo tar -c /usr/local -xzf file_name.tar.gz

   ![](/blog/uploads/golang3.png)
4. The installation is done now. But we have to define the path of our Go installation so that we can use it. I am using nano here, you can use any editor like vim, gedit etc.

       sudo nano ~/.profile
5. Take your cursor to the bottom and enter the following line as shown in code and screenshot.

       PATH="$PATH:/usr/local/bin:$PATH"

   ![](/blog/uploads/golang4.png)