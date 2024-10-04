# Cybersecurity Incident Report


## Section 1: Identify the type of attack that may have caused this network interruption: One Potential Explanation for the website's connection timeout error message is:

The wiresharks logs show  log 52 203.0.113.0(source) to attempt connection using protocl TCP to 192.0.2.1. Through out logs 52,53, & 54 there is a succesfull 3 way handshake. Once completed, there was no attempt to get any data back from our servers, and quickly we start to see through log 57, 59, 61, and more logs multiple attempts from same source(203.0.113.0) to connect to our servers, ultimately overwhelming our system. We can see the amount of attempts to connects increase, once we get to log 98, we see the system no longer be able to connect with any IP, including within employees IPs. Looking through the logs, we can clearly see all of the attacks are coming from the same source IP, 203.0.113.0, making this a DOS attack. 


## Section 2: Explaining how the attack is causing the website to malfunction:
When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. The three steps of the handshake:

1. [SYN] - this is the first attept for the source IP to make a connection to our systems. Syn stands for Synchronize

2. [SYN, ACK] - this packet is 

3. [ACK] -

Explain what happens when a malicious actor sends a large number of SYN packets all at once:

Explain what the logs indicate and how that affects the server:
