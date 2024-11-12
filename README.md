# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

```
Name : Pavan Kumar A B
Reg.No: 212222040113
```

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

![Screenshot 2023-10-24 193657](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/39a0f695-6ec2-4140-9877-f0b8ecbfabfc)

2.	Install java1.8 in folder /usr/local

![Screenshot 2023-10-24 193712](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/f699b523-f51c-403c-bf7b-49572801cb1c)

3.	Install Hadoop

![Screenshot 2023-10-24 193724](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/21883d17-702f-4cec-b534-f0189121e305)

4.	Set the hadoop environment variables: Include the following lines in the
5.	
$HOME/.bashrc file

 ![Screenshot 2023-10-24 193734](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/c2519752-39b7-4eda-bc66-6a3590291f98)

5.	Set hadoop environment variables: Include the following lines /etc/profile file

![Screenshot 2023-10-24 193746](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/3c76dabb-e3e6-416c-bf9b-040569c34f3c)

6.	Run the.bashrc & profile files from the $ prompt for updating the changes


![Screenshot 2023-10-24 193833](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/038259a3-e76b-4210-92f3-4cf2cc30546b)


$ bin/hadoop version	


7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml


path ::	/usr/local/hadoop-2.5.1/etc/hadoop


a)	hadoop-env.sh

Include the following lines in hadoop-env.sh file

![Screenshot 2023-10-24 193842](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/e8edc5e7-bd35-4f38-a9f7-76bc2a9e1354)

b)	core-site.xml

Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![Screenshot 2023-10-24 193851](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/4771b777-f944-4dd5-a26e-c9a4eabf946e)


 
Include the following lines in core-site.xml file between <configuration> and

</configuration> tags

![Screenshot 2023-10-24 193907](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/fda3f89e-cb94-470b-abf2-0e18b013c411)

c)	mapred-site.xml
 
![Screenshot 2023-10-24 194518](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/c1c187e0-1479-4a90-a1c8-705e04f43334)

Include the following lines in mapred-site.xml file
 
![Screenshot 2023-10-24 194545](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/69429f3d-67c3-4884-b54e-a178728526fc)

d)	hdfs-site.xml

Include the following lines in hdfs-site.xml file

![Screenshot 2023-10-24 194609](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/3ddff1e6-f246-463c-ab72-3857b1e6972a)

e)	yarn-site.xml

Include the following lines in yarn-site.xml file

![Screenshot 2023-10-24 194633](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/470d9d38-3b3b-412f-a8fd-ac6429a703b1)

8.	Format the Hadoop File system implemented on top of the local file system using

![Screenshot 2023-10-24 194652](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/d38d0ed5-c260-4b80-8905-406c86d55ad3)

9.	Start Hadoop using

![Screenshot 2023-10-24 194720](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/12029523-2368-4a08-a76b-9259ffaec3ec)

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![Screenshot 2023-10-24 194735](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/d4cbd9e5-faf6-45b5-bfdf-7b61f9f74a39)

11.	Create a directory ‘/input’ in HDFS

![Screenshot 2023-10-24 194750](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/4dc99b55-e758-41ca-be1f-1890d58dc00a)

12.	Copy the input files into the distributed file system

![Screenshot 2023-10-24 194801](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/705faa0c-4648-45d5-b668-d11cc952cac8)

13.	Run some of the examples provided

![Screenshot 2023-10-24 194812](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/cec7b0bc-bf0f-4415-b99c-e2cf3da6e681)


14.	Examine the output files

![Screenshot 2023-10-24 194824](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/5b4225ef-69d0-4e50-8569-bb1ee3aa96c0)

Copy the output files from the distributed file system to the local file system and examine them:

 ![Screenshot 2023-10-24 194835](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/951b694f-e3f3-4a9c-9536-81d0448d842c)

or
View the output files on the distributed file system
![Screenshot 2023-10-24 194845](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/119559905/dac190f0-8d57-4c3f-b385-30f946536cd6)

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
