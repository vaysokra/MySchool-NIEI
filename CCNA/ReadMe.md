### IP ADDRESS
#####   CLASS OF NETWORK
- class A = 1 -> 127(SM) : 255(N) . 0(H) . 0(H) . 0(H)/8    {N=network , H=Host}
- class B = 128 -> 191(SM) : 255(N) . 255(N) . 0(H) . 0(H)/16
- class C = 192 -> 223(SM) : 255(N) . 255(N) . 255(N) . 0(H)/24
#####   IP
- ip of network : 192.168.0.**0**
- ip of device : 192.168.0.**[1->253]** => ex: 192.168.0.4
##### CALCULATE IP of Router
- A= 192 .  168 . 0 . 1 =covert to binary= 11000000 . 10101000 . 00000000 . 00000001
- B= 225 . 255 . 255 . 0 =covert to binary= 11111111 . 11111111 . 11111111 . 00000000
- A and-operator B = 11000000 . 10101000 . 00000000 . 00000000
##### Network Address Translation(NAT)
##### OSI
- application layer
- presentation layer
- session layer
- transportation layer
- network layer
- data link layer 
- physical layer
##### numbers of subnet (N=network , H=host)
- 193.15.0.000|00000 / 24 -> 27
- =>SubnetMask : 255(N).255(N).255(N).224(N) | 0(H)/27  
- N = 2^n - 2       // n : bit ខ្ចី   example : N = 2^3 - 2 = 6 Networks
- Spc = 2^n - 2     // n : bit នៅសល់  example : Spc = 2^5 - 2 = 30 Addresses
- => N1 = 193.15.0.32/27 => we got Spc[1->30] = 193.15.0.[34->63]  ex: Spc1 = 193.15.0.34
- => N2 = 193.15.0.64/27 => we got Spc[31->60] = 193.15.0.[65->94] ex: Spc31 = 193.15.0.64 
- => N3 = 193.15.0.96/27    
- => N4 = 193.15.0.128/27   
- => N5 = 193.15.0.150/27   
- => N6 = 193.15.0.192/27   
- ===> we got 6 Networks and each with 30 addresses
- 193.15.0.0/27 => subnet Mask : 255.255.255.224
