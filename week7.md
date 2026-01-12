<img width="641" height="147" alt="7 50 1httE140 089 1 87 2024-01-12 1336 49999" src="https://github.com/user-attachments/assets/262e0ace-2dbb-4603-8d56-784a3142d616" />
<img width="564" height="162" alt="Initiating ARP Ping Scan at 1336" src="https://github.com/user-attachments/assets/762aaa9d-cd1f-4400-8fb3-f9ca8f7866df" />
This is my security report, complete as best I could with the small issue I faced during this stage.
I used nmap to scan the open network ports of the server, and I found that there was an open port 22/tcp on the server (which is the SSH)
It is good that there are not many open ports, as this largely reduces the attack surface of the server.
The port that is open is essential, as it is needed for SSH to function, therefore it is relatively safe to leave it open, as this makes the server much easier to use and work on.
Overall, I believe that my Ubuntu server is reasonably hardened as a virtual machine accessable via network SSH. I am pleased with my work :)
