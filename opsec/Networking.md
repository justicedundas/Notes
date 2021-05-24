# Networking

## IP Address:

### Public IP Tools

#### Find IP:
* https://resolve.rs/ * https://www.dnsleaktest.com/

#### Find IP Location:
* https://resolve.rs/ip/geolocation.html

#### Find if an IP is "suspicious"
* https://www.virustotal.com/gui/home/search * https://iknowwhatyoudownload.com/

#### Registration info of IP
* https://whois.domaintools.com/

#### Check for open-services/open-devices on IP
* https://www.shodan.io/host/<ip-address>

#### IP blacklist checkers, etc.
* https://www.whatismyip.com * https://browserleaks.com/

#### Check Tor Connection
* https://check.torproject.org

#### Obfuscating/Hide Origin IP methods
* Use public Wi-Fi service * Use Tor Anonymity Network * Use VPN service anonymously (pay cash or monero)

### DNS Requests
How it works: * https://www.youtube.com/watch?v=vrxwXXytEuI

#### Encrypting DNS Requests

*Protocols*

- DoH (DNS over HTTPS) - DoT (DNS over TLS)

*Methods*

- locally hosted -> pi-hole - remotely hosted -> nextdns.io, VPN provider, Tor network

*Issues* 
- TLS protocol used in most browsers causes DNS leaks through SNI (Server Name Indicator) - Firefox is only browser that supports ECH (Encrypted Client 
Hello, or eSNI) 
- only Web Services and CDNs (Client Delivery Networks) behind Cloudflare CDN support ECH/eSNI rn

### The 10 Immutable Laws

Law #1: If a bad guy can persuade you to run his program on your computer, it's not solely your computer anymore.
Law #2: If a bad guy can alter the operating system on your computer, it's not your computer anymore.
Law #3: If a bad guy has unrestricted physical access to your computer, it's not your computer anymore.
Law #4: If you allow a bad guy to run active content in your website, it's not your website any more.
Law #5: Weak passwords trump strong security.
Law #6: A computer is only as secure as the administrator is trustworthy.
Law #7: Encrypted data is only as secure as its decryption key.
Law #8: An out-of-date antimalware scanner is only marginally better than no scanner at all.
Law #9: Absolute anonymity isn't practically achievable, online or offline.
Law #10: Technology is not a panacea.

### 5 P's of Post-Exploitation:

Persistence = Find a way to maintain access
Privilege Escalation = Find a way to get a higher level of access than you already have
Pilfer = Steal things
Pillage = Break things.
Pivot = Move from one box to another and start the killchain all over again.

### Useful Resurces for Security Research:

* https://www.fireeye.com/current-threats/annual-threat-report/mtrends.html
* https://www.sans.org/security-resources/?msc=main-nav

### APT's
* https://www.secureworks.com/blog/advanced-persistent-threats-apt-a
* https://www.fireeye.com/content/dam/fireeye-www/services/pdfs/mandiant-apt1-report.pdf

### OWASP Cheat Sheet
* https://cheatsheetseries.owasp.org/index.html

### Architecture
* Modem
* Router
* Switch
* Firewall
* DMZ
* Proxy
* Endpoint/Host
* Server
* Web Application
* Domain Controller




### Tools

* Ungoogled Chromium:
  * https://github.com/Eloston/ungoogled-chromium



