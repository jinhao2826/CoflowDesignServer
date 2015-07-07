CoflowServer
===================================
This is a Coflow Server.
TCP connection is at least a pair. One is client, the other is server. It is similar in Coflow.
So if you want to use my implementation, you must need at least one Coflow Client and one Coflow Server.
  
1.What is the Coflow?
-----------------------------------
Coflow is one kind of Networking Abstraction for Cluster Applications. 
Paper: http://conferences.sigcomm.org/hotnets/2012/papers/hotnets12-final51.pdf

2.What is the Coflow Client/Server?
--------------------------------------
I implement Coflow in Linux kernel 4.0.
TCP connection is at least a pair. One is client, the other is server.
So if you want to use my implementation, you must need at least one Coflow Client and one Coflow Server.
It is a prototype. I do not merge Client and Server Code together, next version maybe I will do it. And add one compile flag when compile the kernel.
3.How to use?
----------------------------------------------
I am sure both Coflow client and Coflow server can run correctly and stably in Linux kernel 4.0.
You also can port code to other Linux Kernel. I think it is very easy, you can use the Tool like Araxis Merge to port the code. Then compile and update your kernel.
4.How to design Coflow?
-------------------------------------------------------
Please refer to my Design Coflow pdf in Coflow_Application Folder.
5.How to see the result?
-------------------------------------------------------
This prototype goal is to get the Coflow Completion Time.
The result are recorded in Coflow server /var/log/kern.log. Please use sudo vim /var/log/kernel to see the result and use sudo truncate -s 0 /var/log/kernel to clear log.
