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

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/79837812-4c00-4c49-8eeb-74fc936fd073)

5.	Set hadoop environment variables: Include the following lines /etc/profile file

 ![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/7416df4c-3313-4e97-aa0c-8eff395daaa7)



6.	Run the.bashrc & profile files from the $ prompt for updating the changes

![Screenshot (430)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/e1c02e2b-9e64-4b6e-a7cd-dad5de809ed7)

![Screenshot (431)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/ceb3c64b-e717-4504-8bef-75b07277417f)

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/dfb2383d-701c-4c21-b8c6-0070ec7c2f2b)

b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![Screenshot (430)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/a53c81b2-4153-4aff-86e0-630cfebae95f)

 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![Screenshot (431)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/3418a24c-d656-45d5-ac80-87cc8106305f)

c)	mapred-site.xml
 
![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/4b14e30c-453b-4510-99d3-726bad66bc5a)

Include the following lines in mapred-site.xml file
 
![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/e269ba7c-c2c4-4cba-92e4-8fad32b6fa33)

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/512105db-3e63-41e9-af44-3ad26a3aec9e)

e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/336e3956-450d-4195-8f90-9d1ba1d91e54)

8.	Format the Hadoop File system implemented on top of the local file system using

![Screenshot (429)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/83c2dcd5-9325-445c-802d-af4612c43d31)

9.	Start Hadoop using
$sbin/start-all.sh
Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/48f6a0ed-71d2-47ac-adc0-e91108ca91cf)

11.	Create a directory ‘/input’ in HDFS

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/0a6df9a0-3e91-4b8b-a28e-96e3f6e1f2ee)

12.	Copy the input files into the distributed file system

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/7fca1085-622e-41c7-a28f-5f341aada126)

13.	Run some of the examples provided

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/8b77af4f-877c-4c80-8a58-705e7ab9795d)

14.	Examine the output files

![Screenshot (428)](https://github.com/danush564/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/98585166/e3724503-ad6a-46b4-be46-8dd3f5e8195f)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
