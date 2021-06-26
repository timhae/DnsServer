<p align="center">
	<a href="https://technitium.com/dns/">
		<img src="https://technitium.com/img/logo.png" alt="Technitium DNS Server" /><br />
		<b>Technitium DNS Server</b>
	</a><br />
	<br />
	<b>Get a personal local DNS Server for privacy & security.</b><br />
	<b>Block Ads at DNS level!</b>
</p>
<p align="center">
<img src="https://technitium.com/dns/ScreenShot1.png" alt="Technitium DNS Server" />
</p>

Technitium DNS Server is an open source tool that can be used for self hosting a local DNS server for privacy & security or, used for experimentation/testing by software developers on their computer. It works out-of-the-box with no or minimal configuration and provides a user friendly web console accessible using any web browser.

Nobody really bothers about domain name resolution since it works automatically behind the scenes and is complex to understand. Most computer software use the operating system's DNS resolver that usually query the configured ISP's DNS server using UDP protocol. This way works well for most people but, your ISP can see and control what website you can visit even when the website employ HTTPS security. Not only that, some ISPs can redirect, block or inject content into websites you visit even when you use a different DNS provider like Google DNS or Cloudflare DNS. Having Technitium DNS Server configured to use DNS-over-TLS or DNS-over-HTTPS forwarders, these privacy & security issues can be mitigated very effectively.

Developers regularly use the hosts file for configuring an IP address for a domain under testing. However, using the hosts file is cumbersome at times and can only be used to resolve domain name to an IP address. With a fully configurable DNS server running on your local machine, you can configure not just simple A records (for IP address) but, also configure other types of records like CNAME or MX etc. This allow you to have more control and power when you want to do testing that simulates the exact configuration that you have running on production.

Applications of using a locally hosted DNS server is limited only by the user's imagination!

