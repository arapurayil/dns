---
layout: default
title: FAQ
nav_order: 3
description: "Frequently Asked Questions"
permalink: /faq/
---
# Frequently Asked Questions
{: .no_toc .text-delta }

1. TOC
{:toc}

## What is DNS?

Simply put, the Domain Name Service (DNS) is like the phone directory of the Internet.

Every device connected to a network has an IP address, the equivalent of phone numbers. 

The IP address of this site is 157.245.130.6. This is considerably harder to remember than its _domain name_ which is dns.arapurayil.com.

IP addresses can also change after a time, just like a person changes his phone number.

So, we need a DNS resolver to keep track of the correct domain name with the IP address.

## What is an encrypted DNS resolver?

The queries you make on your device are sent to the DNS resolver to get the right IP address. More likely than not, these queries and responses are sent in plain text.

Which means anyone between your device and the resolver is able to eavesdrop or even modify your DNS queries and responses. 

This includes anyone in your local Wi-Fi network, your Internet Service Provider (ISP), and transit providers. 

Those queries can reveal not only what websites an individual visits but also meta data about other services such as the domains of email contacts, chat services, social-media ,etc.

An encrypted DNS can improve your internet privacy and security.

The popular DNS encryption protocols are:
- DNS-over-HTTPS
- DNS-over-TLS
- DNScrypt v2

## Why you should _probably_ change your current DNS resolver

Your default DNS resolver is likely the one set by your ISP or your network administrator and  it is unlikely to support ort encrypted DNS.

Even if they do, DNS encryption doesn't prevent ISPs from logging your DNS queries, and share this information with third-parties, if you're using a resolver they control.

Encryption also does not protect you against the resolver returning the wrong answer (through DNS hijacking or DNS cache poisoning attacks). 

The resolver will need to support DNSSEC to allow clients to verify the integrity of the returned DNS answer and catch any unauthorized tampering.

A resolver using encryption protocols may still need to send unencrypted queries to authoritative name servers, and unless the EDNS Client Subnet (ECS) is disabled and use QNAME minimisation, these queries could reveal the original client address that started the DNS query.

## What kind of DNS resolver should I use?

The DNS resolver that you need for better privacy ans security should atleast have the following attributes :-
- [x] Should not keep logs of personally identifiable information
- [x] Should support DNS encryption protocols like:
    - DNS-over-HTTPS
    - DNS-over-TLS
    - DNScrypt v2
- [x] Validate DNSSEC
- [x] Use QNAME minimisation

There are also resolvers that also blocks domains serving ads, trackers and malicious content.
You should also keep that in mind while choosing a DNS resolver.

## Where can I find a list of such resolvers?

DNS Privacy Project maintains two lists:-
- [Public resolvers maintained by large organisations](https://dnsprivacy.org/wiki/display/DP/DNS+Privacy+Public+Resolvers)
- [Public resolvers maintained by small organisations/individuals](https://dnsprivacy.org/wiki/display/DP/DNS+Privacy+Test+Servers) 

[List of DNSCrypt public resolvers](https://dnscrypt.info/public-servers) maintained by DNSCrypt Project

## How to use an encrypted DNS resolver?

A few systems support encrypted DNS protocols natively but for most systems native implementation of encrypted DNS protocols in other platforms are a work in progress.
- Microsoft has announced in November 2019 that native DNS-over-HTTPS will be supported on Windows 10.
- Apple has a provision for an on-device DNS proxy but support is limited to supervised iOS devices.

<dl style="overflow: auto;">
  <dt>DNS-over-HTTPS</dt>
  <dd>Android: <a href="https://play.google.com/store/apps/details?id=com.frostnerd.smokescreen">Nebulo</a>
  <br>Windows: <a href="https://simplednscrypt.org/">Simple DNSCrypt</a></dd>
  <dt>DNS-over-TLS</dt>
  <dd>Android 9 or later: <a href="https://support.google.com/android/answer/9089903#private_dns">Native implementation</a>; if not <a href="https://play.google.com/store/apps/details?id=com.frostnerd.smokescreen">Nebulo</a>
  <br>Linux: <a href="https://github.com/getdnsapi/stubby">Stubby</a></dd>
  <dt>DNSCrypt v2</dt>
  <dd>iOS: <a href="https://apps.apple.com/us/app/dnscloak-secure-dns-client/id1452162351">DNSCloak</a>
  <br>Windows: <a href="https://simplednscrypt.org/">Simple DNSCrypt</a></dd>
</dl>

Some browsers also offer support, but bear in mind that they offer encryption to only those queries you make inside the browser. 
- [Firefox](https://support.mozilla.org/en-US/kb/firefox-dns-over-https#w_manually-enabling-and-disabling-dns-over-https)
- [Bromite](https://www.bromite.org/doh)

Here is the [list of supported clients](https://dnsprivacy.org/wiki/display/DP/DNS+Privacy+Clients) maintained by DNS Privacy Project
