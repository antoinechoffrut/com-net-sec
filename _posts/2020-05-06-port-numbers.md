---
toc: true
layout: post
title: Common TCP and UDP port numbers
description: Definitions and port numbers
categories: [cheatsheet, networking, protocols]
---


# Protocols: TCP vs UDP
<table>
  <tr>
    <th width="10%">protocol</th>
	<th width="40%">TCP</th>
	<th>UDP</th>
  </tr>
  <tr>
    <td>full name</td>
    <td> Transmission Control Protocol
	</td>
	<td> User Datagram Protocol
	</td>
  </tr>
  <tr>
    <td>connection</td>
    <td> connection-oriented 
	</td>
	<td> connection-less
    </td>
  </tr>
  <tr>
    <td>reliability</td>
    <td> reliable
	</td>
	<td> unreliable
    </td>
  </tr>
  <tr>
    <td>error checking</td>
    <td> error checking and recovery
	</td>
	<td> error checking, no recovery
    </td>
  </tr>
  <tr>
    <td>acknowledgment</td>
    <td>acknowledgment
	</td>
	<td> no acknowledgment
    </td>
  </tr>
</table>

# Port number ranges
See Section 6, page 10 of [RFC6335](https://www.rfc-editor.org/rfc/rfc6335.txt).

| name                                              | range         | assigned by |
|---------------------------------------------------|---------------|-------------|
| well-known ports<br>system ports                  | 0 - 10234     | IANA        |
| user ports<br>registered ports                    | 1024 - 49151  | IANA        |
| dynamic ports<br>private ports<br>ephemeral ports | 49152 - 65535 | never            |


# Common TCP and UDP port numbers
This is the list from the the CompTAI A+ Certification Exam: Core 1
Objectives 220-1001.


| service                       | protocol/port number               |
|-------------------------------|------------------------------------|
| FTP                           | TCP/20 (data)<br>TCP/21 (control)  |
| SSH                           | TCP/22                             |
| Telnet                        | TCP/23                             |
| SMTP                          | TCP/25                             |
| DNS                           | UDP/53                             |
| DHCP                          | UDP/67 (server)<br>UDP/68 (client) |
| HTTP                          | TCP/80                             |
| POP3                          | TCP/110                            |
| IMAP4                         | TCP/143                            |
| NetBIOS<br>(name service)     | UDP/137                            |
| NetBIOS<br>(datagram service) | UDP/138                            |
| NetBIOS<br>(session service)  | TCP/139                            |
| SNMP                          | UDP/161 (get)<br>UDP/162 (trap)    |
| LDAP                          | TCP,UDP/389                        |
| SLP                           | TCP,UDP/427                        |
| HTTPS                         | TCP/443                            |
| SMB<CIFS>                     | TCP/445                            |
| AFP                           | TCP/548                            |
| RDP                           | TCP/3389                           |

Additional ports 

| service | protocol/port number |
|---------|----------------------|
| POP3S   | TCP/995              |
| IMAPS   | TCP/993              |
| PDL     | TCP/9100             |
| RADIUS  | TCP,UDP/1812         |


# Acronyms and descriptions

<table>
  <tr>
    <th width="10%">service</th>
	<th width="40%">name</th>
	<th>description</th>
  </tr>
  <tr>
    <td> FTP     </td>
	<td> File Transfer Protocol                </td>
	<td> send and receive files between systems
  </td>
  </tr>
  <tr>
    <td> SSH     </td>
	<td> Secure SHell                          </td>
	<td> encrypted console access
  </td>
  </tr>
  <tr>
    <td> Telnet  </td>
	<td> Telecommunication Networrk            </td>
	<td> insecure consle access
  </td>
  </tr>
  <tr>
    <td> SMTP    </td>
	<td> Simple Mail Transfer Protocol         </td>
	<td> transfer emails between servers
  </td>
  </tr>
  <tr>
    <td> DNS     </td>
	<td> Domain Name System                    </td>
	<td> convert domain names into IP addresses
  </td>
  </tr>
  <tr>
    <td> DHCP    </td>
	<td> Dynamic Host Configuration Protocol   </td>
	<td> automated configuration of IP addresses
  </td>
  </tr>
  <tr>
    <td> HTTP    </td>
	<td> HyperText Transfer Protocol           </td>
	<td> web server communication
  </td>
  </tr>
  <tr>
    <td> POP3    </td>
	<td> Post Office Protocol v3               </td>
	<td> email client protocol
  </td>
  </tr>
  <tr>
    <td> POP3S   </td>
	<td> POP3 Secure                           </td>
	<td> email client protocol with encryption
  </td>
  </tr>
  <tr>
    <td> IMAP4   </td>
	<td> Internet Message Access Protocol v4   </td>
	<td> email client protocol
  </td>
  </tr>
  <tr>
    <td> IMAPS   </td>
	<td> IMAP Secure                           </td>
	<td> email client protocol with encryption
  </td>
  </tr>
  <tr>
    <td> HTTPS   </td>
	<td> HTTP Secure                           </td>
	<td> web server communication with encryption
  </td>
  </tr>
  <tr>
    <td> NetBIOS </td>
	<td> NetBIOS name service                  </td>
	<td> register, remove, and find Windows service by name
  </td>
  </tr>
  <tr>
    <td> NetBIOS </td>
	<td> NetBIOS datagram service              </td>
	<td> Windows connection-less data transfer
  </td>
  </tr>
  <tr>
    <td> NetBIOS </td>
	<td> NetBIOS session service               </td>
	<td> Windows connection-oriented data transfer
  </td>
  </tr>
  <tr>
    <td> SNMP    </td>
	<td> Simple Network Management Protocol    </td>
	<td> gather statistics from networks
  </td>
  </tr>
  <tr>
    <td> LDAP    </td>
	<td> Lightweight Domain Access Protocol    </td>
	<td> management and authentication on network
  </td>
  </tr>
  <tr>
    <td> SLP     </td>
	<td> Service Location Protocol             </td>
	<td> (macos?) service discovery
  </td>
  </tr>
  <tr>
    <td> SMB     </td>
	<td> Server Message Block                  </td>
	<td> Windows file transfer and printer sharing
  </td>
  </tr>
  <tr>
    <td> CIFS    </td>
	<td> Common Internet File System           </td>
	<td> Windows file transfer and printer sharing
  </td>
  </tr>
  <tr>
    <td> AFP     </td>
	<td> Apple Filing Protocol                 </td>
	<td> macos file transfer
  </td>
  </tr>
  <tr>
    <td> RDP     </td>
	<td> Remote Desktop Protocol               </td>
	<td> graphical display of remote devices
  </td>
  </tr>
  <tr>
    <td> PDL     </td>
	<td> Page Description Language data stream </td>
	<td> raw data stream for printing
  </td>
  </tr>
  <tr>
    <td> SLP     </td>
	<td> Service Location Protocol             </td>
	<td> service discovery protocol
  </td>
  </tr>
  <tr>
    <td> AFP     </td>
	<td> Apple File Protocol                   </td>
	<td> Apple's proprietary file sharing network protocol
  </td>
  </tr>
  <tr>
    <td> RADIUS  </td>
	<td> Remote Authentication<br>             </td>
	<td>
  </td>
  </tr>
</table>

# References
- [IANA: Service names and transport protocol port number
  registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml)
  ([RFC6335](https://tools.ietf.org/html/rfc6335))
- RFC1700: [.txt](https://www.ietf.org/rfc/rfc1700.txt),  [.pdf](https://www.ietf.org/rfc/rfc1700.txt.pdf) (ietf.org)
- Wikipedia: [Well-known
  ports](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers#Well-known_ports),
  in "List of TCP and UDP port numbers"
