For CPU and RAM stress testing, I would use stress-ng, as it uses compute heavy loops to access large amounts of the CPU and RAM resources all at once.
For IO workloads, I would use Fio, as it spams IO patterns to increase IO wait, slowing the system.
For Network testing, I would use iperf3, as it measures max network speeds, leading to large bandwidth usage.
For everything else, I would use nginx to simulate an actual server handling request, leading to medium amounts of resource drain on all fronts.
In order to install these, I would run the following:
sudo apt install stress-ng
sudo apt install fio iperf3 nginx
Expected resource profiles:
CPU stress - I expect the CPU to reapidly reach 100% usage, and for all tasks to take much longer to finish.
RAM stress - I expect the available RAM to decrease very quickly, and other processes to slow down at the same time
Disk stress - I expect this to cause slow responses for disk dependant tasks, and for an increase in disk read and write amounts.
Network stress - I expect the network interface to be filled with requests rapidly, slowing down network related tasks.
Service usage - I expect all resources to be used in medium amounts, with nothing being stressed beyond normal limits
