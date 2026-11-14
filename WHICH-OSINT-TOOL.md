# Which OSINT tool should I use?

Pick a tool by what you are trying to find, then check whether it still works. Many of the most-starred OSINT tools on GitHub have not had a commit in years, and modules that scrape live websites break when those sites change.

Checked on **14 November 2026**. "Commits (90d)" counts commits to the default branch from 16 August to 14 November 2026. Release dates fall back to PyPI where a project does not publish GitHub releases. Web service prices come from each service's own site on the same date.

Use these tools on public information, within the law where you work and the terms of the sites you query. Treat every result as a lead to verify.

Back to the full list: [awesome-OSINT](README.md)

## Start from what you have

| You have | Start with | Then |
|---|---|---|
| A username | [Maigret](https://github.com/soxoj/maigret) | [Sherlock](https://github.com/sherlock-project/sherlock) as a second opinion, then open every hit by hand |
| An email address | [Have I Been Pwned](https://haveibeenpwned.com/) for breaches, [Epieos](https://epieos.com/) for linked accounts | [GHunt](https://github.com/mxrch/GHunt) for a Gmail address |
| A phone number | [PhoneInfoga](https://github.com/sundowndev/phoneinfoga) for carrier and region | [Epieos](https://epieos.com/) for linked accounts |
| A domain | [crt.sh](https://crt.sh/) and [subfinder](https://github.com/projectdiscovery/subfinder) for subdomains | [theHarvester](https://github.com/laramies/theHarvester) for emails and hosts, [dnstwist](https://github.com/elceef/dnstwist) for lookalike domains |
| An IP address or exposed service | [Shodan](https://www.shodan.io/) or [Censys](https://search.censys.io/) | [GreyNoise](https://www.greynoise.io/) to check whether a source IP is a known internet-wide scanner |
| A photo | Google Lens, Yandex, Bing and TinEye in turn | [ExifTool](https://exiftool.org/) if you have the original file, then [SunCalc](https://www.suncalc.org/) and [Overpass Turbo](https://overpass-turbo.eu/) to confirm a location |
| A social media account | [Instaloader](https://github.com/instaloader/instaloader) for Instagram, [twscrape](https://github.com/vladkens/twscrape) for X | Archive what you find before it is deleted |
| A crypto wallet | A block explorer ([Etherscan](https://etherscan.io/), [Blockchair](https://blockchair.com/)) | [Arkham](https://www.arkhamintelligence.com/) or [Breadcrumbs](https://www.breadcrumbs.app/) for labels and flow graphs |
| A whole case to run | [Maltego](https://www.maltego.com/) for link graphs | [theHarvester](https://github.com/laramies/theHarvester) and the tools above, fed into one notes file |

## What changed recently

- **WhatsMyName closed on 9 November 2026.** Its maintainer archived the repo, and the final dataset of 691 sites stays online at its old URL. Tools that read that file, including [blackbird](https://github.com/antoniaci/blackbird), keep working, but detections will drift as sites change.
- **Several popular tools have stopped moving.** No commits for a year or more: [Holehe](https://github.com/megadose/holehe) (last commit September 2024), [SpiderFoot](https://github.com/smicallef/spiderfoot) (November 2023, last release April 2022), [Mosint](https://github.com/alpkeskin/mosint) (September 2023), [snscrape](https://github.com/JustAnotherArchivist/snscrape) (June 2023), [ignorant](https://github.com/megadose/ignorant) (December 2023) and [h8mail](https://github.com/khast3x/h8mail) (June 2022). Some still run. Test them on an account you control before you rely on a result.
- **The busiest projects** in the last 90 days are [Maigret](https://github.com/soxoj/maigret) (255 commits), [theHarvester](https://github.com/laramies/theHarvester) (254), [subfinder](https://github.com/projectdiscovery/subfinder) (75) and [Instaloader](https://github.com/instaloader/instaloader) (63).

## Usernames

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [Maigret](https://github.com/soxoj/maigret) | Checks 3,000+ sites and parses profile pages for names, links and other IDs to pivot on | MIT | v0.6.6 (Sep 2026) | 255 | A full scan is slow. Start with the top sites and widen from there. |
| [Sherlock](https://github.com/sherlock-project/sherlock) | Checks whether a username exists on hundreds of sites | MIT | v0.16.2 (Sep 2026) | 10 | Reports existence only. Sites that answer every URL with a page give false positives. |
| [WhatsMyName](https://github.com/WebBreacher/WhatsMyName) | Community dataset of username detections, with a web app | CC BY-SA 4.0 | none | archived | Closed 9 November 2026. Data frozen at 691 sites. |
| [blackbird](https://github.com/antoniaci/blackbird) | Fast username and email search built on WhatsMyName data | none stated | none | 8 | Inherits WhatsMyName's frozen detections. No license file in the repo. |
| [Snoop](https://github.com/snooppr/snoop) | Username search across 5,000+ sites in the full version | Custom | v1.4.3 (Jan 2026) | 13 | Licensed for personal use only; other use needs written permission. The free demo database is much smaller. |
| [Social-Analyzer](https://github.com/qeeqbox/social-analyzer) | Finds and scores profiles across 1,000+ sites, with a web UI | AGPL-3.0 | 0.45 on PyPI (May 2022) | 2 | No PyPI release since 2022. |

## Email and phone

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [GHunt](https://github.com/mxrch/GHunt) | Investigates a Google account from a Gmail address: name, photos, reviews, calendar | AGPL-3.0 | 2.3.4 on PyPI (Mar 2026) | 0 | Needs cookies from a Google account you log in with. Use a separate account. |
| [Holehe](https://github.com/megadose/holehe) | Checks which sites an email is registered on through password-reset and sign-up flows | GPL-3.0 | 1.61 on PyPI (Jul 2022) | 0 | No commits since September 2024. Modules break silently as sites change their forms. |
| [Mosint](https://github.com/alpkeskin/mosint) | Email OSINT that combines breach, social and DNS lookups | MIT | v3.0.0 (Sep 2023) | 0 | No commits since September 2023. Most sources need your own API keys. |
| [h8mail](https://github.com/khast3x/h8mail) | Breach hunting against breach APIs and local dumps | BSD-3-Clause | 2.5.6 (Jun 2022) | 0 | No commits since June 2022. |
| [PhoneInfoga](https://github.com/sundowndev/phoneinfoga) | Phone number format, carrier and region, plus search links for footprints | GPL-3.0 | v2.11.0 (Feb 2024) | 3 | No release since February 2024. Its own scanners give number metadata; finding a person still takes manual searching. |
| [ignorant](https://github.com/megadose/ignorant) | Checks whether a phone number is registered on a few large sites | GPL-3.0 | none | 0 | No commits since December 2023. |

## Domains and infrastructure

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [theHarvester](https://github.com/laramies/theHarvester) | Collects emails, names, subdomains, hosts and URLs for a domain from public sources | GPL-2.0 | 4.11.1 (Jun 2026) | 254 | Many of its sources only return data with your own API keys. |
| [subfinder](https://github.com/projectdiscovery/subfinder) | Fast passive subdomain discovery | MIT | v2.17.0 (Oct 2026) | 75 | Results improve a lot once you add free API keys for its sources. |
| [OWASP Amass](https://github.com/owasp-amass/amass) | Deep attack-surface mapping with passive and active DNS | Apache-2.0 | v5.1.3 (Oct 2026) | 4 | Major versions change configuration and output. Pin a version in scripts. |
| [dnstwist](https://github.com/elceef/dnstwist) | Generates lookalike domains and checks which are registered, for phishing and typosquat hunting | Apache-2.0 | 20250130 (Jan 2025) | 0 | Quiet since April 2025, but the job is stable and it still runs. |
| [uncover](https://github.com/projectdiscovery/uncover) | Queries Shodan, Censys, FOFA and others from one command | MIT | v1.2.1 (May 2026) | 18 | Uses your own keys for each engine, so you pay each engine's limits. |

## Images and geolocation

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [ExifTool](https://exiftool.org/) | Reads camera, GPS and edit metadata from images, video and documents | GPL-3.0 or Artistic | exiftool.org | 4 | Most social platforms strip metadata on upload. Ask for the original file. |
| [ShadowFinder](https://github.com/bellingcat/ShadowFinder) | Estimates where a photo could have been taken from an object's height, its shadow length and the photo's date and time | MIT | 0.7.1 (Sep 2026) | 3 | Gives a band of possible locations. Combine it with other clues. |

Reverse image search works best when you run the same image through several engines: Google Lens for objects and places, Yandex for faces and buildings, TinEye for matching copies sorted by the date it first crawled them, and Bing for Western web matches.

## Social media

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [Instaloader](https://github.com/instaloader/instaloader) | Downloads Instagram posts, stories, profile data and comments | MIT | v4.16 (Oct 2026) | 63 | Instagram rate-limits heavily and can block the account you log in with. |
| [twscrape](https://github.com/vladkens/twscrape) | X search, profiles, followers and posts through a pool of logged-in accounts | MIT | v0.21.0 (Nov 2026) | 35 | Needs X accounts, which X may suspend. Check X's terms for your use. |
| [snscrape](https://github.com/JustAnotherArchivist/snscrape) | Multi-network scraper | GPL-3.0 | none | 0 | No commits since June 2023. Its X module stopped working when X closed logged-out access. |

## Investigation frameworks

| Tool | What it does | License | Latest release | Commits (90d) | Watch out for |
|---|---|---|---|---|---|
| [SpiderFoot](https://github.com/smicallef/spiderfoot) | Automated scan with 200+ modules across IPs, domains, emails and names | MIT | v4.0 (Apr 2022) | 0 | No commits since November 2023. Modules that call third-party APIs fail as those APIs change. |
| [Recon-ng](https://github.com/lanmaster53/recon-ng) | Modular web recon framework with a Metasploit-style console | GPL-3.0 | none | 1 | Most useful modules need API keys. |
| [sn0int](https://github.com/kpcyrd/sn0int) | Semi-automatic OSINT framework with a module registry | GPL-3.0 | v0.26.1 (Sep 2024) | 2 | No release since September 2024. |
| [Osmedeus](https://github.com/j3ssie/osmedeus) | Workflow engine for reconnaissance and attack-surface scans | MIT | v5.1.2 (Oct 2026) | 9 | Built for bug bounty recon. Heavy for people-focused work. |

## Web services: what is free

What you get without paying, from each service's own pricing or help pages. "Not stated" means the page did not say.

| Service | Free use | Account for free use | Cheapest paid | Limit worth knowing |
|---|---|---|---|---|
| [Have I Been Pwned](https://haveibeenpwned.com/) | Email search in the browser | Not stated | API from $4.39/mo, billed yearly | Stealer-log data needs the Pro plan, from $379/mo |
| [Hunter.io](https://hunter.io/) | 50 credits a month | Yes | $49/mo, or $34/mo billed yearly | Credits do not roll over |
| [crt.sh](https://crt.sh/) | Full search | No | None | |
| [DNSDumpster](https://dnsdumpster.com/) | Basic tier | Yes | $79/yr (on sale at $49) | Basic: 50 requests a day, 50 subdomains each |
| [Shodan](https://www.shodan.io/) | Free account and API key | Yes | $49 once for a lifetime membership, or $69/mo | Membership gives 100 query credits a month. The API allows 1 request a second |
| [Censys](https://search.censys.io/) | Standard ports and services | Yes | Contact sales | |
| [GreyNoise](https://www.greynoise.io/) | 50 searches a week | Yes | Contact sales | 10 days of history on the free tier |
| [PimEyes](https://pimeyes.com/) | 10 searches a day | Not stated | Not stated | Free results show that matches exist but hide most source links |
| [TinEye](https://tineye.com/) | Free for non-commercial use | Not stated | API search bundles from 5,000 searches | Commercial use needs the API |
| [GeoSpy](https://geospy.ai/) | Demo only | | Licences for government and enterprise | |
| [SunCalc](https://www.suncalc.org/), [Overpass Turbo](https://overpass-turbo.eu/), [WhatsMyName](https://whatsmyname.app/) | Free | No | None | WhatsMyName's data is frozen since 9 November 2026 |
| [Phonebook.cz](https://phonebook.cz/) | None | IntelX login | Paid IntelX licence | |
| [MetaSleuth](https://metasleuth.io/) | 200 investigations a month | Not stated | $30/mo | Free covers 11 chains and 1 monitored address |
| [Chainabuse](https://www.chainabuse.com/) | Search reported addresses and URLs | No | Partner access on request | Free API key: 10 calls a month |
| [Maltego](https://www.maltego.com/) | Basic edition, 200 credits | Not stated | Entry: €3,000/yr, after vetting | |
| [Hunchly](https://hunch.ly/) | Free trial | Not stated | $169/yr | Case data stays on your own computer |

Epieos, DeHashed, SecurityTrails, Arkham and Breadcrumbs blocked automated reads of their pricing pages on the check date, so they are left out here.

## How this page is checked

- GitHub numbers come from the GitHub API on the date at the top. Commit counts show activity: a busy repo can still miss your target site, and a quiet one can be finished software.
- Web service details come from each service's own pricing or help pages. Anything a page did not state is left out.
- Spotted something out of date? [Open an issue](https://github.com/edwardtay/awesome-OSINT/issues/new/choose) or a pull request.

<p align="right">(<a href="#which-osint-tool-should-i-use">⬆ back to top</a>)</p>
