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

Verify that your VG has been created successfully by running sudo vgs

![text4](https://user-images.githubusercontent.com/108102087/184543377-5791d7ce-a6f1-4bf5-a77d-2de98cd73cf7.PNG)

Verify that your Logical Volume has been created successfully by running sudo lvs

![text5](https://user-images.githubusercontent.com/108102087/184543927-c98403a6-821b-456d-8024-9dcd5e12eb1f.PNG)

Verifying the entire setup

![text6](https://user-images.githubusercontent.com/108102087/184544428-5d70f2b9-7db6-4d78-beb6-d7204f966b39.PNG)

UPDATE THE `/ETC/FSTAB` FILE
The UUID of the device will be used to update the /etc/fstab file; Test the configuration and reload the daemon

![text1](https://user-images.githubusercontent.com/108102087/185744562-fbd29a8e-e099-48dc-9a48-c7730ec1eca8.PNG)

Verify your setup by running df -h

![text2](https://user-images.githubusercontent.com/108102087/185744708-6bd62ea6-1453-4bfc-947f-f636d31e6fde.PNG)

the database as been mounted

![text3](https://user-images.githubusercontent.com/108102087/185746116-d807d0b0-bc28-4a0b-bd3d-ed942934f304.PNG)

To install PHP and it’s depemdencies

![text4](https://user-images.githubusercontent.com/108102087/185751428-3d32e9a6-7d51-4476-8813-c6f69eb46244.PNG)

Configure DB to work with WordPress and Configure WordPress to connect to remote database
