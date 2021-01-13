---
title: Basics - Dns
date: 2020-12-21T06:52:36+00:00
image_webp: images/blog/blog-post-1.webp
image: images/blog/blog-post-1.jpg
author: John Doe
description: ''

---
##### **What is it?**

It stands for "Domain Name Server".

#####  **How does it work?**

As we already know, computers interact with each other using IP addresses which isn't human friendly, at all. So words (say _anupasusan.com_) is used instead of the IP address (say 192.124.246.899). DNS, being the hero in cape, brings two and two together and displays the address. 

_Domain names_ are responsible for connecting the IP address to the alphabetic website name.

Let me explain how this works in four simple steps:

1. You open the address bar in browser and hit _anupasusan.com_ upon which an immediate search is conducted to see if you have visited the site previously. If DNS records are discovered in the DNS cache, then it is retrieved and rest of DNS lookup is skipped and you are taken directly to _anupasusan.com_.
2. If no DNS records are found, then a query is send to your local DNS server which is typically your internet provider's server and is called "resolving nameserver".
3. If the DNS records are also not cached in the resolving nameserver, it is then directed to the "root nameservers" which are nameservers around the world for storing DNS data and keep it functioning smoothly. Once DNS recornds are found in the root nameserver, it is cached by the computer.
4. Now that the records are located, the connection to the server where the website is stored will open and _anupasusan.com_ will be displayed on screen.

   ##### What is a Nameserver?

   It is simply a server that keeps all the DNS records of your domain name. It's job is to provide your records to anyone asking for it. 

   Each domain name has at atleast two nameservers out of which one acts as primary nameserver. If the primary nameserver doesn't respond, then secondary nameserver(s) comes into action.

   ##### What is CName record?

   CName stands for Canonical Name. A CName record is basically a record that is used to point one domain name to another, instead of an IP address. 

   Example, your website is _anupasusan.com_ but you have also registered for _anupa.com_ and you want it to point it to the main website. In that case you setup a CName record which will direct anyone who visits _anupa.com_ to _anupasusan.com_ instead.

   ##### Some other terminologies you should know:
   * **TLD**: aka Top Level Domain

     the last part of the domain name that comes after the dot

     Example: .COM, .NET, .ORG
   * **Subdomain**: this is the additional part to your domain to your main domain name. They are created usually to navigate to different sections of your website. You can create multiple child domains/ subdomains on your primary website.

     Example: _store.anupasusan.com_

     where _store_ is subdomain, _anupasusan_  is the primary domain and _.com_ is the TLD.
   * **DNS zone:** A DNS Zone represents the domain name space that is managed by a single Authoritative Name Server. A DNS Zone resides on its Authoritative Name Server and contains multiple DNS entries for each sub-domain.
   * **'A' Record:** The address record maps domain name to an IP address.
   * **Naked Domain:** This is simply a domain name without the subdomain prefix.