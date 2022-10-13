# wireshark-demo
Wireshark inable in k8s server

1.sudo groupadd pcap
2.sudo usermod -a -G pcap $USER
3.sudo chgrp pcap /usr/sbin/tcpdump
4.sudo chmod 750 /usr/sbin/tcpdump
5.sudo setcap cap_net_raw,cap_net_admin=eip /usr/sbin/tcpdump
6.sudo tcpdump -s 0 -i eth0 -w tcpdump.pcap


Wireshark is a network protocol analyzer, or an application that captures packets from a network connection, such as from your computer to your home office or the internet. Packet is the name given to a discrete unit of data in a typical Ethernet network.

Wireshark is the most often-used packet sniffer in the world. Like any other packet sniffer, Wireshark does three things:

Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic – quite possibly tens of thousands of packets at a time.
Filtering: Wireshark is capable of slicing and dicing all of this random live data using filters. By applying a filter, you can obtain just the information you need to see.
Visualization: Wireshark, like any good packet sniffer, allows you to dive right into the very middle of a network packet. It also allows you to visualize entire conversations and network streams.
