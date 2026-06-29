# Awesome OSINT [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Stars](https://img.shields.io/github/actions/workflow/status/edwardtay/awesome-OSINT/update-stars.yml?label=star%20updates)](https://github.com/edwardtay/awesome-OSINT/actions/workflows/update-stars.yml)
[![Links](https://img.shields.io/github/actions/workflow/status/edwardtay/awesome-OSINT/links.yml?label=links)](https://github.com/edwardtay/awesome-OSINT/actions/workflows/links.yml)
[![Last Commit](https://img.shields.io/github/last-commit/edwardtay/awesome-OSINT)](https://github.com/edwardtay/awesome-OSINT/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/edwardtay/awesome-OSINT/pulls)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](LICENSE)

> A curated list of open-source intelligence (OSINT) tools — people search, domains, social media, geolocation, breach data, and investigation frameworks.

> ⚠️ = known maintenance concern; verify repository status before adoption.

## How to Choose

| I need to... | Start here |
|---|---|
| Find someone by username | [Username & People Search](#️-username--people-search) |
| Tie an email to leaked accounts | [Email & Breach Data](#-email--breach-data) |
| Map a domain's attack surface | [Domain, DNS & Infrastructure](#-domain-dns--infrastructure) |
| Search the whole internet for exposed hosts | [Internet Scan Engines & Attack Surface](#-internet-scan-engines--attack-surface) |
| Geolocate a photo | [Geolocation & GEOINT](#️-geolocation--geoint) |
| Reverse-search an image or face | [Image & Reverse Image Search](#️-image--reverse-image-search) |
| Check breach exposure | [Email & Breach Data](#-email--breach-data) |
| Investigate a phone number | [Phone & Identity](#-phone--identity) |
| Trace a wallet | [Crypto / Blockchain OSINT](#️-crypto--blockchain-osint) |
| Track a flight/ship | [Transport Tracking](#️-transport-tracking) |
| Triage a malicious file/URL/IP | [Threat Intel & Malware OSINT](#-threat-intel--malware-osint) |
| Run one platform that does it all | [Frameworks & All-in-One](#-frameworks--all-in-one) |

---

## Contents

- [🧰 Frameworks & All-in-One](#-frameworks--all-in-one)
- [🕵️ Username & People Search](#-username--people-search)
- [📧 Email & Breach Data](#-email--breach-data)
- [🌐 Domain, DNS & Infrastructure](#-domain-dns--infrastructure)
- [📡 Internet Scan Engines & Attack Surface](#-internet-scan-engines--attack-surface)
- [☁️ Cloud, IoT & Web Recon](#-cloud-iot--web-recon)
- [💬 Social Media Intelligence (SOCMINT)](#-social-media-intelligence-socmint)
- [📨 Messaging-App OSINT](#-messaging-app-osint)
- [🖼️ Image & Reverse Image Search](#-image--reverse-image-search)
- [🔬 Image, Video & Media Forensics](#-image-video--media-forensics)
- [🗺️ Geolocation & GEOINT](#-geolocation--geoint)
- [📱 Phone & Identity](#-phone--identity)
- [🔎 Google Dorking & Search Operators](#-google-dorking--search-operators)
- [✈️ Transport, RF & SIGINT](#-transport-rf--sigint)
- [⛓️ Crypto / Blockchain OSINT](#-crypto--blockchain-osint)
- [🦠 Threat Intel & Malware OSINT](#-threat-intel--malware-osint)
- [🧅 Dark Web & Paste Sites](#-dark-web--paste-sites)
- [🏛️ Business, Records & Archives](#-business-records--archives)
- [🧩 Browser Extensions & Bookmarklets](#-browser-extensions--bookmarklets)
- [📚 Datasets, Lists & APIs](#-datasets-lists--apis)
- [🪦 Deprecated Tools Graveyard](#-deprecated-tools-graveyard)


## 🧰 Frameworks & All-in-One

Heavyweight platforms that orchestrate dozens of OSINT modules, transforms and link-analysis into one investigation surface.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Maltego](https://www.maltego.com/) | — | — | Visual link-analysis platform mapping relationships between people, domains, infrastructure and social accounts via transforms. |
| [SpiderFoot](https://github.com/smicallef/spiderfoot) | 14k | Python | Automated OSINT engine with 200+ modules correlating data on IPs, domains, emails, names and more. |
| [Recon-ng](https://github.com/lanmaster53/recon-ng) | 3.8k | Python | Full-featured modular web reconnaissance framework with a Metasploit-style interface. |
| [OSINT Framework](https://osintframework.com/) | 9k | JavaScript | Web directory tree linking OSINT resources by data type — the canonical jumping-off map for investigators. |
| [IntelTechniques Tools](https://inteltechniques.com/tools/) | — | — | Michael Bazzell's curated online search tools and workflows for people, email, username and domain investigations. |
| [Mr.Holmes](https://github.com/Lucksi/Mr.Holmes) | 1.6k | Python | All-in-one information-gathering framework for usernames, phone numbers and domains. |
| [OSINT-SPY](https://github.com/SharadKumar97/OSINT-SPY) | 0.6k | Python | Performs OSINT on emails, domains, IPs, devices and Bitcoin addresses from a single CLI. |
| [Datasploit](https://github.com/DataSploit/datasploit) | 3k | Python | Archived but influential OSINT framework that aggregated intel on domains, emails, usernames and phones. ⚠️ |
| [Mitaka](https://github.com/ninoseki/mitaka) | 1.6k | TypeScript | Browser extension that extracts and pivots IOCs (IPs, hashes, domains) to 70+ search engines via right-click. |
| [Hunchly](https://www.hunch.ly/) | — | — | Commercial web-capture tool that automatically logs, hashes and indexes every page visited during an investigation. |
| [Osmedeus](https://github.com/j3ssie/osmedeus) | 5k | Go | Workflow engine for automated reconnaissance and attack-surface mapping. |
| [FinalRecon](https://github.com/thewhiteh4t/FinalRecon) | 2.6k | Python | All-in-one web recon tool (whois, DNS, headers, crawl, Wayback, subdomains). |
| [sn0int](https://github.com/kpcyrd/sn0int) | 2k | Rust | Semi-automatic OSINT framework and package manager for entity-graph recon. |
| [OWASP Maryam](https://github.com/saeeddhqan/maryam) | 1.1k | Python | Modular open-source framework for web-based OSINT and data mining. |
| [maltego-trx](https://github.com/MaltegoTech/maltego-trx) | 300 | Python | Official library for writing custom Maltego transforms and TDS servers. |
| [gOSINT](https://github.com/Nhoya/gOSINT) | 1.1k | Go | Modular CLI OSINT framework for emails, PGP, Telegram and more. ⚠️ |
| [Tsurugi Linux](https://tsurugi-linux.org/) | — | Distro | DFIR/OSINT-focused Linux distribution with a dedicated OSINT tool set. |
| [CSI Linux](https://csilinux.com/) | — | Distro | Investigation-focused Linux platform bundling OSINT, DFIR and dark-web tooling. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🕵️ Username & People Search

Pivot a username, real name or handle into a person's accounts and public-records footprint across the web.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Sherlock](https://github.com/sherlock-project/sherlock) | 62k | Python | Hunts a username across hundreds of social networks and websites to find a person's accounts. |
| [Maigret](https://github.com/soxoj/maigret) | 15k | Python | Builds a dossier on a person by username from 3000+ sites, extracting profile details and relations. |
| [GHunt](https://github.com/mxrch/GHunt) | 16k | Python | Investigates Google accounts and objects — emails, profiles, reviews, photos — from a Gmail address or ID. |
| [blackbird](https://github.com/p1ngul1n0/blackbird) | 3.5k | Python | Fast OSINT username and email search across hundreds of sites with WhatsMyName metadata. |
| [socialscan](https://github.com/iojw/socialscan) | 3k | Python | Checks email and username availability/registration on online platforms with accurate signup-flow queries. |
| [WhatsMyName](https://whatsmyname.app/) | 2k | Python | Community-driven username enumeration project and web app with a large, validated site list. |
| [Creepy](https://github.com/ilektrojohn/creepy) | 1.3k | Python | Geolocation OSINT tool that gathers location data from a target's social-media posts and image metadata. |
| [FastPeopleSearch](https://www.fastpeoplesearch.com/) | — | — | Free US people-search returning addresses, phones, relatives and associates from public records by name. |
| [TruePeopleSearch](https://www.truepeoplesearch.com/) | — | — | Free US public-records lookup for current/past addresses, phone numbers and known relatives. |
| [IDCrawl](https://www.idcrawl.com/) | — | — | People-search aggregator that surfaces social profiles, usernames and public records by name or handle. |
| [Namechk](https://namechk.com/) | — | — | Instantly checks a username and domain across many social networks for availability/registration. |
| [Snoop](https://github.com/snooppr/snoop) | 4k | Python | Username search across 5400+ sites with its own web DB and IP/geo plugins. |
| [Nexfil](https://github.com/thewhiteh4t/nexfil) | 2.6k | Python | Finds profiles by username across 350+ sites with low false positives. ⚠️ |
| [Tookie-osint](https://github.com/Alfredredbird/tookie-osint) | 2.5k | Python | Discovers social media accounts from a username, Sherlock-style. |
| [Octosuite](https://github.com/bellingcat/octosuite) | 1.9k | Python | Terminal toolkit for GitHub account/repo/org OSINT (Bellingcat). |
| [CrossLinked](https://github.com/m8sec/CrossLinked) | 1.6k | Python | Enumerates valid LinkedIn employee names via search-engine scraping. |
| [socid-extractor](https://github.com/soxoj/socid-extractor) | 1k | Python | Extracts account IDs/metadata from profile pages across 130+ sites. |
| [GitFive](https://github.com/mxrch/GitFive) | 1k | Python | Tracks down GitHub users; pivots email to account and dumps SSH keys. |
| [Profil3r](https://github.com/Greyjedix/Profil3r) | 660 | Python | Finds a person's accounts and emails, with data-leak alerting. |
| [Marple](https://github.com/soxoj/marple) | 310 | Python | Collects profile links by username through 10+ search engines. |
| [WebMii](https://webmii.com) | — | Web | People-search engine aggregating public web profiles by name with "PeopleRank". |
| [That'sThem](https://thatsthem.com) | — | Web | Free people search with reverse email/phone/address lookups. |
| [Spokeo](https://www.spokeo.com) | — | Web | People search aggregating 12B+ records by name, phone, email, or address. |
| [Predicta Search](https://www.predictasearch.com) | — | Web | Reverse email/phone/username/name lookup to 100+ social profiles. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 📧 Email & Breach Data

Tie an email to accounts, leaked credentials and breach corpora — registration enumeration to dump search.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Have I Been Pwned](https://haveibeenpwned.com/) | — | — | Checks whether an email or phone appears in known data breaches; offers a domain-monitoring API. |
| [Holehe](https://github.com/megadose/holehe) | 8k | Python | Checks whether an email is registered on dozens of sites using password-reset and signup flows. |
| [h8mail](https://github.com/khast3x/h8mail) | 4k | Python | Email OSINT and breach-hunting tool that pulls passwords from local dumps and online services. |
| [Mosint](https://github.com/alpkeskin/mosint) | 3k | Go | Fast automated email OSINT tool aggregating breach checks, related emails and social lookups. |
| [breach-parse](https://github.com/hmaverickadams/breach-parse) | 1.6k | Shell | Parsing tool for the COMB/large credential dumps to extract emails and passwords for a target domain. |
| [buster](https://github.com/sham00n/buster) | 1k | Python | Advanced email OSINT tool that finds linked accounts, breaches and social profiles for an address. |
| [Dehashed](https://www.dehashed.com/) | — | — | Searchable breach-data engine to query emails, usernames, passwords, names and IPs across leaks. |
| [Snusbase](https://snusbase.com/) | — | — | Commercial breach-database search across billions of leaked records by email, hash, IP or name. |
| [LeakCheck](https://leakcheck.io/) | — | — | Data-breach search engine and API for checking emails, usernames and keywords against leak corpora. |
| [EmailRep](https://emailrep.io/) | — | — | Email reputation service returning risk signals, linked profiles and breach appearance for an address. |
| [Hunter.io](https://hunter.io/) | — | — | Finds and verifies professional email addresses for a domain and reveals common address patterns. |
| [check-if-email-exists](https://github.com/reacherhq/check-if-email-exists) | 9k | Rust | Verifies whether an email address exists without sending mail (SMTP probe). |
| [WhatBreach](https://github.com/Ekultek/WhatBreach) | 1.6k | Python | Finds breaches, databases and pastes tied to an email address. |
| [EmailHarvester](https://github.com/maldevel/EmailHarvester) | 960 | Python | Retrieves a domain's email addresses from multiple search engines. |
| [MailFinder](https://github.com/mishakorzik/MailFinder) | 570 | Python | OSINT tool to find an email address from a first and last name. |
| [EmailFinder](https://github.com/Josue87/EmailFinder) | 420 | Python | Searches a domain's emails through search engines. ⚠️ |
| [XposedOrNot](https://xposedornot.com) | — | Web | Free data-breach search engine and open API for emails and domains. |
| [BreachDirectory](https://breachdirectory.org) | — | Web | Searches public breaches by email/username; free tier plus API. |
| [Hudson Rock Cavalier](https://cavalier.hudsonrock.com) | — | Web | Free infostealer-infection lookup for emails, domains and usernames. |
| [LeakPeek](https://leakpeek.com/) | — | Web | Hosted breach search over 8.2B+ records by email, username, password, domain or name. |
| [Leak-Lookup](https://leak-lookup.com/) | — | Web | Breach search across thousands of dumps; email/username/IP/phone/domain fields. |
| [LeakRadar](https://leakradar.io/en) | — | Web | Stealer-log/combolist engine indexing 507B+ credentials; free search, paid reveal. |
| [Whiteintel](https://whiteintel.io/) | — | Web | Dark-web/infostealer credential monitoring with free domain-compromise search. |
| [ransomware.live](https://www.ransomware.live/) | 334 | Python | Ransomware gang tracker scraping data-leak sites; API and live victim map. |
| [RansomLook](https://www.ransomlook.io/) | 629 | Python | Open-source aggregator tracking 580+ ransomware groups and their leak-site posts. |
| [DDoSecrets](https://ddosecrets.org/) | — | Web | Nonprofit archive publishing/searching 100M+ hacked and leaked documents. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🌐 Domain, DNS & Infrastructure

Footprint a target's domains, subdomains, DNS, certificates and tech stack from passive public sources.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [OWASP Amass](https://github.com/owasp-amass/amass) | 13k | Go | In-depth attack-surface mapping and external asset discovery via passive and active DNS reconnaissance. |
| [theHarvester](https://github.com/laramies/theHarvester) | 12k | Python | Gathers emails, names, subdomains, IPs and URLs for a domain from search engines and certificate logs. |
| [subfinder](https://github.com/projectdiscovery/subfinder) | 11k | Go | Fast passive subdomain enumeration tool that pulls from many online sources via their APIs. |
| [Sublist3r](https://github.com/aboul3la/Sublist3r) | 9k | Python | Classic subdomain enumeration tool using search engines, VirusTotal, Netcraft and DNSdumpster. |
| [dnstwist](https://github.com/elceef/dnstwist) | 5k | Python | Domain-permutation engine that detects typosquats, phishing and brand-impersonation domains. |
| [knockpy](https://github.com/guelfoweb/knock) | 4.5k | Python | Subdomain scanner that enumerates hostnames via wordlists and resolves them with reporting. |
| [assetfinder](https://github.com/tomnomnom/assetfinder) | 3.2k | Go | Quickly finds domains and subdomains related to a target from multiple passive sources. |
| [crt.sh](https://crt.sh/) | — | — | Certificate Transparency log search that surfaces subdomains via every TLS certificate issued for a domain. |
| [DNSDumpster](https://dnsdumpster.com/) | — | — | Free domain research tool mapping a domain's hosts, DNS records and network as a visual diagram. |
| [SecurityTrails](https://securitytrails.com/) | — | — | Historical DNS, WHOIS and domain/IP intelligence platform with deep records and an API. |
| [WHOIS / RDAP](https://www.whois.com/whois/) | — | — | Look up registration details, registrar, dates and contacts for domains and IP allocations. |
| [ViewDNS.info](https://viewdns.info/) | — | — | Free toolbox of DNS, WHOIS, reverse-IP, IP-history and port-check utilities in one place. |
| [BuiltWith](https://builtwith.com/) | — | — | Profiles the technology stack behind a website — CMS, analytics, frameworks, hosting and more. |
| [Wappalyzer](https://www.wappalyzer.com/) | — | — | Technology profiler identifying the CMS, frameworks, analytics and servers a website is built with. |
| [Netlas.io](https://netlas.io/) | — | — | Internet-wide scan and attack-surface search engine for hosts, domains, certificates and responses. |
| [dnsx](https://github.com/projectdiscovery/dnsx) | 2.6k | Go | Fast multi-purpose DNS toolkit for bulk A/AAAA/CNAME/PTR queries and brute-force. |
| [shuffledns](https://github.com/projectdiscovery/shuffledns) | 1.6k | Go | massdns wrapper for active subdomain brute-force and resolution with wildcard filtering. |
| [massdns](https://github.com/blechschmidt/massdns) | 4.1k | C | High-performance stub DNS resolver for bulk lookups (millions of names/sec). |
| [puredns](https://github.com/d3mondev/puredns) | 2.1k | Go | Fast domain resolver and subdomain bruteforcer that filters wildcards and poisoned entries. |
| [Findomain](https://github.com/Findomain/Findomain) | 3.8k | Rust | Cross-platform subdomain enumerator pulling from cert transparency and dozens of sources. |
| [chaos-client](https://github.com/projectdiscovery/chaos-client) | 1k | Go | Client for ProjectDiscovery's Chaos dataset of internet-wide DNS/subdomain data. |
| [asnmap](https://github.com/projectdiscovery/asnmap) | 1k | Go | Maps an organization's network ranges/CIDRs from ASN, org name, IP, or domain. |
| [mapcidr](https://github.com/projectdiscovery/mapcidr) | 1.2k | Go | CIDR/IP range utility for slicing, expanding, and aggregating network ranges. |
| [cero](https://github.com/glebarez/cero) | 700 | Go | Scrapes domain names directly from TLS certificates of live hosts at scale. |
| [CTFR](https://github.com/UnaPibaGeek/ctfr) | 2k | Python | Enumerates HTTPS subdomains by abusing Certificate Transparency logs (no brute-force). |
| [hakrevdns](https://github.com/hakluke/hakrevdns) | 1.5k | Go | Small, fast tool for performing reverse DNS (PTR) lookups en masse. |
| [dnsgen](https://github.com/AlephNullSK/dnsgen) | 900 | Python | Generates intelligent subdomain name permutations from a seed wordlist. |
| [dnsrecon](https://github.com/darkoperator/dnsrecon) | 2.6k | Python | Versatile DNS recon: zone transfers, brute-force, SRV/PTR enumeration, cache snooping. |
| [Fierce](https://github.com/mschwager/fierce) | 2k | Python | DNS reconnaissance scanner for locating non-contiguous IP space and hostnames. |
| [Gobuster](https://github.com/OJ/gobuster) | 11k | Go | Brute-force tool with DNS subdomain, vhost, and directory/file enumeration modes. |
| [alterx](https://github.com/projectdiscovery/alterx) | 900 | Go | Pattern-based subdomain wordlist/permutation generator for active enumeration. |
| [Hurricane Electric BGP Toolkit](https://bgp.he.net) | — | Web | Web portal for ASN, BGP prefix, peering, and reverse-IP intelligence lookups. |
| [RapidDNS](https://rapiddns.io) | — | Web | Free DNS query service for reverse-IP, subdomain, and shared-host lookups. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 📡 Internet Scan Engines & Attack Surface

Search engines for the whole internet — query exposed hosts, devices, banners and certificates without scanning yourself.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Shodan](https://www.shodan.io/) | — | — | Search engine for internet-connected devices — exposed services, banners, ICS/IoT and vulnerabilities. |
| [Censys Search](https://search.censys.io/) | — | — | Continuously updated internet-wide scan dataset for hosts and certificates with rich filtering and an API. |
| [ZoomEye](https://www.zoomeye.org/) | — | — | Internet-wide search engine mapping exposed hosts, devices and services with banner/fingerprint data. |
| [FOFA](https://en.fofa.info/) | — | — | Cyberspace search engine indexing internet-exposed assets, services and fingerprints for recon. |
| [BinaryEdge](https://www.binaryedge.io/) | — | — | Internet-scanning data platform exposing open ports, services, leaked data and attack-surface signals. |
| [Onyphe](https://www.onyphe.io/) | — | — | Cyber-defense search engine correlating internet scan, threat and OSINT data for an IP or domain. |
| [GreyNoise](https://www.greynoise.io/) | — | — | Tells you whether an IP is mass-internet background noise or a targeted threat, cutting alert fatigue. |
| [nuclei](https://github.com/projectdiscovery/nuclei) | 22k | Go | Community-powered, YAML-template vulnerability and exposure scanner. |
| [masscan](https://github.com/robertdavidgraham/masscan) | 24k | C | Asynchronous TCP port scanner capable of scanning the entire internet in minutes. |
| [RustScan](https://github.com/RustScan/RustScan) | 15k | Rust | Modern port scanner that scans all 65k ports in seconds and pipes into Nmap. |
| [naabu](https://github.com/projectdiscovery/naabu) | 4.6k | Go | Fast SYN/CONNECT port scanner built for piping into attack-surface workflows. |
| [httpx](https://github.com/projectdiscovery/httpx) | 8.1k | Go | Fast multi-purpose HTTP probing toolkit for fingerprinting live web servers at scale. |
| [ZMap](https://github.com/zmap/zmap) | 5.4k | C | Fast single-packet network scanner designed for internet-wide research surveys. |
| [uncover](https://github.com/projectdiscovery/uncover) | 2.8k | Go | Queries Shodan, Censys, FOFA, Hunter and Quake from one CLI to find exposed hosts. |
| [Smap](https://github.com/s0md3v/Smap) | 1.7k | Go | Drop-in Nmap replacement returning port/CVE data passively via Shodan's free API. |
| [nrich](https://gitlab.com/shodan-public/nrich) | 1.4k | Rust | Enriches a list of IPs with open ports and known CVEs using Shodan's InternetDB. |
| [IVRE](https://github.com/ivre/ivre) | 3.7k | Python | Self-hosted network recon framework/database for building your own Shodan-like map. |
| [reconFTW](https://github.com/six2dez/reconftw) | 6.7k | Shell | Automated recon orchestrator chaining dozens of subdomain, scan, and vuln tools. |
| [Sn1per](https://github.com/1N3/Sn1per) | 8.7k | Shell | Automated pentest and attack-surface management platform with recon/scan modules. |
| [Criminal IP](https://www.criminalip.io) | — | Web | Search engine for exposed devices, open ports, and internet-facing asset intelligence. |
| [FullHunt](https://fullhunt.io) | — | Web | Attack-surface database/search engine to discover and monitor exposed assets. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>


## ☁️ Cloud, IoT & Web Recon

Find exposed buckets, cloud assets, internet-connected devices, and a site's technology and archived footprint.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [S3Scanner](https://github.com/sa7mon/S3Scanner) | 2.7k | Go | Scans for open/misconfigured buckets across S3-compatible APIs and dumps permissions. |
| [cloud_enum](https://github.com/initstring/cloud_enum) | 2.5k | Python | Multi-cloud OSINT tool enumerating public AWS, Azure, and GCP resources. |
| [CloudBrute](https://github.com/0xsha/CloudBrute) | 1.2k | Go | Finds a company's files/apps/infrastructure across the major cloud providers. |
| [cloudlist](https://github.com/projectdiscovery/cloudlist) | 1k | Go | Lists assets/hostnames from multiple cloud providers using their APIs. |
| [GCPBucketBrute](https://github.com/RhinoSecurityLabs/GCPBucketBrute) | 1k | Python | Enumerates Google Storage buckets and checks for privilege-escalation paths. |
| [GrayhatWarfare](https://buckets.grayhatwarfare.com) | — | Web | Searchable index of public S3/Azure/GCP buckets and exposed files. |
| [ScoutSuite](https://github.com/nccgroup/ScoutSuite) | 7k | Python | Multi-cloud security auditing tool that surfaces misconfigured/exposed assets. |
| [Kamerka](https://github.com/woj-ciech/Kamerka-GUI) | 1.2k | Python | Maps exposed IoT devices, webcams, and ICS on a map using Shodan/Censys/BinaryEdge. |
| [Insecam](http://www.insecam.org) | — | Web | Directory of internet-accessible, unsecured IP cameras worldwide. |
| [webanalyze](https://github.com/rverton/webanalyze) | 2.3k | Go | Go port of Wappalyzer for fast mass web technology fingerprinting. |
| [WhatWeb](https://github.com/urbanadventurer/WhatWeb) | 5.4k | Ruby | Web scanner identifying CMS, frameworks, analytics IDs, and 1800+ technology plugins. |
| [FavFreak](https://github.com/devanshbatham/FavFreak) | 1k | Python | Pivots on favicon.ico hashes to discover related assets/IPs via Shodan. ⚠️ |
| [waybackurls](https://github.com/tomnomnom/waybackurls) | 3.6k | Go | Fetches all URLs the Wayback Machine knows about for a domain. |
| [gau](https://github.com/lc/gau) | 3.8k | Go | Pulls known URLs from Wayback, Common Crawl, OTX, and URLScan for a target. |
| [waymore](https://github.com/xnl-h4ck3r/waymore) | 2k | Python | Deep archive recon across Wayback, Common Crawl, OTX, URLScan and VirusTotal. |
| [hakrawler](https://github.com/hakluke/hakrawler) | 4.8k | Go | Fast web crawler for discovering endpoints, assets, and URLs on a target. |
| [web-check](https://github.com/lissy93/web-check) | 25k | TypeScript | All-in-one website OSINT dashboard: DNS, headers, tech stack, certs, archives, and more. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>
## 💬 Social Media Intelligence (SOCMINT)

Scrape, archive and analyze posts, profiles and channels across the major social and messaging platforms.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Social-Analyzer](https://github.com/qeeqbox/social-analyzer) | 12k | Python | API/CLI/web tool to find and analyze a person's profiles across 1000+ social media sites. |
| [Osintgram](https://github.com/Datalux/Osintgram) | 10k | Python | Interactive Instagram OSINT tool to pull followers, emails, phones, tagged photos and locations. |
| [Instaloader](https://instaloader.github.io/) | 9k | Python | Downloads Instagram posts, stories, profile metadata and comments for archival and analysis. |
| [snscrape](https://github.com/JustAnotherArchivist/snscrape) | 4.6k | Python | Scrapes social networks (X/Twitter, Telegram, Reddit, etc.) without API keys for posts and profiles. |
| [toutatis](https://github.com/megadose/toutatis) | 2.2k | Python | Extracts obfuscated emails, phone numbers and account info from Instagram profiles. |
| [Telepathy](https://github.com/jordanwildon/Telepathy) | 1.1k | Python | Telegram OSINT toolkit for archiving channels and analysing members, messages and forwards. |
| [twint](https://github.com/twintproject/twint) | 16k | Python | Once-popular Twitter scraping tool needing no API — now deprecated/broken after X API changes. ⚠️ |
| [Telegago](https://cse.google.com/cse?cx=006249643689091525507) | — | — | Google custom search engine for discovering public Telegram channels, groups and messages. |
| [TGStat](https://tgstat.com/) | — | — | Telegram analytics and catalog for discovering channels and measuring reach and activity. |
| [YouTube DataViewer](https://citizenevidence.amnestyusa.org/) | — | — | Amnesty tool extracting a YouTube video's exact upload time and thumbnails for reverse search. |
| [twscrape](https://github.com/vladkens/twscrape) | 2.5k | Python | X/Twitter scraper with account-pool auth: search, profiles, followers, tweets, retweeters. |
| [Scweet](https://github.com/Altimis/Scweet) | 1.6k | Python | Scrapes tweets, profiles and followers from X without an API key, with proxy pooling. |
| [Xquik](https://github.com/Xquik-dev/x-twitter-scraper) | 126 | JavaScript | Commercial hosted X/Twitter OSINT API and MCP server for tweet search, user timelines, followers, monitors and webhooks. |
| [Ultimate Social Scrapers](https://github.com/harismuneer/Ultimate-Social-Scrapers) | 3k | Python | Scrapes Facebook/Instagram profile posts, photos and friend/follower lists without the API. |
| [linkedin2username](https://github.com/initstring/linkedin2username) | 1.8k | Python | Generates likely username/email permutations for all employees of a company from LinkedIn. |
| [Osintgraph](https://github.com/XD-MHLOO/Osintgraph) | 767 | Python | Maps an Instagram target's followers/followees into Neo4j to visualize their network. |
| [youtube-metadata](https://github.com/mattwright324/youtube-metadata) | 493 | JavaScript | Gathers metadata for a YouTube video/playlist/channel with thumbnail reverse-search. |
| [fb_friend_list_scraper](https://github.com/n0kovo/fb_friend_list_scraper) | 324 | Python | Scrapes names and usernames from large Facebook friend lists without hitting rate limits. |
| [SnapIntel](https://github.com/Kr0wZ/SnapIntel) | 314 | Python | Investigates Snapchat users: stories, spotlights, lenses, bitmojis and upload heatmaps. |
| [youtube-geofind](https://github.com/mattwright324/youtube-geofind) | 155 | JavaScript | Finds geotagged YouTube videos by channel, topic or location radius, with CSV export. |
| [tik-spyder](https://github.com/estebanpdl/tik-spyder) | 98 | Python | CLI that collects TikTok posts, videos and metadata via Google search for investigations. |
| [reddit-user-analyser](https://github.com/atomiks/reddit-user-analyser) | 200 | JavaScript | Analyzes a Reddit user's activity: top subreddits, posting times and word breakdowns. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>


## 📨 Messaging-App OSINT

Investigate Telegram, Discord, WhatsApp and fediverse accounts, channels and groups.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter) | 11k | C# | Exports any Discord channel, DM, group or server history to HTML/JSON/CSV for offline review. |
| [telegram-phone-number-checker](https://github.com/bellingcat/telegram-phone-number-checker) | 1.7k | Python | Checks whether phone numbers are tied to Telegram accounts, returning username and IDs (Bellingcat). |
| [Telerecon](https://github.com/sockysec/Telerecon) | 1.3k | Python | Reconnaissance framework to scrape Telegram channels/groups, map forwards and profile users. |
| [tgscan](https://github.com/tgscan-dev/tgscan) | 713 | Java | Search engine for discovering Telegram channels, groups and chat history by keyword. |
| [telegram-tracker](https://github.com/estebanpdl/telegram-tracker) | 382 | Python | Collects and analyzes messages/metadata from Telegram channels for disinformation research. |
| [Masto](https://github.com/C3n7ral051nt4g3ncy/Masto) | 265 | Python | Gathers intelligence on Mastodon users/instances and finds all accounts a user holds. |
| [WhatsApp-OSINT](https://github.com/kinghacker0/WhatsApp-OSINT) | 694 | Python | Pulls WhatsApp profile pic, About/status, business verification and linked-device data from a number. |
| [DiscordOSINT](https://github.com/husseinmuhaisen/DiscordOSINT) | 556 | — | Curated techniques for investigating Discord accounts, servers and bots (snowflake decoding, pivots). |
| [doxcord](https://github.com/boringthegod/doxcord) | 82 | Python | Scans Discord servers for shared tracker links that leak each sender's identity. |
| [tgcrawler](https://github.com/iggisv9t/tgcrawler) | 19 | Python | Crawls Telegram channels by following t.me links to map channel networks. |
| [blueskynet](https://github.com/jakecreps/blueskynet) | 15 | JavaScript | Web app to search, analyze and CSV-export results from the Bluesky API for OSINT. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>
## 🖼️ Image & Reverse Image Search

Find where a photo came from, who's in it, and whether it's been manipulated — reverse search, face search and forensics.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Google Lens / Images](https://images.google.com/) | — | — | Reverse image search to identify objects, places and the origin of a photo across the web. |
| [Yandex Images](https://yandex.com/images/) | — | — | Reverse image search engine widely regarded as strongest for faces and location matching. |
| [TinEye](https://tineye.com/) | — | — | Reverse image search specialising in finding exact copies, edits and the oldest occurrence of an image. |
| [Bing Visual Search](https://www.bing.com/visualsearch) | — | — | Microsoft's reverse image search, often complementary to Google and Yandex for Western web matches. |
| [PimEyes](https://pimeyes.com/) | — | — | Facial-recognition search engine that finds other photos of a face across the public web. |
| [FotoForensics](https://fotoforensics.com/) | — | — | Image-manipulation analysis using Error Level Analysis and metadata to spot edits and fakes. |
| [Forensically](https://29a.ch/photo-forensics/) | — | — | Browser-based image forensics toolkit: clone detection, ELA, noise analysis, magnifier and metadata. |
| [Karma Decay](http://karmadecay.com/) | — | — | Reverse image search for Reddit to find where and when an image was previously posted. |
| [ExifTool](https://exiftool.org/) | 1k | Perl | Reads, writes and edits metadata in images, documents and media — essential for media verification. |
| [DeepFace](https://github.com/serengil/deepface) | 23k | Python | Lightweight face recognition and facial attribute (age, gender, emotion) framework. |
| [InsightFace](https://github.com/deepinsight/insightface) | 29k | Python | State-of-the-art 2D and 3D face analysis (detection, recognition, alignment) toolkit. |
| [face_recognition](https://github.com/ageitgey/face_recognition) | 56k | Python | Dlib-based "world's simplest" face recognition API for Python and CLI. ⚠️ |
| [CompreFace](https://github.com/exadel-inc/CompreFace) | 8k | Java | Self-hosted, dockerized open-source face recognition system with REST API. |
| [trace.moe](https://trace.moe/) | 5k | JavaScript | Anime scene search that finds the show, episode, and timestamp from a screenshot. |
| [SmartImage](https://github.com/Decimation/SmartImage) | 1.1k | C# | Windows desktop reverse image search aggregator (SauceNAO, IQDB, Ascii2D, trace.moe). |
| [FaceCheck.ID](https://facecheck.id/) | — | Web | Reverse face search that finds where a person's face appears across the public web. |
| [Search4faces](https://search4faces.com/en/) | — | Web | Facial recognition search across VK, Odnoklassniki, TikTok, and Clubhouse avatars. |
| [Lenso.ai](https://lenso.ai/en) | — | Web | AI reverse image search sorting matches into people, places, duplicates, and related. |
| [SauceNAO](https://saucenao.com/) | — | Web | Reverse image search for art/anime across Pixiv, Danbooru, Gelbooru, and more. |
| [ascii2d](https://ascii2d.net/) | — | Web | Japanese reverse image search matching by color and feature hashes. |
| [IQDB](https://iqdb.org/) | — | Web | Multi-service image search across booru sites (Danbooru, Konachan, Gelbooru, Sankaku). |
| [ImgOps](https://imgops.com/) | — | Web | Meta-tool routing an image to many reverse-search, EXIF, and editing utilities. |
| [Photo Sherlock](https://photosherlock.com/) | — | App | Android/iOS app for reverse image search to check if a photo is fake or stolen. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>


## 🔬 Image, Video & Media Forensics

Detect manipulation, deepfakes and AI-generated media, and verify provenance.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Sherloq](https://github.com/GuidoBartoli/sherloq) | 3.2k | Python | Open-source desktop image forensics suite: ELA, JPEG/quantization, noise and resampling analysis. |
| [DeepfakeBench](https://github.com/SCLBD/DeepfakeBench) | 1.1k | Python | Benchmark unifying datasets and 36 state-of-the-art deepfake-detection models. |
| [FaceForensics++](https://github.com/ondyari/FaceForensics) | 2.7k | Python | Benchmark dataset and detection code for face-manipulation methods. ⚠️ |
| [InVID-WeVerify Plugin](https://weverify.eu/verification-plugin/) | — | Web | Browser-extension verification toolbox: video keyframes, magnifier, metadata, reverse search. |
| [MeVer Verification Assistant](https://mever.iti.gr/forensics/) | — | Web | CERTH service bundling tampering-detection, EXIF, GPS and reverse-search for media verification. |
| [Deepware Scanner](https://scanner.deepware.ai/) | — | Web | Free online scanner analyzing videos for facial-manipulation deepfakes with confidence scores. |
| [Content Credentials Verify](https://contentcredentials.org/verify) | — | Web | Official CAI tool to inspect C2PA provenance manifests embedded in images, video and files. |
| [c2patool](https://github.com/contentauth/c2pa-rs) | 360 | Rust | Official C2PA SDK and CLI to read, verify and write content-provenance manifests. |
| [Illuminarty](https://illuminarty.ai/) | — | Web | Detector estimating whether an image is AI-generated, which model made it, and which regions. |
| [ExifCleaner](https://github.com/szTheory/exifcleaner) | 2.5k | TypeScript | Cross-platform GUI (ExifTool-based) to view and strip metadata from images, video and PDFs. |
| [yt-dlp](https://github.com/yt-dlp/yt-dlp) | 174k | Python | Feature-rich CLI downloader for thousands of sites, used to pull source video and frames. |
| [AI or Not](https://www.aiornot.com/) | — | Web | Service classifying images, audio and video as AI-generated or real, including deepfakes. |
| [Reality Defender](https://www.realitydefender.com/) | — | Web | Multimodal deepfake-detection platform (web app + API/SDK) for image, video, audio and text. |
| [Metadata2Go](https://www.metadata2go.com/) | — | Web | Free browser tool to view, edit and remove EXIF/metadata from images, video, audio and PDFs. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>
## 🗺️ Geolocation & GEOINT

Pin down where an image or video was captured using maps, street-level imagery, sun position and feature queries.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [SunCalc](https://www.suncalc.org/) | — | — | Computes sun position and shadow direction for a time and place to verify or chronolocate photos. |
| [Overpass Turbo](https://overpass-turbo.eu/) | — | — | Query and visualize OpenStreetMap data to find places by feature and narrow a geolocation. |
| [Mapillary](https://www.mapillary.com/) | — | — | Crowdsourced street-level imagery for visual ground-truthing where Street View is absent. |
| [KartaView](https://kartaview.org/) | — | — | Open crowdsourced street-level imagery platform, an alternative source for ground-truthing locations. |
| [GeoSpy](https://geospy.ai/) | — | — | AI geolocation engine that predicts where a photo was taken from visual scene features. |
| [GeoHints](https://geohints.com/) | — | — | Reference of country-specific visual clues — bollards, signs, plates — to narrow image geolocation. |
| [Google Earth](https://earth.google.com/) | — | — | Satellite/3D imagery with historical timeline for matching terrain, buildings and confirming a location. |
| [Bellingcat ShadowFinder](https://github.com/bellingcat/ShadowFinder) | 0.6k | Python | Estimates possible locations of a photo from a known shadow length and timestamp. |
| [Wikimapia](https://wikimapia.org/) | — | — | Crowdsourced map with labelled places and points of interest useful for matching landmarks. |
| [Copernicus Browser](https://browser.dataspace.copernicus.eu/) | — | Web | Free browser for Sentinel and Landsat satellite imagery with time-lapse and band analysis. |
| [NASA Worldview](https://worldview.earthdata.nasa.gov/) | — | Web | Browse 1,200+ global daily satellite imagery layers, many within ~3 hours of observation. |
| [Zoom Earth](https://zoom.earth/) | — | Web | Live satellite and weather imagery with storm tracking, fire detection, and overlays. |
| [USGS EarthExplorer](https://earthexplorer.usgs.gov/) | — | Web | Search and download Landsat, aerial photography, and satellite archive datasets. |
| [OpenAerialMap](https://openaerialmap.org/) | — | Web | Open repository of openly-licensed drone and aerial imagery searchable by location. |
| [Maxar Open Data](https://vantor.com/company/open-data-program) | — | Web | Free near-real-time high-resolution satellite imagery for major disaster events. |
| [Picarta](https://www.picarta.ai/) | — | Web | AI photo geolocation predicting where an image was taken from visual clues, no EXIF needed. |
| [Shadowmap](https://shadowmap.org/) | — | Web | Global 3D sun and shadow simulation for any date/time, for shadow-based chronolocation. |
| [PeakVisor](https://peakvisor.com/) | — | Web | 3D mountain and peak identification with AR overlays for terrain-based geolocation. |
| [Instant Street View](https://www.instantstreetview.com/) | — | Web | Jump directly to any address in Google Street View, including historical imagery. |
| [Liveuamap](https://liveuamap.com/) | — | Web | Live interactive map of conflict and security events geolocated from open-source reporting. |
| [Geograph](https://www.geograph.org.uk/) | — | Web | Archive of 8M+ geotagged ground-level photos across Britain and Ireland. |
| [Bellingcat OSM Search](https://github.com/bellingcat/osm-search) | 200 | Vue | Proximity search of OpenStreetMap features to geolocate images by nearby objects. |
| [Nominatim](https://github.com/osm-search/Nominatim) | 4.4k | Python | OpenStreetMap geocoding/reverse-geocoding engine for names, addresses, and coordinates. |
| [QGIS](https://github.com/qgis/QGIS) | 14k | C++ | Free open-source GIS for geospatial analysis and layering imagery, with 200+ algorithms. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 📱 Phone & Identity

Investigate a phone number's carrier, footprint and the accounts and identities linked to it.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [PhoneInfoga](https://github.com/sundowndev/phoneinfoga) | 12k | Go | Reconnaissance framework for phone numbers — identifies carrier, line type, location and footprints. |
| [ignorant](https://github.com/megadose/ignorant) | 1k | Python | Checks whether a phone number is registered on sites like Amazon, Instagram and Snapchat. |
| [Epieos](https://epieos.com/) | — | — | Reverse email and phone lookup revealing linked Google info, profile photos and registered services. |
| [Phonebook.cz](https://phonebook.cz/) | — | — | IntelligenceX tool listing all emails, subdomains and URLs for a domain from indexed data. |
| [NumLookup](https://www.numlookup.com/) | — | — | Free reverse phone lookup returning carrier, line type and registered-name details where available. |
| [Sync.me](https://sync.me/) | — | — | Caller-ID and reverse phone lookup crowdsourced from a large community address book. |
| [libphonenumber](https://github.com/google/libphonenumber) | 18k | C++ | Google's library for parsing, validating and formatting numbers with carrier/region metadata. |
| [email2phonenumber](https://github.com/martinvigo/email2phonenumber) | 2.7k | Python | Derives a target's phone number from their email via password-reset scraping. |
| [Moriarty-Project](https://github.com/AzizKpln/Moriarty-Project) | 2k | Python | Phone-number intelligence: owner, spam risk, related links and socials. |
| [PhoneNumber-OSINT](https://github.com/spider863644/PhoneNumber-OSINT) | 680 | Python | Gathers OSINT information about a given phone number. |
| [numverify](https://numverify.com) | — | API | Phone-number validation API with carrier, line-type and location data. |
| [Twilio Lookup](https://www.twilio.com/docs/lookup) | — | API | Phone validation, carrier, line type and caller-name (CNAM) lookup API. |
| [Truecaller](https://www.truecaller.com) | — | App | Global caller-ID and spam database covering 3B+ phone numbers. |
| [Spy Dialer](https://www.spydialer.com) | — | Web | Free anonymous reverse phone lookup returning US name/carrier data. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🔎 Google Dorking & Search Operators

Advanced search operators and document-harvesting tools to surface exposed files, metadata and hidden pages.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Photon](https://github.com/s0md3v/Photon) | 11k | Python | Fast crawler that extracts URLs, emails, files, secrets and intel from a target for OSINT. |
| [Pagodo](https://github.com/opsdisk/pagodo) | 2.8k | Python | Automates Google dorking — passively scrapes GHDB dorks and runs them against a target domain. |
| [FOCA](https://github.com/ElevenPaths/FOCA) | 2.3k | C# | Finds metadata and hidden info in documents scraped from a target site to map users and software. |
| [Metagoofil](https://github.com/laramies/metagoofil) | 1.1k | Python | Harvests public documents (PDF, DOC, XLS) for a domain and extracts metadata like users and paths. |
| [Google Hacking Database (GHDB)](https://www.exploit-db.com/google-hacking-database) | — | — | Exploit-DB's curated catalog of Google dork queries that surface exposed files, devices and data. |
| [DorkSearch](https://dorksearch.com/) | — | — | Pre-built dork builder and library that speeds up crafting advanced Google search operators. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## ✈️ Transport, RF & SIGINT

Track aircraft, ships and wireless networks in real time using ADS-B, AIS and wardriving datasets.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Flightradar24](https://www.flightradar24.com/) | — | — | Live and historical flight tracking with aircraft details, routes and playback. |
| [ADS-B Exchange](https://www.adsbexchange.com/) | — | — | Unfiltered, community-fed flight tracking showing military and blocked aircraft other trackers hide. |
| [FlightAware](https://www.flightaware.com/) | — | — | Flight tracking and aviation data platform with history, airport activity and aircraft ownership lookups. |
| [MarineTraffic](https://www.marinetraffic.com/) | — | — | Global ship-tracking platform using AIS data with vessel details, positions and port calls. |
| [VesselFinder](https://www.vesselfinder.com/) | — | — | Real-time AIS vessel tracking with ship particulars, photos and historical voyage data. |
| [OpenSky Network](https://opensky-network.org/) | — | — | Research-grade ADS-B flight dataset and API for historical and live aircraft position queries. |
| [WiGLE](https://wigle.net/) | — | — | Crowdsourced database of wireless networks and cell towers mapped by location for wardriving OSINT. |
| [dump1090](https://github.com/flightaware/dump1090) | 1.6k | C | Real-time ADS-B Mode S decoder for RTL-SDR with a live aircraft web map. |
| [readsb](https://github.com/wiedehopf/readsb) | 900 | C | High-performance ADS-B decoder and feeder powering many receiver builds. |
| [tar1090](https://github.com/wiedehopf/tar1090) | 600 | JavaScript | Web interface for live visualization of ADS-B aircraft tracks. |
| [AIS-catcher](https://github.com/jvde-github/AIS-catcher) | 900 | C++ | Multi-SDR AIS receiver decoding ship NMEA with a built-in map server. |
| [OpenRailwayMap](https://www.openrailwaymap.org/) | — | Web | OSM-based worldwide map of railway tracks, signals and infrastructure. |
| [Gqrx](https://github.com/csete/gqrx) | 1.4k | C++ | SDR receiver with spectrum/waterfall for RTL-SDR, Airspy and HackRF. |
| [SDR++](https://github.com/AlexandreRouma/SDRPlusPlus) | 5k | C++ | Cross-platform modern SDR receiver supporting most popular radios. |
| [Universal Radio Hacker](https://github.com/jopohl/urh) | 11k | Python | Investigate and reverse-engineer wireless protocols from raw RF captures. |
| [rtl_433](https://github.com/merbanan/rtl_433) | 6.5k | C | Decodes ISM-band devices (sensors, TPMS, weather stations, key fobs). |
| [SatDump](https://github.com/SatDump/SatDump) | 1.4k | C++ | Capture and decode weather and imaging satellite downlinks. |
| [Gpredict](https://github.com/csete/gpredict) | 900 | C | Real-time satellite tracking and pass prediction. |
| [Kismet](https://www.kismetwireless.net/) | — | C++ | Wireless network/device detector, sniffer and WIDS for Wi-Fi, BT and SDR. |
| [OpenALPR](https://github.com/openalpr/openalpr) | 11k | C++ | Automatic license-plate recognition library for images and video streams. ⚠️ |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## ⛓️ Crypto / Blockchain OSINT

Trace wallets, transactions and entity attribution across Bitcoin, Ethereum and beyond.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Etherscan](https://etherscan.io/) | — | — | Block explorer for Ethereum — inspect addresses, transactions, tokens and smart contracts. |
| [Blockchain.com Explorer](https://www.blockchain.com/explorer) | — | — | Bitcoin and multi-chain block explorer for tracing addresses, transactions and balances. |
| [Blockchair](https://blockchair.com/) | — | — | Multi-blockchain explorer and analytics with powerful filtering across 17+ chains. |
| [Arkham Intelligence](https://www.arkhamintelligence.com/) | — | — | On-chain analytics that de-anonymises wallets and labels entities to follow flows of funds. |
| [Breadcrumbs](https://www.breadcrumbs.app/) | — | — | Visual blockchain investigation tool for mapping and monitoring fund flows between wallets. |
| [WalletExplorer](https://www.walletexplorer.com/) | — | — | Bitcoin wallet-clustering explorer that groups addresses and links them to known services/exchanges. |
| [Chainabuse](https://www.chainabuse.com/) | — | — | Community scam-reporting database for crypto addresses, exchanges and fraudulent schemes. |
| [OXT](https://oxt.me/) | — | — | Bitcoin analytics and exploration platform focused on transaction-graph and clustering research. |
| [Nansen](https://nansen.ai) | — | Web | Wallet-labeling analytics with 500M+ labeled addresses for "smart money" tracking. |
| [MetaSleuth](https://metasleuth.io) | — | Web | Visual cross-chain fund-flow tracing of stolen/scam funds with auto-pathing to CEX/mixers. |
| [MistTrack](https://misttrack.io) | — | Web | AML/sanctions tracking across 19 chains with OFAC/HMT screening and 400M+ labels. |
| [Crystal Intelligence](https://crystalintelligence.com) | — | Web | Blockchain analytics across 330+ chains for tracing illicit funds and entity screening. |
| [GraphSense](https://graphsense.org) | 134 | Python | Open-source, self-hostable cryptoasset analytics for BTC/ETH/Tron money-flow investigation. |
| [OKLink](https://www.oklink.com) | — | Web | Multi-chain Web3 explorer (40+ chains) with address labels and CEX fund-flow dashboards. |
| [Bubblemaps](https://bubblemaps.io) | — | Web | Visual token-holder analytics mapping wallet clusters to expose insider/sybil concentration. |
| [Dune Analytics](https://dune.com) | — | Web | Community SQL/dashboard platform over 100+ chains for custom on-chain queries. |
| [mempool.space](https://mempool.space) | 3k | TypeScript | Open-source Bitcoin block/mempool explorer for fees, unconfirmed tx, RBF and Lightning. |
| [Cielo](https://cielo.finance) | — | Web | Smart-money wallet tracking across 30+ chains with real-time Telegram/Discord alerts. |
| [Bitquery](https://bitquery.io) | — | API | GraphQL/streaming API indexing 40+ chains with Coinpath money-flow tracing. |
| [WalletLabels](https://www.walletlabels.xyz) | — | Web | Labels 200M+ crypto addresses (exchanges, entities, contracts) via web app and API. |
| [Orbit](https://github.com/s0md3v/Orbit) | 613 | Python | Recursively crawls a wallet's history and graphs sources, sinks and suspicious links. ⚠️ |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🦠 Threat Intel & Malware OSINT

Reputation, sandboxing and IOC sources to triage files, URLs, domains and IPs against threat data.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [MISP](https://www.misp-project.org/) | 5.6k | PHP | Open-source threat-intelligence platform for storing, correlating and sharing indicators of compromise. |
| [VirusTotal](https://www.virustotal.com/) | — | — | Analyzes files, URLs, domains and IPs against dozens of AV engines and surfaces related intelligence. |
| [urlscan.io](https://urlscan.io/) | — | — | Sandboxes and screenshots a URL, recording requests, domains, certificates and resources it touches. |
| [Hybrid Analysis](https://www.hybrid-analysis.com/) | — | — | Free malware sandbox that detonates files and URLs and returns behavioural reports and IOCs. |
| [AbuseIPDB](https://www.abuseipdb.com/) | — | — | Community database of reported malicious IPs with abuse-confidence scores and a lookup API. |
| [abuse.ch](https://abuse.ch/) | — | — | URLhaus, MalwareBazaar and ThreatFox — free community feeds of malware samples, URLs and IOCs. |
| [AlienVault OTX](https://otx.alienvault.com/) | — | — | Open Threat Exchange — community-shared pulses of indicators tied to campaigns and malware. |
| [Pulsedive](https://pulsedive.com/) | — | — | Threat-intelligence search engine enriching and scoring indicators with feeds and risk context. |
| [ThreatMiner](https://www.threatminer.org/) | — | — | Free data-mining portal for pivoting on domains, IPs, hashes and malware with passive intel. |
| [Maltiverse](https://maltiverse.com/) | — | — | Threat-intel platform aggregating and classifying IOCs across hundreds of feeds with an API. |
| [ANY.RUN](https://any.run/) | — | Web | Interactive online malware sandbox for detonating samples across Windows, Linux and Android. |
| [Joe Sandbox](https://www.joesecurity.org/) | — | Web | Deep automated dynamic malware/phishing analysis with behavioral reports and IOCs. |
| [Hatching Triage](https://tria.ge/) | — | Web | Scalable automated malware sandbox with config extraction and a free public tier. |
| [CAPE Sandbox](https://github.com/kevoreilly/CAPEv2) | 3.3k | Python | Cuckoo-derived open-source sandbox specializing in unpacking and malware config extraction. |
| [Intezer](https://analyze.intezer.com/) | — | Web | Genetic malware analysis dissecting binaries into code "genes" to trace malware lineage. |
| [MalShare](https://malshare.com/) | — | Web | Free community malware repository for uploading, searching and downloading samples. |
| [vx-underground](https://vx-underground.org/) | — | Web | Largest open collection of malware source code, samples and research papers. |
| [Malpedia](https://malpedia.caad.fkie.fraunhofer.de/) | — | Web | Fraunhofer FKIE's curated malware family intelligence database for family identification. |
| [YARAify](https://yaraify.abuse.ch/) | — | Web | Scans files against a large repository of YARA rules to hunt malware across samples. |
| [OpenCTI](https://github.com/OpenCTI-Platform/opencti) | 9.6k | TypeScript | Open-source platform for managing CTI knowledge and observables, built on STIX2. |
| [IntelOwl](https://github.com/intelowlproject/IntelOwl) | 4.6k | Python | Open-source platform to enrich and manage threat intelligence at scale via a unified API. |
| [Cortex](https://github.com/TheHive-Project/Cortex) | 1.6k | Scala | Engine for analyzing security observables (IPs, emails, URLs, files, hashes) at scale. |
| [Validin](https://www.validin.com/) | — | Web | Pivots across historical DNS, SSL certs and header/favicon hashes to map malicious infra. |
| [JARM](https://github.com/salesforce/jarm) | 1.3k | Python | Active TLS server fingerprinting to group and identify servers (including C2). ⚠️ |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🧅 Dark Web & Paste Sites

Search Tor hidden services, paste dumps and leak archives for selectors tied to a target.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [OnionSearch](https://github.com/megadose/OnionSearch) | 2k | Python | Scrapes URLs from multiple dark-web search engines for a given keyword. |
| [Ahmia](https://ahmia.fi/) | 1k | Python | Search engine that indexes and lists .onion hidden services on the Tor network. |
| [Intelligence X](https://intelx.io/) | — | — | Search engine and archive for leaks, breaches, the dark web, document repos and historical web data. |
| [psbdmp](https://psbdmp.ws/) | — | — | Searchable archive of deleted and public Pastebin dumps for leaked emails, credentials and data. |
| [Pastebin](https://pastebin.com/) | — | — | Public paste host frequently used to dump leaks; searchable via Google dorks for selectors. |
| [DarkOwl](https://www.darkowl.com/) | — | — | Commercial darknet content platform indexing Tor, I2P and paste data for breach and threat monitoring. |
| [TorBot](https://github.com/DedSecInside/TorBot) | 4.2k | Python | Dark web OSINT crawler mapping .onion link relationships and extracting page metadata. |
| [OnionScan](https://github.com/s-rah/onionscan) | 3.3k | Go | Scans Tor hidden services for OPSEC leaks that can deanonymize operators. ⚠️ |
| [TorCrawl.py](https://github.com/MikeMeliz/TorCrawl.py) | 522 | Python | Crawls and extracts regular or .onion pages through Tor with JSON/SQLite export. |
| [darc](https://github.com/JarryShaw/darc) | 222 | Python | Darkweb crawler using requests and Selenium to fetch, render and screenshot sites. |
| [PasteHunter](https://github.com/kevthehermit/PasteHunter) | 1.1k | Python | Scans Pastebin, Gist and ~100 paste sites against YARA rules for exposed secrets. |
| [pystemon](https://github.com/cvandeplas/pystemon) | 334 | Python | Monitors Pastebin-alike sites for regex/keyword hits and stores or alerts on pastes. |
| [pwndb](https://github.com/davidtavarez/pwndb) | 1.4k | Python | CLI tool to search leaked credentials via the pwndb onion service over Tor. ⚠️ |
| [Haystak](https://haystak.com/) | — | Web | Hosted Tor search engine indexing 1.5B+ .onion pages with free and premium tiers. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🏛️ Business, Records & Archives

Corporate registries, leak archives, financial filings and web time machines for following people, money and entities.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Aleph (OCCRP)](https://aleph.occrp.org/) | 2k | Python | Search engine over leaks, public records and corporate datasets for following people, money and entities. |
| [OpenCorporates](https://opencorporates.com/) | — | — | The largest open database of companies — directors, registrations and filings across jurisdictions. |
| [ICIJ Offshore Leaks](https://offshoreleaks.icij.org/) | — | — | Searchable database from the Panama/Paradise/Pandora Papers linking offshore entities and officers. |
| [SEC EDGAR](https://www.sec.gov/edgar) | — | — | US Securities & Exchange Commission filings — company financials, ownership and disclosure records. |
| [UK Companies House](https://find-and-update.company-information.service.gov.uk/) | — | — | Free official UK registry of companies, officers, filings and ownership. |
| [GLEIF LEI Search](https://search.gleif.org/) | — | — | Global Legal Entity Identifier index for verifying and linking legal entities worldwide. |
| [LittleSis](https://littlesis.org/) | — | — | Free database mapping connections between powerful people, companies and institutions. |
| [Wayback Machine](https://web.archive.org/) | — | — | Internet Archive's web time machine for viewing and citing historical snapshots of web pages. |
| [archive.today](https://archive.ph/) | — | — | On-demand web-page archiver that captures and freezes a snapshot of a URL for evidence. |
| [OpenSanctions](https://www.opensanctions.org/) | — | Web | Consolidated global sanctions, PEP and watchlist database with search and API. |
| [North Data](https://www.northdata.com/) | — | Web | Free aggregator of European company data (21+ countries) with officer/shareholder networks. |
| [Pappers](https://www.pappers.fr/) | — | Web | Free French company register (SIREN, accounts, beneficial owners, BODACC notices). |
| [EU BRIS](https://e-justice.europa.eu/topics/registers-business-insolvency-land/business-registers-search-company-eu_en) | — | Web | Official EU portal interconnecting all member-state business registers. |
| [Unternehmensregister](https://www.unternehmensregister.de/en) | — | Web | Germany's central company register: filings, financial accounts and Handelsregister data. |
| [Rusprofile](https://www.rusprofile.ru/) | — | Web | Free profiles of Russian legal entities (EGRUL data, directors, finances, court cases). |
| [Zauba Corp](https://www.zaubacorp.com/) | — | Web | India company research platform with directors, charges and MCA filings. |
| [Tianyancha](https://www.tianyancha.com/) | — | Web | Large Chinese company-information platform (ownership, shareholders, litigation). |
| [ACRA BizFile](https://www.bizfile.gov.sg/) | — | Web | Singapore's official business registry portal for company searches and profiles. |
| [Equasis](https://www.equasis.org/) | — | Web | Free maritime database of vessel ownership, managers and safety/inspection history. |
| [CourtListener](https://www.courtlistener.com/) | — | Web | Free archive of millions of US court opinions plus PACER (RECAP) federal dockets. |
| [judyrecords](https://www.judyrecords.com/) | — | Web | Free full-text search across hundreds of millions of US court cases. |
| [Sayari](https://sayari.com/) | — | Web | Commercial corporate-network and trade-risk graph across global registries. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>


## 🧩 Browser Extensions & Bookmarklets

Run lookups, reverse-image searches and page capture without leaving the browser.

| Tool | Stars | Language | Description |
|------|-------|----------|-------------|
| [Sputnik](https://github.com/Tek-Yum/Sputnik-OSINT-Extension) | 600 | JavaScript | Context-menu OSINT lookups for IPs, domains, hashes, emails and usernames. |
| [Web Archives](https://github.com/dessant/web-archives) | 1.5k | JavaScript | View archived/cached versions of a page across Wayback, Google, Bing and more. |
| [Search by Image](https://github.com/dessant/search-by-image) | 2.4k | JavaScript | Reverse-image search any picture across many engines from the context menu. |
| [RevEye](https://github.com/steven2358/reveye) | 88 | JavaScript | One-click reverse image search via Google, Bing, Yandex, TinEye and Baidu. |
| [Vortimo OSINT Tool](https://www.vortimo.com/) | — | Web | Captures, tags and enriches visited pages into a local searchable evidence store. |
| [Distill Web Monitor](https://distill.io/) | — | Web | Monitors pages or page regions for changes and triggers alerts. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>
## 📚 Datasets, Lists & APIs

Curated tool catalogs, training resources and machine-readable datasets that feed and structure OSINT workflows.

| Tool | Stars | Description |
|------|-------|-------------|
| [Awesome OSINT](https://github.com/jivoi/awesome-osint) | 22k | The canonical community-maintained curated list of OSINT tools and resources by category. |
| [Trace Labs OSINT VM](https://github.com/tracelabs/tlosint-live) | 1k | Kali-based live OSINT operating system preloaded with investigation tools for missing-persons CTFs. |
| [Bellingcat Online Investigation Toolkit](https://bellingcat.gitbook.io/toolkit) | — | Bellingcat's regularly updated, categorized toolkit of investigation tools and guides. |
| [osint-tool-database](https://github.com/tomvaillant/osint-tool-database) | — | Machine-readable structured dataset of OSINT tools for powering apps and finders. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🪦 Deprecated Tools Graveyard

| Dead Tool | Why | Use Instead |
|-----------|-----|-------------|
| twint | Archived Mar 2023, broken by X API changes | snscrape, official X API. |
| Datasploit | Archived, no longer maintained | SpiderFoot, Recon-ng. |

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

---

## Disclosure

Any referral or affiliate links are clearly relevant to OSINT work, and all tools are included based on merit — affiliation does not influence placement or rankings.

<p align="right">(<a href="#readme">⬆ back to top</a>)</p>

## 🔗 Related Awesome Lists

| List | Description |
|------|-------------|
| [awesome-scrapers](https://github.com/edwardtay/awesome-scrapers) | Scrapers, crawlers and extraction tooling — the collection layer that feeds OSINT pipelines. |
| [awesome-ai-apis](https://github.com/edwardtay/awesome-ai-apis) | AI APIs, tools, frameworks and platforms for building intelligent applications. |
| [awesome-robotics](https://github.com/edwardtay/awesome-robotics) | Robotics frameworks, simulators and platforms. |
| [awesome-web3-ai](https://github.com/edwardtay/awesome-web3-ai) | Web3 x AI tools, agent frameworks and protocols. |
| [awesome-compute](https://github.com/edwardtay/awesome-compute) | GPU and compute platforms for training and inference. |

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

- Add tools you've actually used or evaluated
- Include star count and language where applicable
- Note if a tool is unmaintained (last commit >1 year ago)
- Commercial tools/services are fine but must be clearly labeled

Use OSINT responsibly: respect platform terms, privacy law and local regulations. This list is for lawful research, journalism, due diligence and defensive security.


To the extent possible under law, [Edward Tay](https://github.com/edwardtay) has waived all copyright and related or neighboring rights to this work.
