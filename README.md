# Awesome OSINT [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Stars](https://img.shields.io/github/actions/workflow/status/edwardtay/awesome-OSINT/update-stars.yml?label=star%20updates)](https://github.com/edwardtay/awesome-OSINT/actions/workflows/update-stars.yml)
[![Links](https://img.shields.io/github/actions/workflow/status/edwardtay/awesome-OSINT/links.yml?label=links)](https://github.com/edwardtay/awesome-OSINT/actions/workflows/links.yml)
[![Last Commit](https://img.shields.io/github/last-commit/edwardtay/awesome-OSINT)](https://github.com/edwardtay/awesome-OSINT/commits/main)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/edwardtay/awesome-OSINT/pulls)
[![License: CC0](https://img.shields.io/badge/License-CC0-lightgrey.svg)](LICENSE)

> A curated list of open-source intelligence (OSINT) tools — people search, domains, social media, geolocation, breach data, and investigation frameworks.

> ⚠️ = known maintenance concern; verify repository status before adoption.

## 🧭 The OSINT Stack

This list is the **catalog layer** of an OSINT ecosystem — it tells you *what exists*. Two downstream layers turn that catalog into action:

- **🔎 Try them live → [pwnsy OSINT Search](https://search.pwnsy.com)** and the **[pwnsy Tool Finder](https://pwnsy.com)** — describe what you want to find in plain English and pwnsy picks the right tools from this catalog and runs them for you, no installation required.
- **📓 Learn the methodology → [OSINT field notes](https://notebooks.lever-labs.com/osint/)** — the workflow, opsec, and legal/ethics guide that explains *how* to chain these tools into a sound investigation.

The loop: **this list = what exists** → **the notebook = how to use it** → **pwnsy = run it without installing anything**. Browse a category below, read the field notes to understand the technique, then jump to pwnsy to execute.

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

## ✈️ Transport Tracking

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

This list is the catalog layer of an OSINT ecosystem that also includes [pwnsy](https://pwnsy.com) (a hosted tool finder/runner) and the [OSINT field notes](https://notebooks.lever-labs.com/osint/) study guide, both maintained by the same author. Any referral or affiliate links are clearly relevant to OSINT work, and all tools are included based on merit — affiliation does not influence placement or rankings.

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
