Usage scanner.py: python scanner.py [pcap file]

Only input one pcap file at a time.

Scanners:

Portscan - if packet is TCP or UDP, it checks if the destination has been checked for other ports, if greater than or equal to 100 it alerts.

SYN flood - If packet is TCP, it creates a unique identifier for destination and port, checks if the timestamp is less than one second for the total packets then if there are greater than 100 in a second, alerts for the destination

ARP spoofing - if packet is type ARP, checks if the MAC in the packet matches the MAC in the network config that was given for IP:MAC tuples. If not matching, prints alert.
