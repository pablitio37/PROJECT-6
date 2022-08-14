# PROJECT-6
WEB SOLUTION WITH WORDPRESS

You are progressing in practicing to implement web solutions using different technologies. As a DevOps engineer you will most probably encounter PHP-based solutions since, even in 2021, it is the dominant web programming language used by more websites than any other programming language.

In this project you will be tasked to prepare storage infrastructure on two Linux servers and implement a basic web solution using WordPress. WordPress is a free and open-source content management system written in PHP and paired with MySQL or MariaDB as its backend Relational Database Management System (RDBMS).

Project 6 consists of two parts:

Configure storage subsystem for Web and Database servers based on Linux OS. The focus of this part is to give you practical experience of working with disks, partitions and volumes in Linux.

Install WordPress and connect it to a remote MySQL database server. This part of the project will solidify your skills of deploying Web and DB tiers of Web solution.
## LAUNCH AN EC2 INSTANCE THAT WILL SERVE AS “WEB SERVER”.
Step 1 — Prepare a Web Server
Launch an EC2 instance that will serve as "Web Server". Create 3 volumes in the same AZ as your Web Server EC2, each of 10 GiB.

![text1](https://user-images.githubusercontent.com/108102087/184541329-da4de1d5-9fe2-409c-bacc-5c406fed9b9a.PNG)

Using lsblk utility to view the newly configured partition on each of the 3 disks.

![text2](https://user-images.githubusercontent.com/108102087/184542211-8e2410cb-72ff-4c43-a027-4e4c2eb73aa1.PNG)

Verify that your Physical volume has been created successfully by running sudo pvs

![text3](https://user-images.githubusercontent.com/108102087/184542885-b22301b4-b84a-46d1-b7b5-09c8c79d438b.PNG)
