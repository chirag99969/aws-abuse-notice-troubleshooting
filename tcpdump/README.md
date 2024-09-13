# tcpdump network analysis
 
 ```
  123  tcpdump -r -vv -A -nn -i any dump.pcap 
  124  tcpdump -r -nn dump.pcap 
  125  tcpdump -r  dump.pcap 
  126  tcpdump -r port 80  dump.pcap 
  127  tcpdump -r  dump.pcap  port 80
  128  tcpdump -r  dump.pcap  port 80 src 192.168.0.0
  129  tcpdump -r  dump.pcap  src 192.168.0.0
  130  tcpdump -r  dump.pcap  icmp
  131  tcpdump -r  dump.pcap  tcp
  132  tcpdump -r  dump.pcap  udp
  133  tcpdump -r  dump.pcap  -S
  134  tcpdump -r  dump.pcap  " port 80 and src 192.168.0.0"
  135  tcpdump -r  dump.pcap  " port 80 and src 192.168.0.0" tcp
  136  tcpdump -r  dump.pcap  " port 80 and src 192.168.0.0 and icmp"
  137  tcpdump -r  dump.pcap  " port 80 and src 192.168.0.174 and udp"
  138  tcpdump -r  dump.pcap  " port 80 and src 192.168.0.174"
  139  tcpdump -r -c5  dump.pcap  " port 80 and src 192.168.0.174"
  140  tcpdump -c5 -r dump.pcap  " port 80 and src 192.168.0.174"
  141  tcpdump -c5 -r dump.pcap  " port 443 and src 192.168.0.174"
  142  tcpdump -c5 -A -r dump.pcap  " port 443 and src 192.168.0.174"
  143  tcpdump -c5 -A -r dump.pcap  " port 80 and src 192.168.0.174"
  144  tcpdump -c100 -A -r dump.pcap  " port 80 and src 192.168.0.174"
  145  tcpdump -c100 -A -vvv -r dump.pcap  " port 80 and src 192.168.0.174"
  146  tcpdump -c100 -A -vvv -r dump.pcap src 192.168.0.174
  147  tcpdump -c200 -A -vvv -r dump.pcap src 192.168.0.174
```
