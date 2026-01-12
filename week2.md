<img width="788" height="660" alt="novabench score" src="https://github.com/user-attachments/assets/592aabdb-1939-437c-b23a-388a3760957b" />
<img width="814" height="536" alt="Screenshot 2026-01-12 at 11 59 24" src="https://github.com/user-attachments/assets/94b86320-c733-48b6-b777-b034d2a58b73" />
<img width="709" height="214" alt="Screenshot 2026-01-12 at 12 00 45" src="https://github.com/user-attachments/assets/63b9ef60-37dc-4fae-a206-1c58d1223800" />
The previous images are benchmarking for my base laptop, as well as my virtual machines hardware. I have also got the SSH up and running a touch early, as I thought i should get it out of the way early.
Security configuration list:
SSH hardening - disabling root access over SSH and use key based authentication
Firewall configuration - only allow required ports, and refuse all else
Mandatory access control - enable SELinux or AppArmour, and monitor all access violations to fix any gaps in security.
Automatic updates - enable automatic security updates, regularly check all available updates, and schedule specific safe times to perform them
User priviledge management - create seperate accounts, and use sudo rather than the root user

Threat model:
Threat 1 - Privilege escalation:
This is where a hostile user is given/gains access to a low level access and abuses vulnetabilities to gain access to privileges they are not supposed to have.
This threat can lead to massive damage or data loss if not mitigated.
This threat can be mitigated by keeping sudo commands restricted, enforcing the least privilege needed principle (only giving privileges to those who need them only), as well as keeping all required updates done, and scheduling large updates for safe times of day.
Threat 2 - Unpatched vulnerabilities:
This is where a hostile uses a known vulnerability in outdated software.
This threat can lead to massive compromises in your network/data.
This threat can be mitigated by keeping all software that is used updated asap, and checking for new updates regularly and often.
Threat 3 - SSH brute force
This threat is where a hostile attempts to gain access to your server by guessing(brute forcing) SSH credentials.
This threat can lead to use of your server for nefarious means, or full data loss/downtime for your server.
This threat can be mitigated by disabling password authentication, and using SSH key based authentication exclusively, as well as restricting SSH access by IP address.
