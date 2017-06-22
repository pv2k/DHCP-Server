README

1) The server will have have some IP in the given address range. It will
output it.
2) Later on the server will then listen to the client requests and it will
assign appropriate IP addresses and subnet mask upon receiving a request
from the client.
3) The client will identify itself to the server with its own MAC.
4) The server will allocate addresses depending upon which lab the client
belongs to. And it will return this back to client.

5) The server will send back the IP address with subnet in CIDR format,
Network address, broadcast address, sample gateway, sample DNS.

6) Otherwise it will send error msgs/

7) It will assign an IP address to the client whose MAC address is not
registered in the subnets.conf file.