# Features
- Works on Windows, Linux, macOS and Raspberry Pi.
- Installs in just a minute and works out-of-the-box with zero configuration.
- Block Ads using one or more block list URLs.
- Run [DNS-over-TLS](https://en.wikipedia.org/wiki/DNS_over_TLS) and [DNS-over-HTTPS](https://en.wikipedia.org/wiki/DNS_over_HTTPS) DNS service on your network.
- Use public DNS resolvers like Cloudflare, Google & Quad9 with [DNS-over-TLS](https://en.wikipedia.org/wiki/DNS_over_TLS) and [DNS-over-HTTPS](https://en.wikipedia.org/wiki/DNS_over_HTTPS) protocols as forwarders.
- Advance caching with features like serve stale, prefetching and auto prefetching.
- Supports working as an authoritative as well as a recursive DNS server.
- CNAME cloaking feature to block domain names that resolve to CNAME which are blocked.
- QNAME minimization support in recursive resolver [draft-ietf-dnsop-rfc7816bis-04](https://tools.ietf.org/html/draft-ietf-dnsop-rfc7816bis-04).
- QNAME randomization support for UDP transport protocol [draft-vixie-dnsext-dns0x20-00](https://tools.ietf.org/html/draft-vixie-dnsext-dns0x20-00).
- ANAME propriety record support to allow using CNAME like feature at zone root.
- APP propriety record support that allows custom DNS Apps to directly handle DNS requests and return a custom DNS response based on any business logic.
- Support for features like Split Horizon and Geolocation based responses using DNS Apps feature.
- Primary, Secondary, Stub, and Conditional Forwarder zone support.
- Host domain names on your own DNS server.
- Wildcard sub domain support.
- Enable/disable zones and records to allow testing with ease.
- Built-in DNS Client with option to import responses to local zone.
- Supports out-of-order DNS request processing for DNS-over-TCP and DNS-over-TLS protocols.
- Built-in DHCP Server that can work for multiple networks.
- IPv6 support in DNS server core.
- HTTP & SOCKS5 proxy support which can be configured to route DNS over [Tor Network](https://www.torproject.org/) or use Cloudflare's hidden DNS resolver.
- Web console portal for easy configuration using any web browser.
- Built in HTTP API to allow 3rd party apps to control and configure the DNS server.
- Built-in system logging and query logging.
- Open source cross-platform .NET 5 implementation hosted on GitHub.

# Planned Features
- Query logging support for databases feature as a DNS App.
- Multi-user role based access.
- API key to provide long term access token.
- Clustering support to manage two or more DNS servers.
- TSIG support.
- Dynamic DNS updates.
- EDNS support.
- DNSSEC support.

# Installation
- **Windows**: [Download setup installer](https://download.technitium.com/dns/DnsServerSetup.zip) for easy installation.
- **Linux & Raspberry Pi**: Follow install instructions from [this blog post](https://blog.technitium.com/2017/11/running-dns-server-on-ubuntu-linux.html).
- **Cross-Platform**: [Download portable app](https://download.technitium.com/dns/DnsServerPortable.tar.gz) to run on any platform that has .NET 5 installed.
- **Docker**: Pull the official image from [Docker Hub](https://hub.docker.com/r/technitium/dns-server). Use the [docker-compose.yml](https://github.com/TechnitiumSoftware/DnsServer/blob/develop/docker-compose.yml) example to create a new container and edit it as required for your deployments.

# API Documentation
The DNS server HTTP API allows any 3rd party app or script to configure the DNS server. The HTTP API is used by the web console and thus all the actions that the web console does can be performed via the API. Read the [HTTP API documentation](https://github.com/TechnitiumSoftware/DnsServer/blob/master/APIDOCS.md) for complete details.

# Help Topics
Read the latest [online help topics](https://go.technitium.com/?id=25) which contains the DNS Server user manual and covers frequently asked questions.

# Support
For support, send an email to support@technitium.com. For any issues, feedback, or feature request, create an issue on [GitHub](https://github.com/TechnitiumSoftware/DnsServer/issues).

Join [/r/technitium](https://www.reddit.com/r/technitium/) on Reddit.

# Donate
Make contribution to Technitium by becoming a Patron and help making new software, updates, and features possible.

[Become a Patron now!](https://www.patreon.com/technitium)

# Blog Posts
- [Yolan Romailler: Being ad-free on Android without rooting](https://romailler.ch/2021/04/15/misc-pihole_over_dot/) (Apr 2021)
- [Technitium Blog: Creating And Running DNS Apps On Technitium DNS Server](https://blog.technitium.com/2021/03/creating-and-running-dns-apps-on.html) (Mar 2021)
- [Technitium Blog: How To Host Your Own DNS-over-HTTPS And DNS-over-TLS Services](https://blog.technitium.com/2020/07/how-to-host-your-own-dns-over-https-and.html) (Oct 2020)
- [Technitium Blog: How To Disable Firefox DNS-over-HTTPS On Your Network](https://blog.technitium.com/2020/07/how-to-disable-firefox-dns-over-https.html) (Jul 2020)
- [Technitium Blog: How To Enforce Google Safe Search And YouTube Restricted Mode On Your Network](https://blog.technitium.com/2020/07/how-to-enforce-google-safe-search-and.html) (Jul 2020)
- [Technitium Blog: Technitium DNS Server v5 Released!](https://blog.technitium.com/2020/07/technitium-dns-server-v5-released.html) (Jul 2020)
- [Brian Wojtczak: Keep It Encrypted, Keep It Safe: Working with ESNI, DoH, and DoT](https://www.toptal.com/web/encrypted-safe-with-esni-doh-dot) (Jan 2020)
- [phra's blog: Exfiltrate Like a Pro: Using DNS over HTTPS as a C2 Channel](https://iwantmore.pizza/posts/dnscat2-over-doh.html) (Aug 2019)
- [Scott Hanselman: Exploring DNS with the .NET Core based Technitium DNS Server](https://www.hanselman.com/blog/ExploringDNSWithTheNETCoreBasedTechnitiumDNSServer.aspx) (Apr 2019)
- [Technitium Blog: Turn Raspberry Pi Into Network Wide DNS Server](https://blog.technitium.com/2019/01/turn-raspberry-pi-into-network-wide-dns.html) (Jan 2019)
- [Technitium Blog: Blocking Internet Ads Using DNS Sinkhole](https://blog.technitium.com/2018/10/blocking-internet-ads-using-dns-sinkhole.html) (Oct 2018)
- [Technitium Blog: Configuring DNS Server For Privacy & Security](https://blog.technitium.com/2018/06/configuring-dns-server-for-privacy.html) (Jun 2018)
- [Technitium Blog: Technitium DNS Server v1.3 Released!](https://blog.technitium.com/2018/06/technitium-dns-server-v13-released.html) (Jun 2018)
- [Technitium Blog: Running Technitium DNS Server on Ubuntu Linux](https://blog.technitium.com/2017/11/running-dns-server-on-ubuntu-linux.html) (Nov 2017)
- [Technitium Blog: Technitium DNS Server Released!](https://blog.technitium.com/2017/11/technitium-dns-server-released.html) (Nov 2017)
