---
layout: post
category: Log
title: An idea on IPv6 addressing..
---

**IPv6 addressing.**

We have all heard about  IPv6...Let's go through some basic information regarding this,

IPv6 brings larger address space than IPv4. **IPv4=32 bits ----> IPv6=128 bits** **x : x : x : x : x : x : x : x  **represents this 128 bit long address where, x is 16 bit hex field.In which the last 64 bit used as Interface ID. for example,consider one IPv6

**2001 : 0DB8 : C003 : 0001 : 0000 : 0000 : 0000 : F00D**

here,the leading zeros can be avoided and it becomes

**2001 : 0DB8 : C0D3 : 1 : 0 : 0 : 0 : F00D**

here we can replace consecutive zeros by double colon  '**::**' (only used once) and it becomes

**2001 : 0DB8 : C0D3 : 1 :: F00D**

                 
  |/12  |/32    |/48    |/64 
         
  2001 ** :**  0DB8  **:**** :**** :**Interface ID 
  Registry --->|      |          |        | 
  ISP Prefix ---->    |          |        | 
  Site Prefix ---->              |        | 
  Subnet Prefix  ----->                   | 
          
 The address allocation follows a generally accepted assignment policy. 
          
 Address types are many: Unicast(ont-to-one),Anycast(one-to -nearest),Multicast(ont-to many).(you can google more about it). 
          
 We can see the interface id  above and this single interface may be assigned multiple addresses of any type. Every IPv6 enabled interface must contain at least one **loop back*** and one -link local address. 
          
      IPv6 host address can be assigned in multiple ways: 
      static configuration 
      stateless 
      auto-configuration 
      DHCPv6 
      
 When IPv6 is used over Ethernet Networks,the ethernet MAC address can be used to generate 64 bit interface ID for host,called EUI-64 address. MAC address use 48 bits (check '**ifconfig**' command in terminal to get MAC address of your machine) additional bits must be inserted to fill 64 bits required. 
 
 * Loopback address is a special IP number (127.0.0.1) that is designated for the software loopback interface of a machine. The loopback interface has no hardware associated with it, and it is not physically connected to a network.

*link: https://rosnikv92.wordpress.com/2012/08/25/ipv6-addressing-basics/
author: rosnikv
description: 
post_id: 60
created: 2012/08/25 13:26:10
created_gmt: 2012/08/25 13:26:10
comment_status: open
post_name: ipv6-addressing-basics
status: publish
post_type: post
*
## Comments

**[Arjun](#7 "2012-08-28 16:13:38"):** Could get some info about the topic....thanks

