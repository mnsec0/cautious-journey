## Be wary of the networks you inherit - the most secure systems are the ones that do not exist.
### Check out my main site at [mnsec0.net](https://mnsec0.net)

***

#### Vulnhub CTF: DerpNStink
[Download](https://www.vulnhub.com/entry/derpnstink-1,221/)
##### I was very pleased with this CTF, as it was subjectively easy but I still had to use some advanced techniques to get the final flags.

Let's start off with making sure our machines are connected properly so that they can see each other on the network. You can either put them on a NAT Network, or have your machines use the Bridged Adapter. 

Using Kali, we now run `arp-scan -l` to see the devices on our network, and see that the box we want to attack is at 192.168.1.39:
(image here)

To see what ports are open, we will now use `nmap 192.168.1.39`:
(image here)

