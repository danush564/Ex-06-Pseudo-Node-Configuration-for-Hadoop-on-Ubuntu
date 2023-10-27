# Exp 06 Pseudo Node Configuration for Hadoop on Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

![image](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/7488a792-8b05-4eda-9543-1c69fae36c98)

2.	Install java1.8 in folder /usr/local

![image](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/ae856653-6f86-48dd-b70e-8b985c6f583f)

3.	Install Hadoop

![image](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/7ceaa735-c1bb-4e54-bffb-71dc23935967)

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file

 
5.	Set hadoop environment variables: Include the following lines /etc/profile file


6.	Run the.bashrc & profile files from the $ prompt for updating the changes




$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file


b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)


 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags


c)	mapred-site.xml
 

Include the following lines in mapred-site.xml file
 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file


e)	yarn-site.xml
Include the following lines in yarn-site.xml file
8.	Format the Hadoop File system implemented on top of the local file system using

9.	Start Hadoop using


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:


11.	Create a directory ‘/input’ in HDFS


12.	Copy the input files into the distributed file system

13.	Run some of the examples provided


14.	Examine the output files
Copy the output files from the distributed file system to the local file system and examine them:
 
or
View the output files on the distributed file system

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
