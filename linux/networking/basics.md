# Networking Basics

## TCP/IP Model

- Application Layer
  HTTP/SMTP
  uses packets

- Transport Layer
  TCP / UDP
  uses "Segments"
  attaches ports

- Network Layer
  IP
  ICMP - Internet Control Message Protocol - handles error messages, debugging information
  uses "IP packets"
  attaches IP addresses

- Link Layer
  Physical hardware - Ethernet/Fiber, etc..
  uses "Frames"
  attaches mac addresses

---

1. The application layer talks to the transport layer through a specified "port"

1. The transport layer breaks down data into chunks,
   attaches source and destination ports

1. The network layer adds source and destination IP addresses

1. The link layer adds the source and destination MAC addresses, checksum
   packet separators
