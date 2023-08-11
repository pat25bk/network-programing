# network-programing
## Summary
Notes and resources of network programing
## Notes
<p>
- The OSI seven layers stack is an old network architecture, the modern one is TCP/IP stack/model with just 4 layers:
<ol>
  <li>Application layer: each type of application use its specific protocal, for example HTTP protocal for web app, SMTP/IMAP/POP3 protocals for email, SSH for remote access</li>
  <li>Transprot layer: use two common protocals: TCP and UDP, the source and destination port are be added at this layer </li>
  <li>Internet layer: the source and destimation IP address are added at this layer </li>
  <li>Network access layer (Datalink layer): use protocols such as Ethernet, wifi, 4g for transmiting data over media environment (wireless/wired), the source and destination MAC address is added heare </li>
</ol>
- In Linux OS, the linux kernel handles the transport and internet layer, and provide abstract networking interface to applications in user space with the SOCKET concept. A socket is a abstruct communication channel is associated with an IP address, a transport layer protocal (TCP/UDP) and a port number. After creating a socket, applications now only need to use APIs from socket library like listen(), connect(), recv() and transmit()
</p>

## Resources
<ol>
  <li>Introduction about TCP/IP stack: https://isaaccomputerscience.org/concepts/net_internet_tcp_ip_stack?examBoard=all&stage=all</li>
  <li>Socket programing with Linux kernel: https://linux-kernel-labs.github.io/refs/heads/master/labs/networking.html </li>
</ol>
