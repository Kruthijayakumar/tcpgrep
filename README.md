# tcpgrep
 We developed  a command line tool called Tcpgrep by giving pcapfile as input. that can be used to filter TCP traffic using c language. It can be used to filter traffic based on a variety of criteria, including source and destination IP addresses, ports, and protocols. Tcpgrep can also be used to filter traffic based on the contents of the packets.  
o	For displaying help option ,
   tcpgrep pcapfilename

o	To display the total number of  tcp packets,
tcpgrep pcapfile name -t

o	To display the total number of incomplete tcpsession,
tcpgrep pcapfile name -i

o	To display the incomplete tcpsessions with packet numbers,
tcpgrep pcapfile name -in

o	To display the total number of rst packets,
tcpgrep <pcapfile name> -r

o	To display the total rst packets with packet number,
tcpgrep pcapfile name -rn

o	To display the total number of duplicate ack packets,
tcpgrep pcapfile name -a

o	To display the total number of duplicate ack packets with packet number,
tcpgrep pcapfile name -an

o	To dump specific range of tcp packet,
tcpgrep pcapfile name -p packet range start – end range
example: tcpgrep pcap1.pcap -p 2-10 

o	To dump specific range of ports,
tcpgrep pcapfile name -p: ip address:port no
 
example: tcpgrep pcap1.pcap -p 192.168.4.5:443

o	To dump specified tcpflags,
tcpgrep pcapfile name -pflags: A,P,F,U,S,R
 example : tcpgrep pcap1.pcap -pA ,-pF,-pS,-pU,-pR,-pP
       

