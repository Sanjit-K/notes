What is an #Ip-address ?
- Allows communication over #layer-3 of the #OSI model
- Splits into binary(1 byte between each period) ex: 00110110.11101001.10011011.10100101
	- Goes up to 255.255.255.255
- Somewhere around 4 billion ==IPv4== addresses, however a lot more people use them
	- ==IPv6== made to fix this, has a LOT more address space
- No one uses IPv6 but why?
	- What is a #NAT?
		- Network Address Translation reduces the amount of IP addresses being used by mapping multiple ==private ip-addresses==(your phone, tablet, computer, etc.) to a singular ==public ip-address==(your router)![[NATexample.png]]

| Network Class | Network Numbers | Network Mask  | # of Networks | # of Hosts per Network | INFO                                                                                    |
| ------------- | --------------- | ------------- | ------------- | ---------------------- | --------------------------------------------------------------------------------------- |
| A             | 10.0.0.0        | 255.0.0.0     | 126           | 16,646,144             | Used by HUGE corporations or government organizations                                   |
| B             | 172.16-31.0.0   | 255.255.0.0   | 16,383        | 65,024                 | In the middle                                                                           |
| C             | 192.168.0.0-255 | 255.255.255.0 | 2,097,151     | 254                    | Used by normal people and support up to 254 devices which is more than enough for most. |
- Network mask, or subnet mask, is basically telling the computer which part of the IP address is the "==network==" part and which is the "==host==" part
	- Ex: 192.168.219.199 with the subnet mask 255.255.255.0 tells the computer that the first 3 numbers are the "network" and the last number is the "host"
- What are the network and host parts of an ip-address?
	- The network part is unique across the whole world, and is used as the ip for a router pretty much.  This is why class A ip-addresses are so rare; since they only have a few numbers to use as identifiers, only super giant organizations use these.
	- The host part is unique across only the network, so my phone could have 192.168.219.0 and my laptop could have 192.168.219.1.  These several ==private ip-addresses== use #NAT to then get routed to the internet using the network part of the ip
- An example of a class B ip address:
	 ![[classBexample.png]]

What is an #MAC-address?
- Allows ==switching== in #layer-2 
	- A switch is basically a device that transfers data from one computer over to another specific computer using the MAC address
- Sort of like a physical address; shows what device is what
	- ex: A MAC address can be used to tell if the device is a cellphone, laptop, etc.
- The first 3 pairs of two makes up the ==identifier== which can be put into a MAC address lookup to determine what type of device it is

What is #TCP and #UDP?
- TCP and UDP are 
