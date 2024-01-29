---
title: "What the DNS! Guide to everything DNS"
datePublished: Thu Dec 15 2022 12:21:34 GMT+0000 (Coordinated Universal Time)
cuid: clbp1wc6e000108ma4ahz9pi1
slug: what-the-dns-guide-to-everything-dns
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1671106828168/z7Dx_hATw.png
tags: dns, web-development, webdev, frontend-development

---

DNS is me banging my head after debugging 30 billion hours to know that I messed up the DNS, so here's a DNS guide to make sure that you don't fuck up and waste 30 billion hours of uh, debugging hours.

## What is DNS?

So before domain names were born, people used to visit websites by typing in IP addresses (just more complicated phone numbers), which means, I would have to type 76.76.21.21, to go to hashnode.com

Wow, I can't even remember how to centre a div in CSS, and I have to remember that 8 number digits to go to Hashnode and write about my broken code!?

Then the big brains invented domain names, which are a collection of words in a weird format (eg: www.google.com) that is translated to an IP address, so if I type hashnode.com it will just translate to the IP.

To make this they also had to make something called DNS which could tell your computer what translates to what.

## How does DNS work?

![What is DNS? | How DNS works | Cloudflare](https://www.cloudflare.com/img/learning/dns/what-is-dns/dns-record-request-sequence-3.png align="left")

But of course, it doesn't mean that it is so simple, we are developers, so of course, we built it in such a way:

*   Ask DNS Recursive Resolver to find DNS
    
*   DNS Recursive Resolver asks DNS Root Nameserver which tells idk what you want but I know someone (DNS TLD Server) who might know
    
*   DNS Recursive Resolver asks DNS TLD Server which tells idk what you want but I know someone (Authoritative Nameserver) who might know
    
*   DNS Recursive Resolver asks Authoritative Nameserver and gets the answer finally!!!
    

![25+ Best Dns Memes | Uns Memes, Holt Memes, Oder Memes](https://pics.me.me/thumb_lets-just-say-i-know-a-guy-who-knows-a-guy-57609338.png align="left")

## Common DNS Records

*   **A record**: Maps a domain name to an IP address. This is the most commonly used DNS record and is used to direct traffic to a specific server.
    
*   **AAAA record**: Maps a domain name to an IPv6 address. This is similar to an A record but is used for IPv6 addresses instead of IPv4 addresses.
    
*   **CNAME record**: Maps a domain name to another domain name. This is used to create an alias for a domain so that multiple domain names can be pointed to the same IP address.
    
*   **MX record**: Specifies the mail server responsible for accepting email messages for a domain. This record is used to route emails for a domain to the correct server.
    
*   **NS record**: Specifies the authoritative DNS servers for a domain. This record is used to delegate control of a subdomain to another DNS server.
    
*   **TXT record**: Allows for arbitrary text to be associated with a domain. This is often used for verifying your domain ownership at websites like Good webmaster
    

And many more...

### DNS Tip

Don't use anything apart from Cloudflare for DNS the UI feels like the 1990s for the other tools, CloudFlare is very friendly and has lots of great things that come with DNS:

%[https://cloudflare.com] 

Concluding this article, DNS is complicated, but if you know what you are doing, then it's definitely helpful, so now that you know how DNS works and what common DNS records mean, it's time, to deploy your freaking SIDE PROJECT!!!