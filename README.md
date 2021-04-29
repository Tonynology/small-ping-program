# small-ping-program

This is a ping program which is running on Linux.
The ping requested an IP packet of 4096 bytes in length (4068 of data, 8 for ICMP header, and 20 for IP header) and it was split into 3 fragments and the reply was also split into 3 fragments.
The result shows packet transmitted, received and lost.

After compile, it used Linux Capabilities, “CAP_NET_RAW” in order to be able to use raw socket in a safe way. Setting capabilities on executables allows running the program without having to run the risk of being run as root.

 ![ping1](https://user-images.githubusercontent.com/36941592/116508994-5a084c80-a877-11eb-88f5-aa059eef556a.png)
