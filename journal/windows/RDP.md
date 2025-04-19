
##  Remote Desktop Protocol (RDP)

RDP is a Windows machine protocol for remote access. RDP is popular remote access protocol and is the default remote connection protocol between Microsoft Azure and Hyper-V platforms. The protocol is complex with many extensions, which boils down to higher risk of critical bugs and vulnerabilities for exploitation.

### Illustration 
### Local Machine -> RDP Client -> RDP Server

RDP comunication is asymmetric, most data will go from server to client.
#### Client --INPUT DATA--> Server
#### Client <==OUTPUT DATA== Server
RDP communication is encrypted with RSA's RC4 block cipher by default

### RDP protocol stack

RDP - Remote Access

Encryption - encrypt (scramble data) 

T.125 MCS - handles multiple channel (keyboard, mouse, screen resolution) (encryption methods, size of sesision keys, server random server certificate)

X.224 - handshake to establish reliable connection

TPKT / TLS - packages data into chunks / optional TLS to secure channel before sending. 

TCP - Transmission Control Protocol
