---
layout: post
title: "How to set your custom domain (and SSL certificate) in Github Pages"
description: "In this quick guide, I'll show you how to setup your custom domain in GH Pages, configure the DNS records, and establish the https protocol
for a safer aspect to our website."
---


In this quick guide, I'll show you how to setup your custom domain in GH Pages, configure the DNS records, and establish the https protocol
for a safer aspect of our website.

![introductory image](https://i.imgur.com/hpnvVdT.png)


## Table of content

1. [Introduction](#introduction)

2. [Buying the domain](#buyingdomain)

3. [Getting Github ready](#gettinggithubready)

4. [Configuring DNS records](#dnsrecords)

6. [Getting your Free SSL certificate](#sslcertificate)

7. [Conclusion](#conclusion)

<a name="introduction"></a>
## Introduction
Recently, I have found myself surfing the web trying to find out how to set up my new domain. I've been using [Github Pages](https://pages.github.com/) for a while now, and I considered buying a domain to professionalize my blog. For me, I chose [Hostinger](https://hostinger.es?REFERRALCODE=1ISMAEL06) because of its inexpensive price and its incredible upgrade potential. For example, you can obtain a professional email with your website name in it, for less than a monthly coffee. 

<a name="buyingdomain"></a>
## Buying the domain
First of all, we need our fresh domain. If you already have one, you can skip this step. As I said, before, I recommend [Hostinger](https://hostinger.es?REFERRALCODE=1ISMAEL06), but there are plenty of pages where you can get one almost for free. We'll need to check that our domain is available, and then we will proceed to buy it.

![hostinger buying page](https://i.imgur.com/znVjO2C.png)

As you can see, prices are quite attractive.

<a name="gettinggithubready"></a>
## Getting Github ready
First of all, we will need to access the GH Pahes configuration file of our repo.

![Github pages config inside repository](https://i.imgur.com/LbzKkfJ.png)

Mine is already set up (otherwise, you wouldn't be able to see this). We will fill the custom domain box with... our custom domain. One could think that, if it was this easy, anyone could copy each other's domains. That's why DNS records exist. These are a series of instructions that tell our server how to manage petitions to our website, and we must configure them to our domain to work. 

<a name="dnsrecords"></a>
## Configuring DNS records
With this objective, we have to sign in to Hostinger (or your selected provider), and go to manage domain:

![Manage domain in hostinger](https://i.imgur.com/8DrzJJD.png)

Now, we have to click in DNS / Nameservers (Or its equivalent)

![DNS domain config](https://i.imgur.com/hf9oRBK.png)

Now we have to add a DNS record per Github Pages IP. We can do this by selecting type "A", name "@" and pointing to each of these IPs (you have to add 4 DNS records):

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Once you have added all of them, we may have to wait a while to see our domain functioning, but in most cases, Hostinger does his job quickly. If we want, we can check in our command line if it is alright, using the next command:
```
dig yourweb +nostats +nocomments +nocmd 
```
replacing "yourweb" with your website.

If the output look like this (if you want it to look this good, check my [tutorial](https://ismaelcon.com/zsh-config)), it will be ready to go!
![Output of DNS checking](https://i.imgur.com/3QDf4BU.png)

<a name="sslcertificate"></a>
## Getting your Free SSL certificate
Last, but not least, we have to check a few more todos to our website to look safe, for both search engines and our visitors. The standard of security these days is SSL, but Github offers us a free [TLS Certificate](https://en.wikipedia.org/wiki/Transport_Layer_Security), an improved version of SSL. Sounds good, right?

We have to add a new DNS record, so access the same page as before. Choose: type "CNAME", name "www" and points to "yourgithubuser.github.io", changing "yourgithubuser" for, forgive the redundancy, your GitHub user. Click add, and the last thing you have to do is go to your repo Pages configuration and check the "Enforce HTTPS" checkbox. Now wait a few minutes (it shouldn't take long), and your certificate will come into effect. 

![checking enforce https checkbox](https://i.imgur.com/D2wEtXT.png)

<a name="conclusion"></a>
## Conclusion
I hope that you found this article helpful. I had to scroll through many docs to write it, and I wanted to save the effort for you. I will be delighted to read your comments if you have any questions. If you want to support me, please share with anyone who may find this of help. It means a lot!


