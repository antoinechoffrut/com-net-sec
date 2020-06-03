---
toc: true
layout: post
title: IP addressing
description: Classful network addressing, reserved blocks, etc.
categories: [cheatsheet, networking]
---


# IPv4 classes
<table width="100%">
  <tr>
    <th width="15%"></th>
    <th width="15%">class A</th>
    <th width="15%">class B</th>
    <th width="15%">class C</th>
    <th width="15%">class D</th>
    <th width="15%">class E</th>
  </tr>
  <tr>
  <th>leading bits</th>
    <td>0</td>
    <td>10</td>
    <td>110</td>
    <td>1110</td>
    <td>1111</td>
  </tr>
  <tr>
    <th>subnet mask</th>
    <td>255.0.0.0</td>
    <td>255.255.0.0</td>
    <td>255.255.255.0</td>
    <td>N/A</td>
    <td>N/A</td>
  </tr>
  <tr>
    <th>public range</th>
    <td>1.0.0.0<br>126.255.255.255</td>
    <td>128.0.0.0<br>191.255.255.255</td>
    <td>192.0.0.0<br>223.255.255.255</td>
    <td>224.0.0.0<br>239.255.255.255</td>
	<td>240.0.0.0<br>255.255.255.255</td>
  </tr>
  <tr>
    <th>private range<br>(dot decimal)</th>
    <td>10.0.0.0<br>10.255.255.255</td>
    <td>172.16.0.0<br>172.31.255.255</td>
    <td>192.168.0<br>192.168.255.255</td>
    <td></td>
	<td></td>
  </tr>
  <tr>
    <th>private range<br>(CIDR)</th>
    <td>10.0.0.0/8</td>
    <td>172.16.0.0/12</td>
    <td>192.168.0.0/16</td>
	<td></td>
	<td></td>
  </tr>
  <tr>
    <th>nb of subnets</th>
    <td>126</td>
    <td>16,384</td>
    <td>2,097,152</td>
	<td></td>
	<td></td>
  </tr>
  <tr>
    <th>nb of hosts<br>per network</th>
    <td>16,277,214</td>
    <td>65,534</td>
    <td>254</td>
	<td></td>
	<td></td>
  </tr>
</table>



# Reserved blocks  

<table width="100%">
  <tr>
    <th width="10%">block</th>
    <th width="20%">address range</th>
    <th width="30%">note</th>
  </tr>
  <tr>
    <td>0.0.0.0/8</td>
    <td>0.0.0.0 - 0.255.255.255</td>
    <td>reserved for self-identification</td>
  </tr>
  <tr>
    <td>127.0.0.0/8</td>
    <td>127.0.0.0 - 127.255.255.255</td>
    <td>reserved for loopback</td>
  </tr>
  <tr>
    <td>169.254.0.0/16</td>
    <td>169.254.0.0 - 169.254.255.255</td>
    <td>link-local addressing</td>
  </tr>
</table>

# Appendix: Binary arithmetics

## Powers of 2

| exponent | power |
|----------|-------|
| 0        | 1     |
| 1        | 2     |
| 2        | 4     |
| 3        | 8     |
| 4        | 16    |
| 5        | 32    |
| 6        | 64    |
| 7        | 128   |
| 8        | 256   |
| 9        | 512   |
| 10       | 1024  |

## Masks

| mask (binary) | mask (decimal) | detail      |
|---------------|----------------|-------------|
| 1111 1111     | 255            | = 256 - 1   |
| 1111 1110     | 254            | = 256 - 2   |
| 1111 1100     | 252            | = 256 - 4   |
| 1111 1000     | 248            | = 256 - 8   |
| 1111 0000     | 240            | = 256 - 16  |
| 1110 0000     | 224            | = 256 - 32  |
| 1100 0000     | 192            | = 256 - 64  |
| 1000 0000     | 128            | = 256 - 128 |

