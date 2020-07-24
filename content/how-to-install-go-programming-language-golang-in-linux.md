+++
author = "Vipul Jha"
categories = ["Go", "Guide"]
date = 2019-11-18T20:12:00Z
description = "A post about installing Go Programming Language or GoLang in LInux."
image = "/uploads/golang1.jpg"
title = "How to install Go Programming Language (GoLang) in Linux"
type = "post"

+++
Go is a programming language developed by Robert Griesemer, Rob Pike, and Ken Thompson. Go shares a lot of similarities with C programming language. But it has obviously more features than C. Go has garbage collection, structural typing, memory safety etc. Go is really a fast and flexible programming language. In this post I'll guide you through the complete installation of Go programming language in Linux. This guide should work on all Linux distributions (Ubuntu, Arch etc). In case if it doesn't work you can comment down below, I would love to help you out. We'll also write our first Go program. So let's get started.

## **Prerequisites**

* Any Linux distribution
* Internet
* Love for programming

## **Installation**

* Open this [URL](https://golang.org/dl/ "Go website") in favourite browser and download the file for Linux. It will start downloading a .tar file.

![](/blog/uploads/golang11.jpg)

* Open your terminal and change your directory to the one where you've downloaded the tar file.

       ```
       cd your_directory
       ```

   ![](/blog/uploads/golang2.png)

* Now we have to extract and install the .tar file of Go. Just enter the below command and it will do the job.

       ```
       sudo tar -c /usr/local -xzf file_name.tar.gz
       ```

   ![](/blog/uploads/golang3.png)
   
* The installation is done now. But we have to define the path of our Go installation so that we can use it. I am using nano here, you can use any editor like vim, gedit etc.

       ```
       sudo nano ~/.profile
       ```
* Take your cursor to the bottom and enter the following line as shown in code and screenshot. Then save the changes by using CTRL+O & CTRL+X commands.

       ```
       PATH="$PATH:/usr/local/bin:$PATH"
       ```

   ![](/blog/uploads/golang4.png)

* Now we have to source our changes to system.

       ```
       source ~./profile
       ```
* Now let's verify our installation. Just enter the following command in your terminal.

       ```
       go version
       ```
* If it gives a output similar to the given screenshot then congratulations you've done and amazing job so far. Go programming language is finally installed on your Linux machine.

   ![](/blog/uploads/golang6.png)

## **First Go program**

1. Let's create our first Go program by entering the given command in terminal. I am again using nano here. You can use any text editor.

       ```
       nano first.go
       ```
2. Now paste the following code in the editor and save the program by using CTRL+O & CTRL+X

       ```go
       package main
       
       import "fmt"
       
       func main() {
       	fmt.Println("Hello, Go!")
       }
       ```
3. Run the following command

       ```
       go run first.go
       ```
4. Hurray! You've compiled your first ever Go program.

   ![](/blog/uploads/golang10.png)

So finally we've installed Go programming language in our Linux system and wrote our very first Go program successfully. 