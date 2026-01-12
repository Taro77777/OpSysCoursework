For this task, I installed and activateed SSH on the root VM, where my ubuntu server is running from.
I then ensured that virtualbox had a custom network 'device' that could only be accessed by my macbook and the VM, allowing the virtual machine to have a proper IP without being connected to the full internet itself, making myself a sandbox and reducing my attack surface.
I also already made a non root user, which is under my own name (taro) with key based SSH authentication to skip any issues caused by bad passwords.
<img width="702" height="435" alt="Processes" src="https://github.com/user-attachments/assets/ec984ce3-3500-4712-b201-b72401fb16d6" />
All SSH modification has been completed via SSH from my main laptop (as has everything else with this coursework, really)
