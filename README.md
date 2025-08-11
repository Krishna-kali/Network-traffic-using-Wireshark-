# Network-traffic-using-Wireshark-
Capturing and Analysis network traffic using Wireshark 
1. Installation & Setup
Download: wireshark.org
Install:
Enable Npcap (Windows) or libpcap (Linux/macOS) during setup.
(Optional) Install command-line tools (tshark, dumpcap).
Wireshark is a powerful, open-source network protocol analyzer that allows users to capture and interactively browse the traffic running on a computer network, providing deep inspection of hundreds of protocols.

2. Capturing Traffic
Launch Wireshark (as administrator/root).
Select Interface:Choose an active interface (e.g., Wi-Fi, Ethernet). Look for  traffic spikes.
Avoid any/all interfaces (can be overwhelming).

Start Capture:
Click the Wireshark icon or press Ctrl+E.
Generate Traffic:Browse a website, ping an IP, or run curl ifconfig.me.

Stop Capture:Click the red square or press Ctrl+E again.
![image alt](
3. Basic Analysis Techniques
A. Filter Traffic
ip.addr == 192.168.1.100 -	Traffic to/from a specific IP.
tcp.port == 80 -	HTTP traffic.
udp.port == 53 - DNS queries.
icmp - 	Ping/ICMP packets.
http -	HTTP requests/responses.
tcp.flags.syn == 1 -	TCP connection requests (SYN).
dns -	All DNS traffic.
