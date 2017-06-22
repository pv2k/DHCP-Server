### DHCP Server

> Simple server that listens to client requests and assign appropriate IP address and subnet mask. The server has to allocate the address depending upon which lab the client belongs to and ssend it back to the client.

### Input: 
The server listens to client requests and assign appropriate IP address and subnet mask. The server has to allocate the address depending upon which lab the client belongs to and ssend it back to the client.
The Server will read from a file “​ subnets.conf​ ”, which will have the following format:
1st Line - Generic Network Address with CIDR
2nd Line - Number of labs:​ n
Next ​ n ​ lines - Lab_name<colon>capacity
Next to end of file- MAC Address<space>Lab_name
Run the server and in another terminal, execute this:
<pre>
./client -m <mac_address>
</pre>
If the -m parameter is omitted (i.e. mac is omitted), it reads the MAC address of the appropriate interface of the system it is being run from.

### Outputformat:
-> IP address with subnet(CIDR format)
-> Network address
-> Broadcast address
-> Default Gateway
-> Default DNS
-> Subnet mask

For additional test cases, look into the "testcases" folder and copy them into subnets.conf
