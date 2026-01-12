For CPU and RAM stress testing, I would use stress-ng, as it uses compute heavy loops to access large amounts of the CPU and RAM resources all at once.
For IO workloads, I would use Fio, as it spams IO patterns to increase IO wait, slowing the system.
For Network testing, I would use iperf3, as it measures max network speeds, leading to large bandwidth usage.
For everything else, I would use nginx to simulate an actual server handling request, leading to medium amounts of resource drain on all fronts.
In order to install these, I would run the following:
sudo apt install stress-ng
sudo apt install fio iperf3 nginx
