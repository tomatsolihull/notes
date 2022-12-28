#networking
# Dynamic Host Configuration Protocol

- Distributes [[zk/IP]] Addresses and other information to hosts on a network
- Uses [[zk/UDP]] Port 67 on server, 68 on client

## The Process
More detail [on Wikipedia](https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol) and within [[zk/IETF#RFC]] [RFC 2131](https://datatracker.ietf.org/doc/html/rfc2131#section-3)

### 1. DHCPDISCOVER (client broadcast)
From client to broadcast address to 'discover' DHCP servers on a network
Can also be used to request current IP address from an authoritative server.

### 2. DHCPOFFER (server to client)
Server offers an IP address/details

### 3. DHCPREQUEST (client to server)
Client requests the IP address previously offered

### 4. DHCPACK (server to client)
Server acknowledges the request

At each stage, the client can specify which parameters it is interested in (parameter request list) and the maximum size of the DHCP reply from the server.