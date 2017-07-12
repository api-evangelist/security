---
published: true
layout: post
title: Opportunity To Develop A Threat Intelligence Aggregation API
date: 2017-07-10T09:00:00.000Z
tags:
  - API Evangelist
  - Security
  - Cybersecurity
  - Project
image: >-
  https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/facing-cannon_copper_circuit.jpg
---
<p><img src="https://s3.amazonaws.com/kinlane-productions/algo-rotoscope/stories/facing-cannon_copper_circuit.jpg" align="right" width="40%" style="padding: 15px;" /></p>I came across [this valuable list of threat intelligence resources](https://github.com/hslatman/awesome-threat-intelligence) and think that the section on information sources should be aggregated and provided as a single threat intelligence API. When I come across valuable information repos like this my first impulse is to go through them, standardize and upload as JSON and YAML to Github, making all of this data forkable, and available via an API.

Of course if I responded to every impulse like this I would never get any of my normal work done, and actually pay my bills. A second option for me is to put things out there publicly in hopes that a) someone will pay me to do the work, or b) someone else who has more time, and the rent paid will tackle the work. With this in mind, this list of sources should be standardized, and publish to Github and as an API:

<table>
    <tr>
        <td>
            <a href="http://s3.amazonaws.com/alexa-static/top-1m.csv.zip" target="_blank">Alexa Top 1 Million sites</a>
        </td>
        <td>
            Probable Whitelist of the top 1 Million sites from Amazon(Alexa).
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://docs.google.com/spreadsheets/u/1/d/1H9_xaxQHpWaa4O_Son4Gx0YOIzlcBWMsdvePFX68EKU/pubhtml" target="_blank">APT Groups and Operations</a>
        </td>
        <td>
            A spreadsheet containing information and intelligence about APT groups, operations and tactics.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.autoshun.org/" target="_blank">AutoShun</a>
        </td>
        <td>
            A public service offering at most 2000 malicious IPs and some more resources.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.circl.lu/projects/bgpranking/" target="_blank">BGP Ranking</a>
        </td>
        <td>
            Ranking of ASNs having the most malicious content.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://intel.malwaretech.com/" target="_blank">Botnet Tracker</a>
        </td>
        <td>
            Tracks several active botnets.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://danger.rulez.sk/projects/bruteforceblocker/" target="_blank">BruteForceBlocker</a>
        </td>
        <td>
            BruteForceBlocker is a perl script that monitors a server's sshd logs and identifies brute force attacks, which it then uses to automatically configure firewall blocking rules and submit those IPs back to the project site, <a href="http://danger.rulez.sk/projects/bruteforceblocker/blist.php">http://danger.rulez.sk/projects/bruteforceblocker/blist.php</a>.
        </td>
    </tr>    
    <tr>
        <td>
            <a href="http://osint.bambenekconsulting.com/feeds/c2-ipmasterlist.txt" target="_blank">C&amp;C Tracker</a>
        </td>
        <td>
            A feed of known, active and non-sinkholed C&amp;C IP addresses, from Bambenek Consulting.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://cinsscore.com/list/ci-badguys.txt" target="_blank">CI Army List</a>
        </td>
        <td>
        A subset of the commercial <a href="http://cinsscore.com/">CINS Score</a> list, focused on poorly rated IPs that are not currently present on other threatlists.
        </td>
    </tr>    
    <tr>
        <td>
            <a href="http://s3-us-west-1.amazonaws.com/umbrella-static/index.html" target="_blank">Cisco Umbrella</a>
        </td>
        <td>
            Probable Whitelist of the top 1 million sites resolved by Cisco Umbrella (was OpenDNS).
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://intel.criticalstack.com/" target="_blank">Critical Stack Intel</a>
        </td>
        <td>
            The free threat intelligence parsed and aggregated by Critical Stack is ready for use in any Bro production system. You can specify which feeds you trust and want to ingest.
        </td>
    </tr>
     <tr>
        <td>
            <a href="https://www.c1fapp.com/" target="_blank">C1fApp</a>
        </td>
        <td>
            C1fApp is a threat feed aggregation application, providing a single feed, both Open Source and private. Provides statistics dashboard, open API for search and is been running for a few years now. Searches are on historical data.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.cymon.io/" target="_blank">Cymon</a>
        </td>
        <td>
            Cymon is an aggregator of indicators from multiple sources with history, so you have a single interface to multiple threat feeds. It also provides an API to search a database along with a pretty web interface.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://intel.deepviz.com/recap_network.php" target="_blank">Deepviz Threat Intel</a>
        </td>
        <td>
            Deepviz offers a sandbox for analyzing malware and has an API available with threat intelligence harvested from the sandbox.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://rules.emergingthreats.net/fwrules/" target="_blank">Emerging Threats Firewall Rules</a>
        </td>
        <td>
            A collection of rules for several types of firewalls, including iptables, PF and PIX.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://rules.emergingthreats.net/blockrules/" target="_blank">Emerging Threats IDS Rules</a>
        </td>
        <td>
            A collection of Snort and Suricata <i>rules</i> files that can be used for alerting or blocking.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://exonerator.torproject.org/" target="_blank">ExoneraTor</a>
        </td>
        <td>
            The ExoneraTor service maintains a database of IP addresses that have been part of the Tor network.  It answers the question whether there was a Tor relay running on a given IP address on a given date.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://www.exploitalert.com/" target="_blank">Exploitalert</a>
        </td>
        <td>
            Listing of latest exploits released.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://feodotracker.abuse.ch/" target="_blank">ZeuS Tracker</a>
        </td>
        <td>
            The Feodo Tracker <a href="https://www.abuse.ch/" target="_blank">abuse.ch</a> tracks the Feodo trojan.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://iplists.firehol.org/" target="_blank">FireHOL IP Lists</a>
        </td>
        <td>
            400+ publicly available IP Feeds analysed to document their evolution, geo-map, age of IPs, retention policy, overlaps. The site focuses on cyber crime (attacks, abuse, malware).
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://fraudguard.io/" target="_blank">FraudGuard</a>
        </td>
        <td>
            FraudGuard is a service designed to provide an easy way to validate usage by continuously collecting and analyzing real-time internet traffic.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://hailataxii.com/" target="_blank">Hail a TAXII</a>
        </td>
        <td>
            Hail a TAXII.com is a repository of Open Source Cyber Threat Intelligence feeds in STIX format. They offer several feeds, including some that are listed here already in a different format, like the Emerging Threats rules and PhishTank feeds.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.iblocklist.com/lists" target="_blank">I-Blocklist</a>
        </td>
        <td>
            I-Blocklist maintains several types of lists containing IP addresses belonging to various categories. Some of these main categories include countries, ISPs and organizations. Other lists include web attacks, TOR, spyware and proxies. Many are free to use, and available in various formats.
        </td>
    </tr>
    <tr>
    <tr>
        <td>
            <a href="https://majestic.com/reports/majestic-million" target="_blank">Majestic Million</a>
        </td>
        <td>
            Probable Whitelist of the top 1 million web sites, as ranked by Majestic. Sites are ordered by the number of referring subnets. More about the ranking can be found on their <a href="https://blog.majestic.com/development/majestic-million-csv-daily/" target="_blank">blog</a>.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://www.malshare.com/" target="_blank">MalShare.com</a>
        </td>
        <td>
            The MalShare Project is a public malware repository that provides researchers free access to samples.
        </td>
    </tr>    
    <tr>
        <td>
            <a href="http://www.malwaredomains.com/" target="_blank">MalwareDomains.com</a>
        </td>
        <td>
            The DNS-BH project creates and maintains a listing of domains that are known to be used to propagate malware and spyware. These can be used for detection as well as prevention (sinkholing DNS requests).
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.metadefender.com/threat-intelligence-feeds" target="_blank">Metadefender.com</a>
        </td>
        <td>
            Metadefender Cloud Threat Intelligence Feeds contains top new malware hash signatures, including MD5, SHA1, and SHA256. These new malicious hashes have been spotted by Metadefender Cloud within the last 24 hours. The feeds are updated daily with newly detected and reported malware to provide actionable and timely threat intelligence.
        </td>
    </tr>   
    <tr>
        <td>
            <a href="https://services.normshield.com" target="_blank">NormShield Services</a>
        </td>
        <td>
            NormShield Services provide thousands of domain information (including whois information) that potential phishing attacks may come from. Breach and blacklist services also available. There is free sign up for public services for continuous monitoring.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://www.openbl.org/lists.html" target="_blank">OpenBL.org</a>
        </td>
        <td>
            A feed of IP addresses found to be attempting brute-force logins on services such as SSH, FTP, IMAP and phpMyAdmin and other web applications.
        </td>
    </tr>    
    <tr>
        <td>
            <a href="https://openphish.com/phishing_feeds.html" target="_blank">OpenPhish Feeds</a>
        </td>
        <td>
            OpenPhish receives URLs from multiple streams and analyzes them using its proprietary phishing detection algorithms. There are free and commercial offerings available.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.phishtank.com/developer_info.php" target="_blank">PhishTank</a>
        </td>
        <td>
            PhishTank delivers a list of suspected phishing URLs. Their data comes from human reports, but they also ingest external feeds where possible. It's a free service, but registering for an API key is sometimes necessary.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://ransomwaretracker.abuse.ch/" target="_blank">Ransomware Tracker</a>
        </td>
        <td>
            The Ransomware Tracker by <a href="https://www.abuse.ch/" target="_blank">abuse.ch</a> tracks and monitors the status of domain names, IP addresses and URLs that are associated with Ransomware, such as Botnet C&mp;C servers, distribution sites and payment sites.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://isc.sans.edu/suspicious_domains.html" target="_blank">SANS ICS Suspicious Domains</a>
        </td>
        <td>
            The Suspicious Domains Threat Lists by <a href="https://isc.sans.edu/suspicious_domains.html" target="_blank">SANS ICS</a> tracks suspicious domains. It offers 3 lists categorized as either <a href="https://isc.sans.edu/feeds/suspiciousdomains_High.txt" target="_blank">high</a>, <a href="https://isc.sans.edu/feeds/suspiciousdomains_Medium.txt" target="_blank">medium</a> or <a href="https://isc.sans.edu/feeds/suspiciousdomains_Low.txt" target="_blank">low</a> sensitivity, where the high sensitivity list has fewer false positives, whereas the low sensitivty list with more false positives. There is also an <a href="https://isc.sans.edu/feeds/suspiciousdomains_whitelist_approved.txt" target="_blank">approved whitelist</a> of domains.<br/>
            Finally, there is a suggested <a href="https://isc.sans.edu/block.txt" target="_blank">IP blocklist</a> from <a href="https://dshield.org">DShield</a>.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://github.com/Neo23x0/signature-base" target="_blank">signature-base</a>
        </td>
        <td>
            A database of signatures used in other tools by Neo23x0.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.spamhaus.org/" target="_blank">The Spamhaus project</a>
        </td>
        <td>
            The Spamhaus Project contains multiple threatlists associated with spam and malware activity.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://sslbl.abuse.ch/" target="_blank">SSL Blacklist</a>
        </td>
        <td>
            SSL Blacklist (SSLBL) is a project maintained by abuse.ch. The goal is to provide a list of "bad" SSL certificates identified by abuse.ch to be associated with malware or botnet activities. SSLBL relies on SHA1 fingerprints of malicious SSL certificates and offers various blacklists
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://statvoo.com/dl/top-1million-sites.csv.zip" target="_blank">Statvoo Top 1 Million Sites</a>
        </td>
        <td>
            Probable Whitelist of the top 1 million web sites, as ranked by Statvoo.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://strongarm.io" target="_blank">Strongarm, by Percipient Networks</a>
        </td>
        <td>
            Strongarm is a DNS blackhole that takes action on indicators of compromise by blocking malware command and control. Strongarm aggregates free indicator feeds, integrates with commercial feeds, utilizes Percipient's IOC feeds, and operates DNS resolvers and APIs for you to use to protect your network and business. Strongarm is free for personal use.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://www.talosintelligence.com/aspis/" target="_blank">Talos Aspis</a>
        </td>
        <td>
            Project Aspis is a closed collaboration between Talos and hosting providers to identify and deter major threat actors. Talos shares its expertise, resources, and capabilities including network and system forensics, reverse engineering, and threat intelligence at no cost to the provider.
        </td>
    </tr>
    <tr>
        <td>
            <a href="http://www.threatglass.com/" target="_blank">Threatglass</a>
        </td>
        <td>
            An online tool for sharing, browsing and analyzing web-based malware. Threatglass allows users to graphically browse website infections by viewing screenshots of the stages of infection, as well as by analyzing network characteristics such as host relationships and packet captures.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://www.threatminer.org/" target="_blank">ThreatMiner</a>
        </td>
        <td>
            ThreatMiner has been created to free analysts from data collection and to provide them a portal on which they can carry out their tasks, from reading reports to pivoting and data enrichment.
            The emphasis of ThreatMiner isn't just about indicators of compromise (IoC) but also to provide analysts with contextual information related to the IoC they are looking at.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://virusshare.com/" target="_blank">VirusShare</a>
        </td>
        <td>
            VirusShare.com is a repository of malware samples to provide security researchers, incident responders, forensic analysts, and the morbidly curious access to samples of malicious code. Access to the site is granted via invitation only.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://github.com/Yara-Rules/rules" target="_blank">Yara-Rules</a>
        </td>
        <td>
            An open source repository with different Yara signatures that are compiled, classified and kept as up to date as possible.
        </td>
    </tr>
    <tr>
        <td>
            <a href="https://zeustracker.abuse.ch/" target="_blank">ZeuS Tracker</a>
        </td>
        <td>
            The ZeuS Tracker by <a href="https://www.abuse.ch/" target="_blank">abuse.ch</a> tracks ZeuS Command & Control servers (hosts) around the world and provides you a domain- and a IP-blocklist.
        </td>
    </tr>
</table>

<p>Ideally, [each source on this list](https://github.com/hslatman/awesome-threat-intelligence) would be publishing a forkable version of their data on Github and/or deploying a simple web API, but alas it isn't the world we live in. Part of the process to standardardize and normalize the threat intelligence from all of these source would be to reach out to each provider, and take their temperature regarding working together to improve the data source by itself, as well as part of an aggregated set of data and API sources.</p>

<p>Similar to what I'm trying to do across many of the top business sectors being impacted by APIs, we need to to work aggregating all the existing sources of threat intelligence, and begin identifying a common schema that any new player could adopt. We need an open data schema, API definition, as well as suite of open source server and client tooling to emerge, if we are going to stay ahead of the cybersecurity storm that has engulfed us, and will continue to surround us until we work together to push it back.</p>
