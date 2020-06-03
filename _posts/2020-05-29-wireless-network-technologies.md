---
toc: true
layout: post
title: Wireless network technologies
description: IEEE 802.11, Bluetooth, Zigbee and Z-Wave
categories: [cheatsheet, wireless, protocols]
---


# The 802.11 standards
<table>
  <tr>
    <th>standard</th>
	<th>freq</th>
	<th>max<br>throughput<br>(total)</th>
	<th>max<br>MIMO<br>streams</th>
	<th>max<br>throughput<br>(per stream)</th>
	<th>band-<br>width</th>
	<th>max<br>range<br>(indoor)</th>
	<th>back-<br>ward<br>compat-<br>ibility</th>
	<th>year</th>
  </tr>
  <tr>
    <td>802.11<b>a</b></td>
    <td>5.0 GHz</td>
	<td>54 Mbps</td>
	<td> - </td>
	<td>54 Mbps</td>
	<td>20 MHz</td>
	<td>35 m</td>
	<td> - </td>
	<td>1999</td>
  </tr>
  <tr>
    <td>802.11<b>b</b>               </td>
	<td>2.4 GHz            </td>
	<td>11 Mbps                        </td>
	<td> - </td>
	<td>11 Mbps</td>
	<td>22 MHz                 </td>
	<td>35 m                   </td>
	<td>-                          </td>
	<td>1999</td>
  </tr>
  <tr>
    <td>802.11<b>g</b>               </td>
	<td>2.4 GHz            </td>
	<td>54 Mbps                        </td>
	<td> - </td>
	<td>54 Mbps</td>
	<td>20 MHz                 </td>
	<td>38 m                   </td>
	<td>802.11<b>b</b>                </td>
	<td>2003</td>
  </tr>
  <tr>
    <td>802.11<b>n</b></td>
	<td>2.4 GHz<br>5.0 GHz </td>
	<td>600 Mbps</td>
	<td>4 MIMO</td>
	<td>150 Mbps</td>
	<td>24, 40 MHz             </td>
	<td>70 m                   </td>
	<td>802.11<b>a</b>/<b>b</b>/<b>g</b></td>
	<td>2009</td>
  </tr>
  <tr>
    <td>802.11<b>ac</b></td>
	<td>5.0 GHz            </td>
	<td>6.8 Gbps </td>
	<td>8 MU-MIMO</td>
	<td>866.7 MHz</td>
	<td>20, 40,<br>80, 160 MHz </td>
	<td>35 m                   </td>
	<td>802.11<b>a</b>/<b>n</b>          </td>
	<td>2013</td>
  </tr>
</table>


## Channels and frequencies

<table>
  <tr>
    <th width="10%">band name</th>
	<th width="40%">frequency band</th>
	<th>non-overlapping 20 MHz-wide channels</th>
  </tr>
  <tr>
    <td>2.4 GHz</td>
	<td>2.400-2.500GHz</td>
	<td>3 (&#35;1, &#35;6, &#35;11 of 11 available)</td>
  </tr>
  <tr>
    <td>5.0 GHz</td>
	<td>4.915–5.825 GHz</td>
	<td>23</td>
  </tr>
</table>

# Bluetooth
- Bluetooth is a short-range wireless interconnetion of mobile phones,
  computers and other electronic devices.
- Devices operate in the 2.4 to 2.485 GHz radio frequency range and
  are typically used for PANs.


## Classification

|                          | max. permitted power | approximate distance |
|--------------------------|----------------------|----------------------|
| class 1                  | 100 mW               | ~330 ft (100 m)      |
| class 2<br>(most common) | 2.5 mW               | ~30 ft (10 m)        |
| class 3                  | 1 mW                 | ~3 ft (1 m)          |

## Specifications

| specification | version    | data transfer rate                 |
|---------------|------------|------------------------------------|
| 1.0           | v1.2       | 1 Mbps                             |
| 2.0           | v2.0 + EDR | 3 Mbps                             |
| 3.0           | v3.0 + HS  | 24 Mbps                            |
| 4.0           | v4.0 + LE  | 1 Mbps                             |
| 5.0           | v5.0 + LE  | 125 Kbps, 500 Kbps, 1 Mbps, 2 Mbps |

# References
- Professor Messer:
  - [802.11 wireless standards - CompTIA A+ 220-1001](https://www.professormesser.com/free-a-plus-training/220-1001/802-11-wireless-standards/)
  - [Wireless network technologies - CompTIA A+
    220-1101](https://www.professormesser.com/free-a-plus-training/220-1001/wireless-network-technologies-2/)
  - [Wireless interface speeds and distances - CompTIA A+
    220-901](https://www.professormesser.com/free-a-plus-training/220-901/wireless-interface-speeds-and-distances/)
- Wikipedia:
  - [IEEE 802.11: Protocol](https://en.wikipedia.org/wiki/IEEE_802.11#Protocol)
  - [IEEE 802.11: Channels and frequencies](https://en.wikipedia.org/wiki/IEEE_802.11#Channels_and_frequencies)
  - [Bluetooth](https://en.wikipedia.org/wiki/Bluetooth)
- [David Bigger](https://www.biggeritsolutions.com), CompTIA A+ course
- [Metis: WiFi 5GHz band and wide
  channels](https://metis.fi/en/2018/02/5ghz-channels/)
- [Flylib: The Bluetooth
  protocol](https://flylib.com/books/en/4.215.1.116/1/) 
