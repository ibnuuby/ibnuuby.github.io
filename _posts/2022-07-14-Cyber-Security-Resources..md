---
title: "Cyber Security Resources"
author: Ibnu Ubaeydillah
layout: post
comments: true
permalink: /Cyber-Security-Resources/
categories: Genel
tags: [resources, all-post]
---

Hai disini saya mengumpulkan bahan belajar tentang cyber security yang telah saya kumpulkan, semoga resource yang saya kumpulkan ini dapat bermanfaat untuk teman-teman yang giat belajar tentang cyber security, bagi yang ingin berkontribusi dalam resource ini, silakan bisa menghubungi saya di [`@xcore13x`](https://twitter.com/xcore13x). 


## Content
- [Introduce Cyber Security](#Introduce-Cyber-Security)
- [Cyber Security Career Roadmap](#cyber-security-career-roadmap)
- [Cyber Security Awareness](#Cyber-Security-Awareness)
- [Web Application Hacking/Security](#web-application-hackingsecurity)
  - [Local File Inclusion](#local-file-inclusion)
  - [Open Redirect](#open-redirect)
  - [Cross-Site Request Forgery (CSRF)](#cross-site-request-forgery-csrf)
  - [Cross-Site Scripting (XSS)](#cross-site-scripting-xss)
  - [Insecure Direct Object References (IDOR)](#insecure-direct-object-references-idor)
  - [SQL Injection](#sql-injection)
- [Red Team](#red-team)
  - [Initial Access](#initial-access)
  - [Execution](#execution)
  - [Persistence](#persistence)
  - [Privilege Escalation](#privilege-escalation)
  - [Defense Evasion](#defense-evasion)
  - [Credential Access](#credential-access)
  - [Discovery](#discovery)
  - [Lateral Movement](#lateral-movement)
  - [Collection](#collection)
  - [Exfiltration](#exfiltration)
  - [Command and Control](#command-and-control)
  - [Embedded and Peripheral Devices Hacking](#embedded-and-peripheral-devices-hacking)
  - [Misc](#misc)
  - [RedTeam Gadgets](#redTeam-gadgets)
  - [Training](#training)
  - [Certification](#certification)
- [Blue Team](#blue-team)
  - [Automation](#automation)
    - [Code libraries and bindings](#code-libraries-and-bindings)
    - [Security Orchestration, Automation, and Response (SOAR)](#security-orchestration-automation-and-response-soar)
  - [Cloud platform security](#cloud-platform-security)
    - [Distributed monitoring](#distributed-monitoring)
    - [Kubernetes](#kubernetes)
    - [Service meshes](#service-meshes)
  - [Communications security (COMSEC)](#communications-security-comsec)
  - [DevSecOps](#devsecops)
    - [Application or Binary Hardening](#application-or-binary-hardening)
    - [Compliance testing and reporting](#compliance-testing-and-reporting)
    - [Dependency confusion](#dependency-confusion)
    - [Fuzzing](#fuzzing)
    - [Policy enforcement](#policy-enforcement)
    - [Supply chain security](#supply-chain-security)
  - [Honeypots](#honeypots)
    - [Tarpits](#tarpits)
  - [Host-based tools](#host-based-tools)
    - [Sandboxes](#sandboxes)
  - [Identity and AuthN/AuthZ](#identity-and-authnauthz)
  - [Incident Response tools](#incident-response-tools)
    - [IR management consoles](#ir-management-consoles)
    - [Evidence collection](#evidence-collection)
  - [Network perimeter defenses](#network-perimeter-defenses)
    - [Firewall appliances or distributions](#firewall-appliances-or-distributions)
  - [Operating System distributions](#operating-system-distributions)
  - [Phishing awareness and reporting](#phishing-awareness-and-reporting)
  - [Preparedness training and wargaming](#preparedness-training-and-wargaming)
  - [Security configurations](#security-configurations)
  - [Security monitoring](#security-monitoring)
    - [Endpoint Detection and Response (EDR)](#endpoint-detection-and-response-edr)
    - [Network Security Monitoring (NSM)](#network-security-monitoring-nsm)
    - [Security Information and Event Management (SIEM)](#security-information-and-event-management-siem)
    - [Service and performance monitoring](#service-and-performance-monitoring)
    - [Threat hunting](#threat-hunting)
  - [Threat intelligence](#threat-intelligence)
    - [Fingerprinting](#fingerprinting)
    - [Threat signature packages and collections](#threat-signature-packages-and-collections)
  - [Tor Onion service defenses](#tor-onion-service-defenses)
  - [Transport-layer defenses](#transport-layer-defenses)
    - [Overlay and Virtual Private Networks (VPNs)](#overlay-and-virtual-private-networks-vpns)
  - [macOS-based defenses](#macos-based-defenses)
  - [Windows-based defenses](#windows-based-defenses)
    - [Active Directory](#active-directory)
  - [Reverse Engineering](#reverse-engineering)
  - [Malware Analysis](#malware-analysis)
- [Bug Bounty](#bug-bounty)
  - [Story Bug Hunting](#story-bug-hunting)
- [Resources Cyber Security from Twitter](#resources-cyber-security-from-twitter)
- [Cyber-Security-Books](#cyber-security-books)
- [OSCP-Resources](#oscp-resources)
  - [Oscp Repo](#oscp-repo)
  - [TJnulls-OSCP-Prep-Guide](#tjnull-oSCP-prep-guide)

------

## Introduce Cyber Security
- [Pengenalan Cyber Security](https://www.youtube.com/watch?v=pTQ2VcdcObU&t=6s) - OVIS UI
- [Cyber Security Fundamental (Bahasa Indonesia) - Core Security Principles](https://youtu.be/yIzsTukZ8e4) -Moklet Teach ID
- [Ruang Lingkup Cyber Security](https://www.youtube.com/watch?v=BNcaTTglmRA) - OVIS UI
- [Cyber Security 101: Filosofi Dasar Keamanan Siber](https://youtu.be/on742mcT4jo) - Manajemen TI
- [Mendeteksi dan Mengatasi Insiden Cyber Security](https://youtu.be/JwQOyeHswCM) - OVIS UI
- [Belajar Cyber Security](https://youtu.be/E3IC32iErwU) - Web Programming UNPAS ft Doddy Ferdiansyah
- [Hacking - Haram vs Halal](https://youtu.be/xpISUxyMiOY) - ECHO|TALK 

## Cyber Security Career Roadmap
- [Cybersecurity Career Path](https://github.com/rezaduty/cybersecurity-career-path) - Rezaduty

------

## Cyber Security Awareness
- [Mengenal Kejahatan Cyber dan Upaya Pencegah di Era New-Normal](https://youtu.be/KiSBI2YJeVk?t=5137) - M.Khabiburrohman 
- [How Do Hackers Works - Live Hacking Demo](https://youtu.be/7LengaQm4XU?t=5558) - Mukhammad Khabiburrohman 
- [Kenali Potensi Bahaya Cyber dan Cara Proteksinya](https://youtu.be/KiSBI2YJeVk?t=2459)- Edy Subowo, M.Kom 
- [Security Awareness: Story From The Dark Side](https://youtu.be/6Y1JDbf0YcQ) - [Blue Team Indonesia](https://blueteam.id/)
- [Bentuk Ancaman Dan Kerentan Cyber Security](https://youtu.be/c-N-jgwgWdQ) - OVIS UI
- [Bersosial Media Dengan Aman](https://www.youtube.com/watch?v=IaJoKjCgvYo) - OVIS UI
- [Webcam Laptop & Kamera Ponsel Bisa Diretas](https://www.youtube.com/watch?v=BRHJ5W41pIo) - OVIS UI
- [Rekomendasi Antivirus & Antisipasi](https://www.youtube.com/watch?v=Tb16MWBxdD4) - OVIS UI
- [Mengidentifikasi Website/Aplikasi Berbahaya](https://www.youtube.com/watch?v=uD3PyA37d7E) - OVIS UI
- [Cyber Ssecurity di Era Teknologi Informasi](https://www.youtube.com/watch?v=lFBQmoqvOJM) - CeLOE Telkom University
- [Cyber Security Awareness Internet Safety](https://youtu.be/lv2UeicNMMA) - MASTEL TV

------

## Peluang Project & Perjelanan Karir di Cyber Security
- [Membangun Jalur Karir Di Cyber Security](https://youtu.be/Gh6Mz2wuMuM?t=706) - Dr. Toto Atmojo 
- [How Can I Become A Penetration Tester](https://youtu.be/Gh6Mz2wuMuM?t=3097) - Thomas Gregory 
- [Cybersecurity Threats, Challenges, Opportunites](https://youtu.be/Gh6Mz2wuMuM?t=5212) - Semi Yulianto 
- [Menjadi Cyber Security Defendor - Wawancara Exclusive](https://youtu.be/0efIcVpxX2E) - Digit Oktavianto
- [Nusantech Webinar - Berkarir di Bidang Cyber Security](https://www.youtube.com/watch?v=FkPTFYqGjR8&t=3458s) - Satria Ady Pradana 
- [Karir di bidang Cybersecurity](https://www.youtube.com/watch?v=KQ8Cv5OnkBA) - Budi Raharjo Channel

------

## Web Application Hacking/Security
- [Pengenalan Web Application Security](https://www.youtube.com/watch?v=Mz3u2v-Y5pU) - Surabaya Hacker Link
- [Buku Web Application Security Indonesia](https://www.youtube.com/watch?v=c-cO8Cr6HIs) - Semi Yulianto

### Local File Inclusion

- [Web - PHP Local File inclusion (LFI)](https://www.youtube.com/watch?v=h-2UrETGKFg) - Cyber Security IPB	
- [Pengenalan Local File Inclusion](https://www.youtube.com/watch?v=CSx3zqgX2BI) - Ethical Hacking Indonesia
- [Local File Inclusion Vulnerability (LFI) dalam PHP [Bagian 1]](https://www.youtube.com/watch?v=i0uWUy4oMRI) - Bimo Sukarno
- [Local File Inclusion Vulnerability (LFI) dalam PHP [Bagian 2]](https://www.youtube.com/watch?v=H80SgoP8Kl0) - Bimo Sukarno
- [Local File Inclusion Vulnerability (LFI) dalam PHP LFI to RCE [Bagian 3]](https://www.youtube.com/watch?v=5U8r5it_9Yw) - Bimo Sukarno
- [Local File Inclusion and File Upload](https://www.youtube.com/watch?v=qqarbngfrNk) - Nikko Enggaliano
- [Local File Inclusion - Basic](https://www.youtube.com/watch?v=0HOiwQhlpZQ) - Surabaya Hacker Link
- [Upload Shell LFI/RFI - PHP Expect Wrapper](https://www.youtube.com/watch?v=MI0cpDMfrMU) - Indosec
 
### Open Redirect
- [Sekilas Open Redirect dan Cara Kerja](https://youtu.be/lHdfeY4RB3E?t=578) - Pondok Daring Siber 

### Cross-Site Request Forgery (CSRF)
- [Mengenal Lebih dalam tentang Serangan CSRF](https://youtu.be/nED23ARZvwQ) - Surabaya Hacker Link
- [Tutorial dan Simulasi CSRF Attack di CodeIgniter](https://youtu.be/9JH22oAiB_8) - SUSANTOKUN
- [Demo Cross-site Request Forgery (Bahasa Indonesia) (CSRF/XSRF)](https://www.youtube.com/watch?v=uI2Y08Fzl-M) - Kemal Elmizan
- [Mengenal Tentang CSRF (Web Security)](https://www.youtube.com/watch?v=IA4CVROQ1-U) - IndoSEC

### Cross-Site Scripting (XSS) 
- [Web Security - Konsep XSS (Cross Site Scripting)](https://www.youtube.com/watch?v=RkTrT437MP0) - Cyber Security IPB
- [Mengenal Lebih Dalam XSS (Cross-site Scripting)](https://www.youtube.com/watch?v=v6WVZHAB_gQ) - Surabaya Hacker Link
- [Tips Hunting mencari XSS (Cross-site Scripting)](https://youtu.be/caSQisDxboE) - Rando Channel
- [Pengenalan Tools XSStrike Untuk Mencari Bug XSS](https://www.youtube.com/watch?v=NBCI5pAVEUQ) - Ethical Hacking Indonesia
- [DVWA - Serangan Cross-Site Scripting (XSS) Reflected, Stored & DOM + Solusi](https://www.youtube.com/watch?v=ElTBEOMGwPc) - Ngoding Coding
- [Mencuri Cookies Menggunakan Serangan Cross Site Scripting Stored (XSS Stored)](https://www.youtube.com/watch?v=ibnVWCCtsHU) - Ayz Channel
- [Mengidentifikasi serangan XSS](https://youtu.be/Dy6_QVxgkUo?t=1336) -  Ando Rumampuk on Orang Siber Channel

### Insecure Direct Object References (IDOR)
- [Sekilas IDOR dan Cara Kerja](https://youtu.be/lHdfeY4RB3E?t=1634) - Pondok Daring Siber
- [Demo Serangan Dasar IDOR Menggunakan Burpsuite](https://youtu.be/lHdfeY4RB3E?t=3678) - Pondok Daring Siber

### SQL Injection
- [Web - SQL injection dasar](https://youtu.be/qbwhbfdVg3E?list=PLn8rJDl0kSc4-o1ewkJ4VtKF-_0RQKJoN) - Cyber Security IPB	 
- [Web - SQL injection teknik UNION](https://youtu.be/XDyOVns8gXg?list=PLn8rJDl0kSc4-o1ewkJ4VtKF-_0RQKJoN) - Cyber Security IPB	
- [Web - Blind SQL injection](https://youtu.be/DNhJw1b1q58?list=PLn8rJDl0kSc4-o1ewkJ4VtKF-_0RQKJoN) - Cyber Security IPB	
- [Web - Blind SQL injection berbasis waktu (time-based)](https://youtu.be/9FOa0tPNqMk?list=PLn8rJDl0kSc4-o1ewkJ4VtKF-_0RQKJo) - Cyber Security IPB	
- [SQL injection pada proses INSERT](https://youtu.be/RSg5OeU6QGM?list=PLn8rJDl0kSc4-o1ewkJ4VtKF-_0RQKJoN) - Cyber Security IPB	
- [SQL Injection Bypass Login](https://youtu.be/orRnaHyFcEg) - Surabaya Hacker Links
- [SQL Injection - Pentest Case Study for Beginners (in Bahasa Indonesia)](https://youtu.be/URkCKbZNlnA) - Semi Yulianto
- [SQL Injection - Yet Another Pentest Case Study (in Bahasa Indonesia)](https://youtu.be/uW86ikKTRqg) - Semi Yulianto

------
# Red Team
Tim merah adalah sebuah grup yang berperan sebagai musuh atau pesaing untuk memberikan umpan balik keamanan dari perspektif itu. Tim merah digunakan di banyak bidang, terutama dalam keamanan siber, keamanan bandara, militer, dan badan intelijen. 
(ref//https://en.wikipedia.org/wiki/Red_team)

## Initial Access
- [The Hitchhiker’s Guide To Initial Access](https://posts.specterops.io/the-hitchhikers-guide-to-initial-access-57b66aa80dd6)
- [How To: Empire’s Cross Platform Office Macro](https://www.blackhillsinfosec.com/empires-cross-platform-office-macro/)
- [The Hitchhiker’s Guide To Initial Access](https://posts.specterops.io/the-hitchhikers-guide-to-initial-access-57b66aa80dd6)
- [How To: Empire’s Cross Platform Office Macro](https://www.blackhillsinfosec.com/empires-cross-platform-office-macro/)
- [Phishing with PowerPoint](https://www.blackhillsinfosec.com/phishing-with-powerpoint/)
- [PHISHING WITH EMPIRE](https://enigma0x3.net/2016/03/15/phishing-with-empire/)
- [Bash Bunny](https://hakshop.com/products/bash-bunny)
- [OWASP Presentation of Social Engineering - OWASP](https://owasp.org/www-pdf-archive/Presentation_Social_Engineering.pdf)
- [USB Drop Attacks: The Danger of “Lost And Found” Thumb Drives](https://www.redteamsecure.com/usb-drop-attacks-the-danger-of-lost-and-found-thumb-drives/)
- [Weaponizing data science for social engineering: Automated E2E spear phishing on Twitter - Defcon 24](https://media.defcon.org/DEF%20CON%2024/DEF%20CON%2024%20presentations/DEF%20CON%2024%20-%20Seymour-Tully-Weaponizing-Data-Science-For-Social-Engineering-WP.pdf)
- [Cobalt Strike - Spear Phishing documentation](https://www.cobaltstrike.com/help-spear-phish)
- [Cobalt Strike Blog - What's the go-to phishing technique or exploit?](https://blog.cobaltstrike.com/2014/12/17/whats-the-go-to-phishing-technique-or-exploit/)
- [Spear phishing with Cobalt Strike - Raphael Mudge](https://www.youtube.com/watch?v=V7UJjVcq2Ao)
- [EMAIL RECONNAISSANCE AND PHISHING TEMPLATE GENERATION MADE SIMPLE](https://cybersyndicates.com/2016/05/email-reconnaissance-phishing-template-generation-made-simple/)
- [Phishing for access](http://www.rvrsh3ll.net/blog/phishing/phishing-for-access/)
- [Excel macros with PowerShell](https://4sysops.com/archives/excel-macros-with-powershell/)
- [PowerPoint and Custom Actions](https://phishme.com/powerpoint-and-custom-actions/)
- [Macro-less Code Exec in MSWord](https://sensepost.com/blog/2017/macro-less-code-exec-in-msword/)
- [Multi-Platform Macro Phishing Payloads](https://medium.com/@malcomvetter/multi-platform-macro-phishing-payloads-3b688e8eff68)
- [Abusing Microsoft Word Features for Phishing: “subDoc”](https://rhinosecuritylabs.com/research/abusing-microsoft-word-features-phishing-subdoc/)
- [Phishing Against Protected View](https://enigma0x3.net/2017/07/13/phishing-against-protected-view/)
- [POWERSHELL EMPIRE STAGERS 1: PHISHING WITH AN OFFICE MACRO AND EVADING AVS](https://fzuckerman.wordpress.com/2016/10/06/powershell-empire-stagers-1-phishing-with-an-office-macro-and-evading-avs/)
- [The PlugBot: Hardware Botnet Research Project](https://www.redteamsecure.com/the-plugbot-hardware-botnet-research-project/)
- [Luckystrike: An Evil Office Document Generator](https://www.shellntel.com/blog/2016/9/13/luckystrike-a-database-backed-evil-macro-generator)
- [The Absurdly Underestimated Dangers of CSV Injection](http://georgemauer.net/2017/10/07/csv-injection.html)
- [Macroless DOC malware that avoids detection with Yara rule](https://furoner.wordpress.com/2017/10/17/macroless-malware-that-avoids-detection-with-yara-rule/amp/)
- [Phishing between the app whitelists](https://medium.com/@vivami/phishing-between-the-app-whitelists-1b7dcdab4279)
- [Executing Metasploit & Empire Payloads from MS Office Document Properties (part 1 of 2)](https://stealingthe.network/executing-metasploit-empire-payloads-from-ms-office-document-properties-part-1-of-2/)
- [Executing Metasploit & Empire Payloads from MS Office Document Properties (part 2 of 2)](https://stealingthe.network/executing-metasploit-empire-payloads-from-ms-office-document-properties-part-2-of-2/)
- [Social Engineer Portal](https://www.social-engineer.org/)
- [7 Best social Engineering attack](http://www.darkreading.com/the-7-best-social-engineering-attacks-ever/d/d-id/1319411)
- [Using Social Engineering Tactics For Big Data Espionage - RSA Conference Europe 2012](https://www.rsaconference.com/writable/presentations/file_upload/das-301_williams_rader.pdf)
- [USING THE DDE ATTACK WITH POWERSHELL EMPIRE](https://1337red.wordpress.com/using-the-dde-attack-with-powershell-empire/)
- [Phishing on Twitter - POT](https://www.kitploit.com/2018/02/pot-phishing-on-twitter.html)
- [Microsoft Office – NTLM Hashes via Frameset](https://pentestlab.blog/2017/12/18/microsoft-office-ntlm-hashes-via-frameset/)
- [Defense-In-Depth write-up](https://oddvar.moe/2017/09/13/defense-in-depth-writeup/)
- [Spear Phishing 101](https://blog.inspired-sec.com/archive/2017/05/07/Phishing.html)

## Execution 
- [Research on CMSTP.exe,](https://msitpros.com/?p=3960)
- [Windows oneliners to download remote payload and execute arbitrary code](https://arno0x0x.wordpress.com/2017/11/20/windows-oneliners-to-download-remote-payload-and-execute-arbitrary-code/)
- [Executing Commands and Bypassing AppLocker with PowerShell Diagnostic Scripts](https://bohops.com/2017/12/02/clickonce-twice-or-thrice-a-technique-for-social-engineering-and-untrusted-command-execution/)
- [WSH Injection: A Case Study](https://posts.specterops.io/wsh-injection-a-case-study-fd35f79d29dd)
- [Gscript Dropper](http://lockboxx.blogspot.com/2018/02/intro-to-using-gscript-for-red-teams.html)

## Persistence
- [A View of Persistence](https://rastamouse.me/blog/view-of-persistence/)
- [hiding registry keys with psreflect](https://posts.specterops.io/hiding-registry-keys-with-psreflect-b18ec5ac8353)
- [Persistence using RunOnceEx – Hidden from Autoruns.exe](https://oddvar.moe/2018/03/21/persistence-using-runonceex-hidden-from-autoruns-exe/)
- [Persistence using GlobalFlags in Image File Execution Options – Hidden from Autoruns.exe](https://oddvar.moe/2018/04/10/persistence-using-globalflags-in-image-file-execution-options-hidden-from-autoruns-exe/)
- [Putting data in Alternate data streams and how to execute it – part 2](https://oddvar.moe/2018/04/11/putting-data-in-alternate-data-streams-and-how-to-execute-it-part-2/)
- [WMI Persistence with Cobalt Strike](https://blog.inspired-sec.com/archive/2017/01/20/WMI-Persistence.html)
- [Leveraging INF-SCT Fetch & Execute Techniques For Bypass, Evasion, & Persistence](https://bohops.com/2018/02/26/leveraging-inf-sct-fetch-execute-techniques-for-bypass-evasion-persistence/)
- [Leveraging INF-SCT Fetch & Execute Techniques For Bypass, Evasion, & Persistence (Part 2)](https://bohops.com/2018/03/10/leveraging-inf-sct-fetch-execute-techniques-for-bypass-evasion-persistence-part-2/)
- [Vshadow: Abusing the Volume Shadow Service for Evasion, Persistence, and Active Directory Database Extraction](https://bohops.com/2018/02/10/vshadow-abusing-the-volume-shadow-service-for-evasion-persistence-and-active-directory-database-extraction/)

## Privilege Escalation
- [First entry: Welcome and fileless UAC bypass,](https://winscripting.blog/2017/05/12/first-entry-welcome-and-uac-bypass/)
- [Exploiting Environment Variables in Scheduled Tasks for UAC Bypass,](https://tyranidslair.blogspot.ru/2017/05/exploiting-environment-variables-in.html)
- Reading Your Way Around UAC in 3 parts:
   [Part 1.](https://tyranidslair.blogspot.ru/2017/05/reading-your-way-around-uac-part-1.html)
   [Part 2.](https://tyranidslair.blogspot.ru/2017/05/reading-your-way-around-uac-part-2.html)
   [Part 3.](https://tyranidslair.blogspot.ru/2017/05/reading-your-way-around-uac-part-3.html)
- [Bypassing UAC using App Paths,](https://enigma0x3.net/2017/03/14/bypassing-uac-using-app-paths/)
- ["Fileless" UAC Bypass using sdclt.exe,](https://enigma0x3.net/2017/03/17/fileless-uac-bypass-using-sdclt-exe/)
- [UAC Bypass or story about three escalations,](https://habrahabr.ru/company/pm/blog/328008/)
- ["Fileless" UAC Bypass Using eventvwr.exe and Registry Hijacking,](https://enigma0x3.net/2016/08/15/fileless-uac-bypass-using-eventvwr-exe-and-registry-hijacking/)
- [Bypassing UAC on Windows 10 using Disk Cleanup,](https://enigma0x3.net/2016/07/22/bypassing-uac-on-windows-10-using-disk-cleanup/)
- [Using IARPUninstallStringLauncher COM interface to bypass UAC,](http://www.freebuf.com/articles/system/116611.html)
- [Fileless UAC Bypass using sdclt](https://posts.specterops.io/fileless-uac-bypass-using-sdclt-exe-3e9f9ad4e2b3)
- [Eventvwr File-less UAC Bypass CNA](https://www.mdsec.co.uk/2016/12/cna-eventvwr-uac-bypass/)
- [Windows 7 UAC whitelist](http://www.pretentiousname.com/misc/win7_uac_whitelist2.html)


## Escalation
- [Windows Privilege Escalation Checklist](https://github.com/netbiosX/Checklists/blob/master/Windows-Privilege-Escalation.md)
- [From Patch Tuesday to DA](https://blog.inspired-sec.com/archive/2017/03/17/COM-Moniker-Privesc.html)
- [A Path for Privilege Escalation](https://blog.cobaltstrike.com/2016/12/08/cobalt-strike-3-6-a-path-for-privilege-escalation/)

## Defense Evasion
- [Window 10 Device Guard Bypass](https://github.com/tyranid/DeviceGuardBypasses)
- [App Locker ByPass List](https://github.com/api0cradle/UltimateAppLockerByPassList)
- [Window Signed Binary](https://github.com/vysec/Windows-SignedBinary)
- [Bypass Application Whitelisting Script Protections - Regsvr32.exe & COM Scriptlets (.sct files)](http://subt0x10.blogspot.sg/2017/04/bypass-application-whitelisting-script.html)
- [Bypassing Application Whitelisting using MSBuild.exe - Device Guard Example and Mitigations](http://subt0x10.blogspot.sg/2017/04/bypassing-application-whitelisting.html)
- [Empire without powershell](https://bneg.io/2017/07/26/empire-without-powershell-exe/)
- [Powershell without Powershell to bypass app whitelist](https://www.blackhillsinfosec.com/powershell-without-powershell-how-to-bypass-application-whitelisting-environment-restrictions-av/)
- [MS Signed mimikatz in just 3 steps](https://github.com/secretsquirrel/SigThief)
- [Hiding your process from sysinternals](https://riscybusiness.wordpress.com/2017/10/07/hiding-your-process-from-sysinternals/)
- [code signing certificate cloning attacks and defenses](https://posts.specterops.io/code-signing-certificate-cloning-attacks-and-defenses-6f98657fc6ec)
- [userland api monitoring and code injection detection](https://0x00sec.org/t/userland-api-monitoring-and-code-injection-detection/5565)
- [In memory evasion](https://blog.cobaltstrike.com/2018/02/08/in-memory-evasion/)
- [Bypassing AMSI via COM Server Hijacking](https://posts.specterops.io/bypassing-amsi-via-com-server-hijacking-b8a3354d1aff)
- [process doppelganging](https://hshrzd.wordpress.com/2017/12/18/process-doppelganging-a-new-way-to-impersonate-a-process/)
- [Week of Evading Microsoft ATA - Announcement and Day 1 to Day 5](http://www.labofapenetrationtester.com/2017/08/week-of-evading-microsoft-ata-day1.html)
- [VEIL-EVASION AES ENCRYPTED HTTPKEY REQUEST: SAND-BOX EVASION](https://cybersyndicates.com/2015/06/veil-evasion-aes-encrypted-httpkey-request-module/)
- [Putting data in Alternate data streams and how to execute it](https://oddvar.moe/2018/01/14/putting-data-in-alternate-data-streams-and-how-to-execute-it/)
- [AppLocker – Case study – How insecure is it really? – Part 1](https://oddvar.moe/2017/12/13/applocker-case-study-how-insecure-is-it-really-part-1/)
- [AppLocker – Case study – How insecure is it really? – Part 2](https://oddvar.moe/2017/12/21/applocker-case-study-how-insecure-is-it-really-part-2/)
- [Harden Windows with AppLocker – based on Case study part 2](https://oddvar.moe/2017/12/13/harden-windows-with-applocker-based-on-case-study-part-1/)
- [Harden Windows with AppLocker – based on Case study part 2](https://oddvar.moe/2017/12/21/harden-windows-with-applocker-based-on-case-study-part-2/)
- [Office 365 Safe links bypass](https://oddvar.moe/2018/01/03/office-365-safe-links-bypass/)
- [Windows Defender Attack Surface Reduction Rules bypass](https://oddvar.moe/2018/03/15/windows-defender-attack-surface-reduction-rules-bypass/)
- [Bypassing Device guard UMCI using CHM – CVE-2017-8625](https://oddvar.moe/2017/08/13/bypassing-device-guard-umci-using-chm-cve-2017-8625/)
- [Bypassing Application Whitelisting with BGInfo](https://oddvar.moe/2017/05/18/bypassing-application-whitelisting-with-bginfo/)
- [Cloning and Hosting Evil Captive Portals using a Wifi PineApple](https://blog.inspired-sec.com/archive/2017/01/10/cloning-captive-portals.html)
- [https://bohops.com/2018/01/23/loading-alternate-data-stream-ads-dll-cpl-binaries-to-bypass-applocker/](https://bohops.com/2018/01/23/loading-alternate-data-stream-ads-dll-cpl-binaries-to-bypass-applocker/)
- [Executing Commands and Bypassing AppLocker with PowerShell Diagnostic Scripts](https://bohops.com/2018/01/07/executing-commands-and-bypassing-applocker-with-powershell-diagnostic-scripts/)
- [mavinject.exe Functionality Deconstructed](https://posts.specterops.io/mavinject-exe-functionality-deconstructed-c29ab2cf5c0e)

## Credential Access
- [Windows Access Tokens and Alternate credentials](https://blog.cobaltstrike.com/2015/12/16/windows-access-tokens-and-alternate-credentials/)
- [Bringing the hashes home with reGeorg & Empire](https://sensepost.com/blog/2016/bringing-the-hashes-home-with-regeorg-empire/)
- [Intercepting passwords with Empire and winning](https://sensepost.com/blog/2016/intercepting-passwords-with-empire-and-winning/)
- [Local Administrator Password Solution (LAPS) Part 1](https://rastamouse.me/blog/laps-pt1/)
- [Local Administrator Password Solution (LAPS) Part 2](https://rastamouse.me/blog/laps-pt2/)
- [USING A SCF FILE TO GATHER HASHES](https://1337red.wordpress.com/using-a-scf-file-to-gather-hashes/)
- [Remote Hash Extraction On Demand Via Host Security Descriptor Modification](https://www.harmj0y.net/blog/)
- [Offensive Encrypted Data Storage](https://www.harmj0y.net/blog/redteaming/offensive-encrypted-data-storage/)
- [Practical guide to NTLM Relaying](https://byt3bl33d3r.github.io/practical-guide-to-ntlm-relaying-in-2017-aka-getting-a-foothold-in-under-5-minutes.html)
- [Dump Clear-Text Passwords for All Admins in the Domain Using Mimikatz DCSync](https://adsecurity.org/?p=2053)
- [Dumping Domain Password Hashes](https://pentestlab.blog/2018/07/04/dumping-domain-password-hashes/)
  
## Discovery
- [Red Team Operating in a Modern Environment](https://www.owasp.org/images/4/4b/Red_Team_Operating_in_a_Modern_Environment.pdf)
- [My First Go with BloodHound](https://blog.cobaltstrike.com/2016/12/14/my-first-go-with-bloodhound/)
- [Introducing BloodHound](https://wald0.com/?p=68)
- [A Red Teamer’s Guide to GPOs and OUs](https://wald0.com/?p=179)
- [Automated Derivative Administrator Search](https://wald0.com/?p=14)
- [A Pentester’s Guide to Group Scoping](https://www.harmj0y.net/blog/activedirectory/a-pentesters-guide-to-group-scoping/)
- [Local Group Enumeration](https://www.harmj0y.net/blog/redteaming/local-group-enumeration/)
- [The PowerView PowerUsage Series #1 - Mass User Profile Enumeration](http://www.harmj0y.net/blog/powershell/the-powerview-powerusage-series-1/)
- [The PowerView PowerUsage Series #2 – Mapping Computer Shortnames With the Global Catalog](http://www.harmj0y.net/blog/powershell/the-powerview-powerusage-series-2/)
- [The PowerView PowerUsage Series #3 – Enumerating GPO edit rights in a foreign domain](http://www.harmj0y.net/blog/powershell/the-powerview-powerusage-series-3/)
- [The PowerView PowerUsage Series #4 – Finding cross-trust ACEs](http://www.harmj0y.net/blog/powershell/the-powerview-powerusage-series-3/)
- [Aggressor PowerView](http://threat.tevora.com/aggressor-powerview/)
- [Lay of the Land with BloodHound](http://threat.tevora.com/lay-of-the-land-with-bloodhound/)
- [Scanning for Active Directory Privileges & Privileged Accounts](https://adsecurity.org/?p=3658)
- [Microsoft LAPS Security & Active Directory LAPS Configuration Recon](https://adsecurity.org/?p=3164)
- [Trust Direction: An Enabler for Active Directory Enumeration and Trust Exploitation](https://bohops.com/2017/12/02/trust-direction-an-enabler-for-active-directory-enumeration-and-trust-exploitation/)
- [SPN Discovery](https://pentestlab.blog/2018/06/04/spn-discovery/)
   
## Lateral Movement 

- [A Citrix Story](https://rastamouse.me/blog/a-citrix-story/)
- [Jumping Network Segregation with RDP](https://rastamouse.me/blog/rdp-jump-boxes/)
- [Pass hash pass ticket no pain](http://resources.infosecinstitute.com/pass-hash-pass-ticket-no-pain/)
- [Abusing DNSAdmins privilege for escalation in Active Directory](http://www.labofapenetrationtester.com/2017/05/abusing-dnsadmins-privilege-for-escalation-in-active-directory.html)
- [Using SQL Server for attacking a Forest Trust](http://www.labofapenetrationtester.com/2017/03/using-sql-server-for-attacking-forest-trust.html)
- [Extending BloodHound for Red Teamers](https://www.youtube.com/watch?v=Pn7GWRXfgeI)
- [OPSEC Considerations for beacon commands](https://blog.cobaltstrike.com/2017/06/23/opsec-considerations-for-beacon-commands/)
- [My First Go with BloodHound](https://blog.cobaltstrike.com/2016/12/14/my-first-go-with-bloodhound/)
- [Kerberos Party Tricks: Weaponizing Kerberos Protocol Flaws](http://www.exumbraops.com/blog/2016/6/1/kerberos-party-tricks-weaponizing-kerberos-protocol-flaws)
- [Lateral movement using excel application and dcom](https://enigma0x3.net/2017/09/11/lateral-movement-using-excel-application-and-dcom/)
- [Lay of the Land with BloodHound](http://threat.tevora.com/lay-of-the-land-with-bloodhound/)
- [The Most Dangerous User Right You (Probably) Have Never Heard Of](https://www.harmj0y.net/blog/activedirectory/the-most-dangerous-user-right-you-probably-have-never-heard-of/)
- [Agentless Post Exploitation](https://blog.cobaltstrike.com/2016/11/03/agentless-post-exploitation/)
- [A Guide to Attacking Domain Trusts](https://www.harmj0y.net/blog/redteaming/a-guide-to-attacking-domain-trusts/)   
- [Pass-the-Hash Is Dead: Long Live LocalAccountTokenFilterPolicy](https://www.harmj0y.net/blog/redteaming/pass-the-hash-is-dead-long-live-localaccounttokenfilterpolicy/)
- [Targeted Kerberoasting](https://www.harmj0y.net/blog/activedirectory/targeted-kerberoasting/)
- [Kerberoasting Without Mimikatz](https://www.harmj0y.net/blog/powershell/kerberoasting-without-mimikatz/)
- [Abusing GPO Permissions](https://www.harmj0y.net/blog/redteaming/abusing-gpo-permissions/)
- [Abusing Active Directory Permissions with PowerView](https://www.harmj0y.net/blog/redteaming/abusing-active-directory-permissions-with-powerview/)
- [Roasting AS-REPs](https://www.harmj0y.net/blog/activedirectory/roasting-as-reps/)
- [Getting the goods with CrackMapExec: Part 1](https://byt3bl33d3r.github.io/getting-the-goods-with-crackmapexec-part-1.html)
- [Getting the goods with CrackMapExec: Part 2](https://byt3bl33d3r.github.io/getting-the-goods-with-crackmapexec-part-2.html)
- [DiskShadow: The Return of VSS Evasion, Persistence, and Active Directory Database Extraction](https://bohops.com/2018/03/26/diskshadow-the-return-of-vss-evasion-persistence-and-active-directory-database-extraction/)
- [Abusing Exported Functions and Exposed DCOM Interfaces for Pass-Thru Command Execution and Lateral Movement](https://bohops.com/2018/03/17/abusing-exported-functions-and-exposed-dcom-interfaces-for-pass-thru-command-execution-and-lateral-movement/)
- [a guide to attacking domain trusts](https://posts.specterops.io/a-guide-to-attacking-domain-trusts-971e52cb2944)
- [Outlook Home Page – Another Ruler Vector](https://sensepost.com/blog/2017/outlook-home-page-another-ruler-vector/)
- [Outlook Forms and Shells](https://sensepost.com/blog/2017/outlook-forms-and-shells/)
- [Abusing the COM Registry Structure: CLSID, LocalServer32, & InprocServer32](https://bohops.com/2018/06/28/abusing-com-registry-structure-clsid-localserver32-inprocserver32/)
- [LethalHTA - A new lateral movement technique using DCOM and HTA](https://codewhitesec.blogspot.com/2018/07/lethalhta.html)
- [Abusing DCOM For Yet Another Lateral Movement Technique](https://bohops.com/2018/04/28/abusing-dcom-for-yet-another-lateral-movement-technique/)
   
##  Collection  
- [Accessing clipboard from the lock screen in Windows 10 Part 1](https://oddvar.moe/2017/01/24/accessing-clipboard-from-the-lock-screen-in-windows-10/)
- [Accessing clipboard from the lock screen in Windows 10 Part 2](https://oddvar.moe/2017/01/27/access-clipboard-from-lock-screen-in-windows-10-2/)

  
   
##  Exfiltration
- [DNS Data exfiltration — What is this and How to use?](https://blog.fosec.vn/dns-data-exfiltration-what-is-this-and-how-to-use-2f6c69998822)
- [DNS Tunnelling](http://resources.infosecinstitute.com/dns-tunnelling/)
- [sg1: swiss army knife for data encryption, exfiltration & covert communication](https://securityonline.info/sg1-swiss-army-knife-for-data-encryption-exfiltration-covert-communication/?utm_source=ReviveOldPost&utm_medium=social&utm_campaign=ReviveOldPost)
- [Data Exfiltration over DNS Request Covert Channel: DNSExfiltrator](https://n0where.net/data-exfiltration-over-dns-request-covert-channel-dnsexfiltrator)
- [DET (extensible) Data Exfiltration Toolkit](https://github.com/PaulSec/DET)
- [Data Exfiltration via Formula Injection Part1](https://www.notsosecure.com/data-exfiltration-formula-injection/)


##  Command and Control

### Domain Fronting
- [Empre Domain Fronting](https://www.xorrior.com/Empire-Domain-Fronting/)
- [Escape and Evasion Egressing Restricted Networks - Tom Steele and Chris Patten](https://www.optiv.com/blog/escape-and-evasion-egressing-restricted-networks)
- [Finding Frontable Domain](https://github.com/rvrsh3ll/FindFrontableDomains)
- [TOR Fronting – Utilising Hidden Services for Privacy](https://www.mdsec.co.uk/2017/02/tor-fronting-utilising-hidden-services-for-privacy/)
- [Simple domain fronting PoC with GAE C2 server](https://www.securityartwork.es/2017/01/31/simple-domain-fronting-poc-with-gae-c2-server/)
- [Domain Fronting Via Cloudfront Alternate Domains](https://www.mdsec.co.uk/2017/02/domain-fronting-via-cloudfront-alternate-domains/)
- [Finding Domain frontable Azure domains - thoth / Fionnbharr (@a_profligate)](https://theobsidiantower.com/2017/07/24/d0a7cfceedc42bdf3a36f2926bd52863ef28befc.html)
- [Google Groups: Blog post on finding 2000+ Azure domains using Censys](https://groups.google.com/forum/#!topic/traffic-obf/7ygIXCPebwQ)
- [Red Team Insights on HTTPS Domain Fronting Google Hosts Using Cobalt Strike](https://www.cyberark.com/threat-research-blog/red-team-insights-https-domain-fronting-google-hosts-using-cobalt-strike/)
- [SSL Domain Fronting 101](http://www.rvrsh3ll.net/blog/offensive/ssl-domain-fronting-101/)
- [How I Identified 93k Domain-Frontable CloudFront Domains](https://www.peew.pw/blog/2018/2/22/how-i-identified-93k-domain-frontable-cloudfront-domains)
- [Validated CloudFront SSL Domains](https://medium.com/@vysec.private/validated-cloudfront-ssl-domains-27895822cea3)
- [CloudFront Hijacking](https://www.mindpointgroup.com/blog/pen-test/cloudfront-hijacking/)
- [CloudFrunt GitHub Repo](https://github.com/MindPointGroup/cloudfrunt)

### Connection Proxy
- [Redirecting Cobalt Strike DNS Beacons](http://www.rvrsh3ll.net/blog/offensive/redirecting-cobalt-strike-dns-beacons/)
- [Apache2Mod Rewrite Setup](https://github.com/n0pe-sled/Apache2-Mod-Rewrite-Setup)
- [Cobalt Strike HTTP C2 Redirectors with Apache mod_rewrite](https://bluescreenofjeff.com/2016-06-28-cobalt-strike-http-c2-redirectors-with-apache-mod_rewrite/)
- [High-reputation Redirectors and Domain Fronting](https://blog.cobaltstrike.com/2017/02/06/high-reputation-redirectors-and-domain-fronting/)
- [Cloud-based Redirectors for Distributed Hacking](https://blog.cobaltstrike.com/2014/01/14/cloud-based-redirectors-for-distributed-hacking/)
- [Combatting Incident Responders with Apache mod_rewrite](https://bluescreenofjeff.com/2016-04-12-combatting-incident-responders-with-apache-mod_rewrite/)
- [Operating System Based Redirection with Apache mod_rewrite](https://bluescreenofjeff.com/2016-04-05-operating-system-based-redirection-with-apache-mod_rewrite/)
- [Invalid URI Redirection with Apache mod_rewrite](https://bluescreenofjeff.com/2016-03-29-invalid-uri-redirection-with-apache-mod_rewrite/)
- [Strengthen Your Phishing with Apache mod_rewrite and Mobile User Redirection](https://bluescreenofjeff.com/2016-03-22-strengthen-your-phishing-with-apache-mod_rewrite-and-mobile-user-redirection/)
- [mod_rewrite rule to evade vendor sandboxes](https://gist.github.com/curi0usJack/971385e8334e189d93a6cb4671238b10)
- [Expire Phishing Links with Apache RewriteMap](https://bluescreenofjeff.com/2016-04-19-expire-phishing-links-with-apache-rewritemap/)
- [Serving random payloads with NGINX](https://gist.github.com/jivoi/a33ace2e25515a31aa2ffbae246d98c9)
- [Mod_Rewrite Automatic Setup](https://blog.inspired-sec.com/archive/2017/04/17/Mod-Rewrite-Automatic-Setup.html)
- [Hybrid Cobalt Strike Redirectors](https://zachgrace.com/2018/02/20/cobalt_strike_redirectors.html)
- [Expand Your Horizon Red Team – Modern SAAS C2](https://cybersyndicates.com/2017/04/expand-your-horizon-red-team/)
- [RTOps: Automating Redirector Deployment With Ansible](http://threat.tevora.com/automating-redirector-deployment-with-ansible/)

### Web Services
- [C2 with Dropbox](https://pentestlab.blog/2017/08/29/command-and-control-dropbox/)
- [C2 with gmail](https://pentestlab.blog/2017/08/03/command-and-control-gmail/)
- [C2 with twitter](https://pentestlab.blog/2017/09/26/command-and-control-twitter/)
- [Office 365 for Cobalt Strike C2](https://labs.mwrinfosecurity.com/blog/tasking-office-365-for-cobalt-strike-c2/)
- [Red Team Insights on HTTPS Domain Fronting Google Hosts Using Cobalt Strike](https://www.cyberark.com/threat-research-blog/red-team-insights-https-domain-fronting-google-hosts-using-cobalt-strike/)
- [A stealthy Python based Windows backdoor that uses Github as a C&C server](http://securityblog.gr/4434/a-stealthy-python-based-windows-backdoor-that-uses-github-as-a-cc-server/)
- [External C2 (Third-Party Command and Control)](https://www.cobaltstrike.com/help-externalc2)
- [Cobalt Strike over external C2 – beacon home in the most obscure ways](https://outflank.nl/blog/2017/09/17/blogpost-cobalt-strike-over-external-c2-beacon-home-in-the-most-obscure-ways/)
- [External C2 for Cobalt Strike](https://github.com/ryhanson/ExternalC2/)
- [External C2 framework for Cobalt Strike](http://www.insomniacsecurity.com/2018/01/11/externalc2.html)
- [External C2 framework - GitHub Repo](https://github.com/Und3rf10w/external_c2_framework)
- [Hiding in the Cloud: Cobalt Strike Beacon C2 using Amazon APIs](https://github.com/Und3rf10w/external_c2_framework)
- [Exploring Cobalt Strike's ExternalC2 framework](https://blog.xpnsec.com/exploring-cobalt-strikes-externalc2-framework/)

### Application Layer Protocol
- [C2 WebSocket](https://pentestlab.blog/2017/12/06/command-and-control-websocket/)
- [C2 WMI](https://pentestlab.blog/2017/11/20/command-and-control-wmi/)
- [C2 Website](https://pentestlab.blog/2017/11/14/command-and-control-website/)
- [C2 Image](https://pentestlab.blog/2018/01/02/command-and-control-images/)
- [C2 Javascript](https://pentestlab.blog/2018/01/08/command-and-control-javascript/)
- [C2 WebInterface](https://pentestlab.blog/2018/01/03/command-and-control-web-interface/)
- [C2 with DNS](https://pentestlab.blog/2017/09/06/command-and-control-dns/)
- [C2 with https](https://pentestlab.blog/2017/10/04/command-and-control-https/)
- [C2 with webdav](https://pentestlab.blog/2017/09/12/command-and-control-webdav/)
- [Introducing Merlin — A cross-platform post-exploitation HTTP/2 Command & Control Tool](https://medium.com/@Ne0nd0g/introducing-merlin-645da3c635a)
- [InternetExplorer.Application for C2](https://adapt-and-attack.com/2017/12/19/internetexplorer-application-for-c2/)

### Infrastructure
- [Automated Red Team Infrastructure Deployment with Terraform - Part 1](https://rastamouse.me/blog/terraform-pt1/)
- [Automated Red Team Infrastructure Deployment with Terraform - Part 2](https://rastamouse.me/blog/terraform-pt2/)
- [Red Team Infrastructure - AWS Encrypted EBS](https://rastamouse.me/blog/encrypted-ebs/)
- [6 RED TEAM INFRASTRUCTURE TIPS](https://cybersyndicates.com/2016/11/top-red-team-tips/)
- [How to Build a C2 Infrastructure with Digital Ocean – Part 1](https://www.blackhillsinfosec.com/build-c2-infrastructure-digital-ocean-part-1/)
- [Infrastructure for Ongoing Red Team Operations](https://blog.cobaltstrike.com/2014/09/09/infrastructure-for-ongoing-red-team-operations/)
- [Attack Infrastructure Log Aggregation and Monitoring](https://posts.specterops.io/attack-infrastructure-log-aggregation-and-monitoring-345e4173044e)
- [Randomized Malleable C2 Profiles Made Easy](https://bluescreenofjeff.com/2017-08-30-randomized-malleable-c2-profiles-made-easy/)
- [Migrating Your infrastructure](https://blog.cobaltstrike.com/2015/10/21/migrating-your-infrastructure/)
- [ICMP C2](https://pentestlab.blog/2017/07/28/command-and-control-icmp/)
- [Using WebDAV features as a covert channel](https://arno0x0x.wordpress.com/2017/09/07/using-webdav-features-as-a-covert-channel/)
- [Safe Red Team Infrastructure](https://medium.com/@malcomvetter/safe-red-team-infrastructure-c5d6a0f13fac)
- [EGRESSING BLUECOAT WITH COBALTSTIKE & LET'S ENCRYPT](https://cybersyndicates.com/2016/12/egressing-bluecoat-with-cobaltstike-letsencrypt/)
- [Command and Control Using Active Directory](http://www.harmj0y.net/blog/powershell/command-and-control-using-active-directory/)
- [A Vision for Distributed Red Team Operations](https://blog.cobaltstrike.com/2013/02/12/a-vision-for-distributed-red-team-operations/)
- [Designing Effective Covert Red Team Attack Infrastructure](https://bluescreenofjeff.com/2017-12-05-designing-effective-covert-red-team-attack-infrastructure/)
- [Serving Random Payloads with Apache mod_rewrite](https://bluescreenofjeff.com/2017-06-13-serving-random-payloads-with-apache-mod_rewrite/)
- [Mail Servers Made Easy](https://blog.inspired-sec.com/archive/2017/02/14/Mail-Server-Setup.html)
- [Securing your Empire C2 with Apache mod_rewrite](https://thevivi.net/2017/11/03/securing-your-empire-c2-with-apache-mod_rewrite/)
- [Automating Gophish Releases With Ansible and Docker](https://jordan-wright.com/blog/post/2018-02-04-automating-gophish-releases/)
- [How to Write Malleable C2 Profiles for Cobalt Strike](https://bluescreenofjeff.com/2017-01-24-how-to-write-malleable-c2-profiles-for-cobalt-strike/)
- [How to Make Communication Profiles for Empire](https://bluescreenofjeff.com/2017-03-01-how-to-make-communication-profiles-for-empire/)
- [A Brave New World: Malleable C2](http://www.harmj0y.net/blog/redteaming/a-brave-new-world-malleable-c2/)
- [Malleable Command and Control](https://www.cobaltstrike.com/help-malleable-c2)


##  Embedded and Peripheral Devices Hacking
- [Gettting in with the Proxmark3 & ProxBrute](https://www.trustwave.com/Resources/SpiderLabs-Blog/Getting-in-with-the-Proxmark-3-and-ProxBrute/)
- [Practical Guide to RFID Badge copying](https://blog.nviso.be/2017/01/11/a-practical-guide-to-rfid-badge-copying/)
- [Contents of a Physical Pentester Backpack](https://www.tunnelsup.com/contents-of-a-physical-pen-testers-backpack/)
- [MagSpoof - credit card/magstripe spoofer](https://github.com/samyk/magspoof)
- [Wireless Keyboard Sniffer](https://samy.pl/keysweeper/)
- [RFID Hacking with The Proxmark 3](https://blog.kchung.co/rfid-hacking-with-the-proxmark-3/)
- [Swiss Army Knife for RFID](https://www.cs.bham.ac.uk/~garciaf/publications/Tutorial_Proxmark_the_Swiss_Army_Knife_for_RFID_Security_Research-RFIDSec12.pdf)
- [Exploring NFC Attack Surface](https://media.blackhat.com/bh-us-12/Briefings/C_Miller/BH_US_12_Miller_NFC_attack_surface_WP.pdf)
- [Outsmarting smartcards](http://gerhard.dekoninggans.nl/documents/publications/dekoninggans.phd.thesis.pdf)
- [Reverse engineering HID iClass Master keys](https://blog.kchung.co/reverse-engineering-hid-iclass-master-keys/)
- [Android Open Pwn Project (AOPP)](https://www.pwnieexpress.com/aopp)


##  Misc
- [Red Tips of Vysec](https://github.com/vysec/RedTips)
- [Cobalt Strike Tips for 2016 ccde red teams](https://blog.cobaltstrike.com/2016/02/23/cobalt-strike-tips-for-2016-ccdc-red-teams/)
- [Models for Red Team Operations](https://blog.cobaltstrike.com/2015/07/09/models-for-red-team-operations/)
- [Planning a Red Team exercise](https://github.com/magoo/redteam-plan)
- [Raphael Mudge - Dirty Red Team tricks](https://www.youtube.com/watch?v=oclbbqvawQg)
- [introducing the adversary resilience methodology part 1](https://posts.specterops.io/introducing-the-adversary-resilience-methodology-part-one-e38e06ffd604)
- [introducing the adversary resilience methodology part 2](https://posts.specterops.io/introducing-the-adversary-resilience-methodology-part-two-279a1ed7863d)
- [Responsible red team](https://medium.com/@malcomvetter/responsible-red-teams-1c6209fd43cc)
- [Red Teaming for Pacific Rim CCDC 2017](https://bluescreenofjeff.com/2017-05-02-red-teaming-for-pacific-rim-ccdc-2017/)
- [How I Prepared to Red Team at PRCCDC 2015](https://bluescreenofjeff.com/2015-04-15-how-i-prepared-to-red-team-at-prccdc-2015/)
- [Red Teaming for Pacific Rim CCDC 2016](https://bluescreenofjeff.com/2016-05-24-pacific-rim-ccdc_2016/)
- [Responsible Red Teams](https://medium.com/@malcomvetter/responsible-red-teams-1c6209fd43cc)
- [Awesome-CobaltStrike](https://github.com/zer0yu/Awesome-CobaltStrike)
- RedTeaming from Zero to One [Part-1](https://payatu.com/redteaming-from-zero-to-one-part-1) [Part-2](https://payatu.com/redteaming-zero-one-part-2)

##  RedTeam Gadgets
#### Network Implants
- [LAN Tap Pro](https://hackerwarehouse.com/product/lan-tap-pro/)
- [LAN Turtle](https://hakshop.com/collections/network-implants/products/lan-turtle)
- [Bash Bunny](https://hakshop.com/collections/physical-access/products/bash-bunny)
- [Key Croc](https://shop.hak5.org/collections/sale/products/key-croc)
- [Packet Squirrel](https://hakshop.com/products/packet-squirrel)
- [Shark Jack](https://shop.hak5.org/collections/sale/products/shark-jack)
#### Wifi Auditing
- [WiFi Pineapple](https://hakshop.com/products/wifi-pineapple)
- [Alpha Long range Wireless USB](https://hackerwarehouse.com/product/alfa-802-11bgn-long-range-usb-wireless-adapter/)
- [Wifi-Deauth Monster](https://www.tindie.com/products/lspoplove/dstike-wifi-deauther-monster/)
- [Crazy PA](https://www.amazon.com/gp/product/B00VYA3A2U/ref=as_li_tl)
- [Signal Owl](https://shop.hak5.org/products/signal-owl)
#### IoT
- [BLE Key](https://hackerwarehouse.com/product/blekey/)
- [Proxmark3](https://hackerwarehouse.com/product/proxmark3-kit/)
- [Zigbee Sniffer](https://www.attify-store.com/products/zigbee-sniffing-tool-atmel-rzraven)
- [Attify IoT Exploit kit](https://www.attify-store.com/collections/frontpage/products/jtag-exploitation-kit-with-lab-manual)
#### Software Defined Radio - SDR
- [HackRF One Bundle](https://hackerwarehouse.com/product/hackrf-one-kit/)
- [RTL-SDR](https://hackerwarehouse.com/product/rtlsdr/)
- [YARD stick one Bundle](https://hackerwarehouse.com/product/yard-stick-one-kit/)
- [Ubertooth](https://hackerwarehouse.com/product/ubertooth-one/)
#### Misc
- [Key Grabber](https://hackerwarehouse.com/product/keygrabber/)
- [Magspoof](https://store.ryscc.com/products/magspoof%20)
- [Poison tap](https://samy.pl/poisontap/)
- [keysweeper](https://samy.pl/keysweeper/)
- [USB Rubber Ducky](https://hakshop.com/collections/physical-access/products/usb-rubber-ducky-deluxe)
- [Screen Crab](https://shop.hak5.org/collections/sale/products/screen-crab)
- [O.MG Cable](https://shop.hak5.org/collections/featured-makers/products/o-mg-cable)
- [Keysy](https://shop.hak5.org/collections/featured-makers/products/keysy)
- [Dorothy for Okta SSO](https://github.com/elastic/dorothy)

##  Ebooks
- [Next Generation Red Teaming](https://www.amazon.com/Next-Generation-Teaming-Henry-Dalziel/dp/0128041714)
- [Targeted Cyber Attack](https://www.amazon.com/Targeted-Cyber-Attacks-Multi-staged-Exploits/dp/0128006048)
- [Advanced Penetration Testing: Hacking the World's Most Secure Networks](https://www.amazon.com/Advanced-Penetration-Testing-Hacking-Networks/dp/1119367689)
- [Social Engineers' Playbook Practical Pretexting](https://www.amazon.com/Social-Engineers-Playbook-Practical-Pretexting/dp/0692306617/)
- [The Hacker Playbook 3: Practical Guide To Penetration Testing](https://www.amazon.com/Hacker-Playbook-Practical-Penetration-Testing-ebook/dp/B07CSPFYZ2)
- [How to Hack Like a PORNSTAR: A step by step process for breaking into a BANK ](https://www.amazon.com/How-Hack-Like-PORNSTAR-breaking-ebook/dp/B01MTDLGQQ)

##  Training ( Free )
- [Tradecraft - a course on red team operations](https://www.youtube.com/watch?v=IRpS7oZ3z0o&list=PL9HO6M_MU2nesxSmhJjEvwLhUoHPHmXvz)
- [Advanced Threat Tactics Course & Notes](https://blog.cobaltstrike.com/2015/09/30/advanced-threat-tactics-course-and-notes/)
- [FireEye - a whiteboard session on red team operations](https://www.fireeye.com/services/red-team-assessments/red-team-operations-video-training.html)

#### Home Lab
- [Building an Effective Active Directory Lab Environment for Testing](https://adsecurity.org/?p=2653)
- [Setting up DetectionLab](https://www.c2.lol/articles/setting-up-chris-longs-detectionlab)
- [vulnerable-AD - Script to make your home AD Lab vulnerable](https://github.com/WazeHell/vulnerable-AD)

##  Certification
- [CREST Certified Simulated Attack Specialist](http://www.crest-approved.org/examination/certified-simulated-attack-specialist/)
- [CREST Certified Simulated Attack Manager](http://www.crest-approved.org/examination/certified-simulated-attack-manager/)
- [SEC564: Red Team Operations and Threat Emulation](https://www.sans.org/course/red-team-operations-and-threat-emulation)
- [ELearn Security Penetration Testing eXtreme](https://www.elearnsecurity.com/course/penetration_testing_extreme/)
- [Certified Red Team Professional](https://www.pentesteracademy.com/activedirectorylab)
- [Certified Red Teaming Expert](https://www.pentesteracademy.com/redteamlab)
- [PentesterAcademy Certified Enterprise Security Specialist (PACES)](https://www.pentesteracademy.com/gcb)

------
# Blue Team
Tim biru adalah sekelompok individu yang melakukan analisis sistem informasi untuk memastikan keamanan, mengidentifikasi kelemahan keamanan, memverifikasi efektivitas setiap tindakan keamanan, dan memastikan semua tindakan keamanan akan terus efektif setelah implementasi.
(ref//https://en.wikipedia.org/wiki/Blue_team_(computer_security))


## Automation

- [Ansible Lockdown](https://ansiblelockdown.io/) - Curated collection of information security themed Ansible roles that are both vetted and actively maintained.
- [Clevis](https://github.com/latchset/clevis) - Plugable framework for automated decryption, often used as a Tang client.
- [DShell](https://github.com/USArmyResearchLab/Dshell) - Extensible network forensic analysis framework written in Python that enables rapid development of plugins to support the dissection of network packet captures.
- [Dev-Sec.io](https://dev-sec.io/) - Server hardening framework providing Ansible, Chef, and Puppet implementations of various baseline security configurations.
- [peepdf](https://eternal-todo.com/tools/peepdf-pdf-analysis-tool) - Scriptable PDF file analyzer.
- [PyREBox](https://talosintelligence.com/pyrebox) - Python-scriptable reverse engineering sandbox, based on QEMU.
- [Watchtower](https://containrrr.dev/watchtower/) - Container-based solution for automating Docker container base image updates, providing an unattended upgrade experience.

### Code libraries and bindings

- [MultiScanner](https://github.com/mitre/multiscanner) - File analysis framework written in Python that assists in evaluating a set of files by automatically running a suite of tools against them and aggregating the output.
- [Posh-VirusTotal](https://github.com/darkoperator/Posh-VirusTotal) - PowerShell interface to VirusTotal.com APIs.
- [censys-python](https://github.com/censys/censys-python) - Python wrapper to the Censys REST API.
- [libcrafter](https://github.com/pellegre/libcrafter) - High level C++ network packet sniffing and crafting library.
- [python-dshield](https://github.com/rshipp/python-dshield) - Pythonic interface to the Internet Storm Center/DShield API.
- [python-sandboxapi](https://github.com/InQuest/python-sandboxapi) - Minimal, consistent Python API for building integrations with malware sandboxes.
- [python-stix2](https://github.com/oasis-open/cti-python-stix2) - Python APIs for serializing and de-serializing Structured Threat Information eXpression (STIX) JSON content, plus higher-level APIs for common tasks.

### Security Orchestration, Automation, and Response (SOAR)

See also [Security Information and Event Management (SIEM)](#security-information-and-event-management-siem), and [IR management consoles](#ir-management-consoles).

- [Shuffle](https://shuffler.io/) - Graphical generalized workflow (automation) builder for IT professionals and blue teamers.

## Cloud platform security

See also [asecure.cloud/tools](https://asecure.cloud/tools/).

- [Aaia](https://github.com/rams3sh/Aaia) - Helps in visualizing AWS IAM and Organizations in a graph format with help of Neo4j.
- [Falco](https://falco.org/) - Behavioral activity monitor designed to detect anomalous activity in containerized applications, hosts, and network packet flows by auditing the Linux kernel and enriched by runtime data such as Kubernetes metrics.
- [Kata Containers](https://katacontainers.io/) - Secure container runtime with lightweight virtual machines that feel and perform like containers, but provide stronger workload isolation using hardware virtualization technology as a second layer of defense.
- [Principal Mapper (PMapper)](https://github.com/nccgroup/PMapper) - Quickly evaluate IAM permissions in AWS via script and library capable of identifying risks in the configuration of AWS Identity and Access Management (IAM) for an AWS account or an AWS organization.
- [Prowler](https://github.com/toniblyx/prowler) - Tool based on AWS-CLI commands for Amazon Web Services account security assessment and hardening.
- [Scout Suite](https://github.com/nccgroup/ScoutSuite) - Open source multi-cloud security-auditing tool, which enables security posture assessment of cloud environments.
- [gVisor](https://github.com/google/gvisor) - Application kernel, written in Go, that implements a substantial portion of the Linux system surface to provide an isolation boundary between the application and the host kernel.

### Distributed monitoring

See also [§ Service and performance monitoring](#service-and-performance-monitoring).

- [Cortex](https://cortexmetrics.io/) - Provides horizontally scalable, highly available, multi-tenant, long term storage for Prometheus.
- [Jaeger](https://www.jaegertracing.io/) - Distributed tracing platform backend used for monitoring and troubleshooting microservices-based distributed systems.
- [OpenTelemetry](https://opentelemetry.io/) - Observability framework for cloud-native software, comprising a collection of tools, APIs, and SDKs for exporting application performance metrics to a tracing backend (formerly maintained by the OpenTracing and OpenCensus projects).
- [Prometheus](https://prometheus.io/) - Open-source systems monitoring and alerting toolkit originally built at SoundCloud.
- [Zipkin](https://zipkin.io/) - Distributed tracing system backend that helps gather timing data needed to troubleshoot latency problems in service architectures.

### Kubernetes

See also [Kubernetes-Security.info](https://kubernetes-security.info/).

- [KubeSec](https://kubesec.io/) - Static analyzer of Kubernetes manifests that can be run locally, as a Kuberenetes admission controller, or as its own cloud service.
- [Kyverno](https://kyverno.io/) - Policy engine designed for Kubernetes.
- [Linkerd](https://linkerd.io/) - Ultra light Kubernetes-specific service mesh that adds observability, reliability, and security to Kubernetes applications without requiring any modification of the application itself.
- [Managed Kubernetes Inspection Tool (MKIT)](https://github.com/darkbitio/mkit) - Query and validate several common security-related configuration settings of managed Kubernetes cluster objects and the workloads/resources running inside the cluster.
- [Polaris](https://polaris.docs.fairwinds.com/) - Validates Kubernetes best practices by running tests against code commits, a Kubernetes admission request, or live resources already running in a cluster. 
- [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets) - Kubernetes controller and tool for one-way encrypted Secrets.
- [certificate-expiry-monitor](https://github.com/muxinc/certificate-expiry-monitor) - Utility that exposes the expiry of TLS certificates as Prometheus metrics.
- [k-rail](https://github.com/cruise-automation/k-rail) - Workload policy enforcement tool for Kubernetes.
- [kube-forensics](https://github.com/keikoproj/kube-forensics) - Allows a cluster administrator to dump the current state of a running pod and all its containers so that security professionals can perform off-line forensic analysis.
- [kube-hunter](https://kube-hunter.aquasec.com/) - Open-source tool that runs a set of tests ("hunters") for security issues in Kubernetes clusters from either outside ("attacker's view") or inside a cluster.
- [kubernetes-event-exporter](https://github.com/opsgenie/kubernetes-event-exporter) - Allows exporting the often missed Kubernetes events to various outputs so that they can be used for observability or alerting purposes.

### Service meshes

See also [ServiceMesh.es](https://servicemesh.es/).

- [Consul](https://consul.io/) - Solution to connect and configure applications across dynamic, distributed infrastructure and, with Consul Connect, enabling secure service-to-service communication with automatic TLS encryption and identity-based authorization.
- [Istio](https://istio.io/) - Open platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data.

## Communications security (COMSEC)

See also [Transport-layer defenses](#transport-layer-defenses).

- [GPG Sync](https://github.com/firstlookmedia/gpgsync) - Centralize and automate OpenPGP public key distribution, revocation, and updates amongst all members of an organization or team.
- [Geneva (Genetic Evasion)](https://censorship.ai/) - Novel experimental genetic algorithm that evolves packet-manipulation-based censorship evasion strategies against nation-state level censors to increase availability of otherwise blocked content.
- [GlobaLeaks](https://www.globaleaks.org/) - Free, open source software enabling anyone to easily set up and maintain a secure whistleblowing platform.
- [SecureDrop](https://securedrop.org/) - Open source whistleblower submission system that media organizations and NGOs can install to securely accept documents from anonymous sources.
- [Teleport](https://goteleport.com/) - Allows engineers and security professionals to unify access for SSH servers, Kubernetes clusters, web applications, and databases across all environments.

## DevSecOps

See also [awesome-devsecops](https://github.com/devsecops/awesome-devsecops).

- [Bane](https://github.com/genuinetools/bane) - Custom and better AppArmor profile generator for Docker containers.
- [BlackBox](https://github.com/StackExchange/blackbox) - Safely store secrets in Git/Mercurial/Subversion by encrypting them "at rest" using GnuPG.
- [Checkov](https://www.checkov.io/) - Static analysis for Terraform (infrastructure as code) to help detect CIS policy violations and prevent cloud security misconfiguration.
- [Cilium](https://cilium.io/) - Open source software for transparently securing the network connectivity between application services deployed using Linux container management platforms like Docker and Kubernetes.
- [Clair](https://github.com/coreos/clair) - Static analysis tool to probe for vulnerabilities introduced via application container (e.g., Docker) images.
- [CodeQL](https://securitylab.github.com/tools/codeql) - Discover vulnerabilities across a codebase by performing queries against code as though it were data.
- [DefectDojo](https://www.defectdojo.org/) - Application vulnerability management tool built for DevOps and continuous security integration.
- [Gauntlt](http://gauntlt.org/) - Pentest applications during routine continuous integration build pipelines.
- [Git Secrets](https://github.com/awslabs/git-secrets) - Prevents you from committing passwords and other sensitive information to a git repository.
- [SOPS](https://github.com/mozilla/sops) - Editor of encrypted files that supports YAML, JSON, ENV, INI and binary formats and encrypts with AWS KMS, GCP KMS, Azure Key Vault, and PGP.
- [Snyk](https://snyk.io/) - Finds and fixes vulnerabilities and license violations in open source dependencies and container images.
- [SonarQube](https://sonarqube.org) - Continuous inspection tool that provides detailed reports during automated testing and alerts on newly introduced security vulnerabilities.
- [Trivy](https://github.com/aquasecurity/trivy) - Simple and comprehensive vulnerability scanner for containers and other artifacts, suitable for use in continuous integration pipelines.
- [Vault](https://www.vaultproject.io/) - Tool for securely accessing secrets such as API keys, passwords, or certificates through a unified interface.
- [git-crypt](https://www.agwa.name/projects/git-crypt/) - Transparent file encryption in git; files which you choose to protect are encrypted when committed, and decrypted when checked out.
- [helm-secrets](https://github.com/jkroepke/helm-secrets) - Helm plugin that helps manage secrets with Git workflow and stores them anywhere, backed by SOPS.
- [terrascan](https://runterrascan.io/) - Static code analyzer for Infrastructure as Code tools that helps detect compliance and security violations to mitigate risk before provisioning cloud native resources.
- [tfsec](https://aquasecurity.github.io/tfsec/) - Static analysis security scanner for your Terraform code designed to run locally and in CI pipelines.

### Application or Binary Hardening

- [DynInst](https://dyninst.org/dyninst) - Tools for binary instrumentation, analysis, and modification, useful for binary patching.
- [DynamoRIO](https://dynamorio.org/) - Runtime code manipulation system that supports code transformations on any part of a program, while it executes, implemented as a process-level virtual machine.
- [Egalito](https://egalito.org/) - Binary recompiler and instrumentation framework that can fully disassemble, transform, and regenerate ordinary Linux binaries designed for binary hardening and security research.
- [Valgrind](https://www.valgrind.org/) - Instrumentation framework for building dynamic analysis tools.

### Compliance testing and reporting

- [Chef InSpec](https://www.chef.io/products/chef-inspec) - Language for describing security and compliance rules, which become automated tests that can be run against IT infrastructures to discover and report on non-compliance.
- [OpenSCAP Base](https://www.open-scap.org/tools/openscap-base/) - Both a library and a command line tool (`oscap`) used to evaluate a system against SCAP baseline profiles to report on the security posture of the scanned system(s). 

### Dependency confusion

See also [§ Supply chain security](#supply-chain-security).

- [Dependency Combobulator](https://github.com/apiiro/combobulator) - Open source, modular and extensible framework to detect and prevent dependency confusion leakage and potential attacks.
- [Confusion checker](https://github.com/sonatype-nexus-community/repo-diff) - Script to check if you have artifacts containing the same name between your repositories.
- [snync](https://github.com/snyk-labs/snync) - Prevent and detect if you're vulnerable to dependency confusion supply chain security attacks.

### Fuzzing

See also [Awesome-Fuzzing](https://github.com/secfigo/Awesome-Fuzzing).

* [Atheris](https://pypi.org/project/atheris/) - Coverage-guided Python fuzzing engine based off of libFuzzer that supports fuzzing of Python code but also native extensions written for CPython.
* [FuzzBench](https://google.github.io/fuzzbench/) - Free service that evaluates fuzzers on a wide variety of real-world benchmarks, at Google scale.
* [OneFuzz](https://github.com/microsoft/onefuzz) - Self-hosted Fuzzing-as-a-Service (FaaS) platform.

### Policy enforcement

- [AllStar](https://github.com/ossf/allstar) - GitHub App installed on organizations or repositories to set and enforce security policies.
- [Conftest](https://conftest.dev/) - Utility to help you write tests against structured configuration data.
- [Open Policy Agent (OPA)](https://www.openpolicyagent.org/) - Unified toolset and framework for policy across the cloud native stack.
- [Tang](https://github.com/latchset/tang) - Server for binding data to network presence; provides data to clients only when they are on a certain (secured) network.

### Supply chain security

See also [§ Dependency confusion](#dependency-confusion).

- [Grafeas](https://grafeas.io/) - Open artifact metadata API to audit and govern your software supply chain.
- [Helm GPG (GnuPG) Plugin](https://github.com/technosophos/helm-gpg) - Chart signing and verification with GnuPG for Helm.
- [Notary](https://github.com/theupdateframework/notary) - Aims to make the internet more secure by making it easy for people to publish and verify content.
- [in-toto](https://in-toto.io/) - Framework to secure the integrity of software supply chains.

## Honeypots

See also [awesome-honeypots](https://github.com/paralax/awesome-honeypots).

- [CanaryTokens](https://github.com/thinkst/canarytokens) - Self-hostable honeytoken generator and reporting dashboard; demo version available at [CanaryTokens.org](https://canarytokens.org/).
- [Kushtaka](https://kushtaka.org) - Sustainable all-in-one honeypot and honeytoken orchestrator for under-resourced blue teams.
- [Manuka](https://github.com/spaceraccoon/manuka) - Open-sources intelligence (OSINT) honeypot that monitors reconnaissance attempts by threat actors and generates actionable intelligence for Blue Teamers.

### Tarpits

- [Endlessh](https://github.com/skeeto/endlessh) - SSH tarpit that slowly sends an endless banner.
- [LaBrea](http://labrea.sourceforge.net/labrea-info.html) - Program that answers ARP requests for unused IP space, creating the appearance of fake machines that answer further requests very slowly in order to slow down scanners, worms, etcetera.

## Host-based tools

- [Artillery](https://github.com/BinaryDefense/artillery) - Combination honeypot, filesystem monitor, and alerting system designed to protect Linux and Windows operating systems.
- [chkrootkit](http://chkrootkit.org/) - Locally checks for signs of a rootkit on GNU/Linux systems.
- [Crowd Inspect](https://www.crowdstrike.com/resources/community-tools/crowdinspect-tool/) - Free tool for Windows systems aimed to alert you to the presence of malware that may be communicating over the network.
- [Fail2ban](https://www.fail2ban.org/) - Intrusion prevention software framework that protects computer servers from brute-force attacks.
- [Open Source HIDS SECurity (OSSEC)](https://www.ossec.net/) - Fully open source and free, feature-rich, Host-based Instrusion Detection System (HIDS).
- [Rootkit Hunter (rkhunter)](http://rkhunter.sourceforge.net/) - POSIX-compliant Bash script that scans a host for various signs of malware.

### Sandboxes

- [Bubblewrap](https://github.com/containers/bubblewrap) - Sandboxing tool for use by unprivileged Linux users capable of restricting access to parts of the operating system or user data.
- [Dangerzone](https://dangerzone.rocks/) - Take potentially dangerous PDFs, office documents, or images and convert them to a safe PDF.
- [Firejail](https://firejail.wordpress.com/) - SUID program that reduces the risk of security breaches by restricting the running environment of untrusted applications using Linux namespaces and seccomp-bpf.

## Identity and AuthN/AuthZ

- [Gluu Server](https://gluu.org/) - Central authentication and authorization for Web and mobile applications with a Free and Open Source Software cloud-native community distribution.

## Incident Response tools

See also [awesome-incident-response](https://github.com/meirwah/awesome-incident-response).

- [LogonTracer](https://github.com/JPCERTCC/LogonTracer) - Investigate malicious Windows logon by visualizing and analyzing Windows event log.
- [Volatility](https://www.volatilityfoundation.org/) - Advanced memory forensics framework.
- [aws_ir](https://github.com/ThreatResponse/aws_ir) - Automates your incident response with zero security preparedness assumptions.

### IR management consoles

See also [Security Orchestration, Automation, and Response (SOAR)](#security-orchestration-automation-and-response-soar).

- [CIRTKit](https://github.com/opensourcesec/CIRTKit) - Scriptable Digital Forensics and Incident Response (DFIR) toolkit built on Viper.
- [Fast Incident Response (FIR)](https://github.com/certsocietegenerale/FIR) - Cybersecurity incident management platform allowing for easy creation, tracking, and reporting of cybersecurity incidents.
- [Rekall](http://www.rekall-forensic.com/) - Advanced forensic and incident response framework.
- [TheHive](https://thehive-project.org/) - Scalable, free Security Incident Response Platform designed to make life easier for SOCs, CSIRTs, and CERTs, featuring tight integration with MISP.
- [threat_note](https://github.com/defpoint/threat_note) - Web application built by Defense Point Security to allow security researchers the ability to add and retrieve indicators related to their research.

### Evidence collection

- [AutoMacTC](https://github.com/CrowdStrike/automactc) - Modular, automated forensic triage collection framework designed to access various forensic artifacts on macOS, parse them, and present them in formats viable for analysis.
- [OSXAuditor](https://github.com/jipegit/OSXAuditor) - Free macOS computer forensics tool.
- [OSXCollector](https://github.com/Yelp/osxcollector) - Forensic evidence collection & analysis toolkit for macOS.
- [ir-rescue](https://github.com/diogo-fernan/ir-rescue) - Windows Batch script and a Unix Bash script to comprehensively collect host forensic data during incident response.
- [Margarita Shotgun](https://github.com/ThreatResponse/margaritashotgun) - Command line utility (that works with or without Amazon EC2 instances) to parallelize remote memory acquisition.

## Network perimeter defenses

- [Gatekeeper](https://github.com/AltraMayor/gatekeeper) - First open source Distributed Denial of Service (DDoS) protection system.
- [fwknop](https://www.cipherdyne.org/fwknop/) - Protects ports via Single Packet Authorization in your firewall.
- [ssh-audit](https://github.com/jtesta/ssh-audit) - Simple tool that makes quick recommendations for improving an SSH server's security posture.

### Firewall appliances or distributions

See also [Wikipedia: List of router and firewall distributions](https://en.wikipedia.org/wiki/List_of_router_and_firewall_distributions).

- [IPFire](https://www.ipfire.org/) - Hardened GNU/Linux based router and firewall distribution forked from IPCop.
- [OPNsense](https://opnsense.org/) - Hardened FreeBSD based firewall and routing platform forked from pfSense.
- [pfSense](https://www.pfsense.org/) - FreeBSD firewall and router distribution forked from m0n0wall.

## Operating System distributions

- [Computer Aided Investigative Environment (CAINE)](https://caine-live.net/) - Italian GNU/Linux live distribution that pre-packages numerous digital forensics and evidence collection tools.
- [Security Onion](https://securityonion.net/) - Free and open source GNU/Linux distribution for intrusion detection, enterprise security monitoring, and log management.
- [Qubes OS](https://qubes-os.org/) - Desktop environment built atop the Xen hypervisor project that runs each end-user program in its own virtual machine intended to provide strict security controls to constrain the reach of any successful malware exploit.

## Phishing awareness and reporting

See also [awesome-pentest § Social Engineering Tools](https://github.com/fabacab/awesome-pentest#social-engineering-tools).

- [CertSpotter](https://github.com/SSLMate/certspotter) - Certificate Transparency log monitor from SSLMate that alerts you when a SSL/TLS certificate is issued for one of your domains.
- [Gophish](https://getgophish.com/) - Powerful, open-source phishing framework that makes it easy to test your organization's exposure to phishing.
- [King Phisher](https://github.com/securestate/king-phisher) - Tool for testing and promoting user awareness by simulating real world phishing attacks.
- [NotifySecurity](https://github.com/certsocietegenerale/NotifySecurity) - Outlook add-in used to help your users to report suspicious e-mails to security teams.
- [Phishing Intelligence Engine (PIE)](https://github.com/LogRhythm-Labs/PIE) - Framework that will assist with the detection and response to phishing attacks.
- [Swordphish](https://github.com/certsocietegenerale/swordphish-awareness) - Platform allowing to create and manage (fake) phishing campaigns intended to train people in identifying suspicious mails. 
- [mailspoof](https://github.com/serain/mailspoof) - Scans SPF and DMARC records for issues that could allow email spoofing.
- [phishing_catcher](https://github.com/x0rz/phishing_catcher) - Configurable script to watch for issuances of suspicious TLS certificates by domain name in the Certificate Transparency Log (CTL) using the [CertStream](https://certstream.calidog.io/) service.

## Preparedness training and wargaming

- [APTSimulator](https://github.com/NextronSystems/APTSimulator) - Toolset to make a system look as if it was the victim of an APT attack.
- [Atomic Red Team](https://atomicredteam.io/) - Library of simple, automatable tests to execute for testing security controls.
- [BadBlood](https://www.secframe.com/badblood/) - Fills a test (non-production) Windows Domain with data that enables security analysts and engineers to practice using tools to gain an understanding and prescribe to securing Active Directory.
- [Caldera](https://caldera.mitre.org/) - Scalable, automated, and extensible adversary emulation platform developed by MITRE.
- [Drool](https://www.dns-oarc.net/tools/drool) - Replay DNS traffic from packet capture files and send it to a specified server, such as for simulating DDoS attacks on the DNS and measuring normal DNS querying.
- [DumpsterFire](https://github.com/TryCatchHCF/DumpsterFire) - Modular, menu-driven, cross-platform tool for building repeatable, time-delayed, distributed security events for Blue Team drills and sensor/alert mapping.
- [Infection Monkey](https://www.guardicore.com/infectionmonkey/) - Open-source breach and attack simulation (BAS) platform that helps you validate existing controls and identify how attackers might exploit your current network security gaps.
- [Metta](https://github.com/uber-common/metta) - Automated information security preparedness tool to do adversarial simulation.
- [Network Flight Simulator (`flightsim`)](https://github.com/alphasoc/flightsim) - Utility to generate malicious network traffic and help security teams evaluate security controls and audit their network visibility.
- [RedHunt OS](https://github.com/redhuntlabs/RedHunt-OS) - Ubuntu-based Open Virtual Appliance (`.ova`) preconfigured with several threat emulation tools as well as a defender's toolkit.

## Security configurations


- [Bunkerized-nginx](https://github.com/bunkerity/bunkerized-nginx) - Docker image of an NginX configuration and scripts implementing many defensive techniques for Web sites.

## Security monitoring

* [Starbase](https://github.com/JupiterOne/starbase) - Collects assets and relationships from services and systems into an intuitive graph view to offer graph-based security analysis for everyone.

### Endpoint Detection and Response (EDR)

- [Wazuh](https://wazuh.com/) - Open source, multiplatform agent-based security monitoring based on a fork of OSSEC HIDS.

### Network Security Monitoring (NSM)

See also [awesome-pcaptools](https://github.com/caesar0301/awesome-pcaptools).

- [ChopShop](https://github.com/MITRECND/chopshop) - Framework to aid analysts in the creation and execution of pynids-based decoders and detectors of APT tradecraft.
- [Maltrail](https://github.com/stamparm/maltrail) - Malicious network traffic detection system.
- [Moloch](https://github.com/aol/moloch) - Augments your current security infrastructure to store and index network traffic in standard PCAP format, providing fast, indexed access.
- [OwlH](https://www.owlh.net/) - Helps manage network IDS at scale by visualizing Suricata, Zeek, and Moloch life cycles.
- [Real Intelligence Threat Analysis (RITA)](https://github.com/activecm/rita) - Open source framework for network traffic analysis that ingests Zeek logs and detects beaconing, DNS tunneling, and more.
- [Respounder](https://github.com/codeexpress/respounder) - Detects the presence of the Responder LLMNR/NBT-NS/MDNS poisoner on a network.
- [Snort](https://snort.org/) - Widely-deployed, Free Software IPS capable of real-time packet analysis, traffic logging, and custom rule-based triggers.
- [SpoofSpotter](https://github.com/NetSPI/SpoofSpotter) - Catch spoofed NetBIOS Name Service (NBNS) responses and alert to an email or log file.
- [Stenographer](https://github.com/google/stenographer) - Full-packet-capture utility for buffering packets to disk for intrusion detection and incident response purposes.
- [Suricata](https://suricata-ids.org/) - Free, cross-platform, IDS/IPS with on- and off-line analysis modes and deep packet inspection capabilities that is also scriptable with Lua.
- [Tsunami](https://github.com/google/tsunami-security-scanner) - General purpose network security scanner with an extensible plugin system for detecting high severity vulnerabilities with high confidence. 
- [VAST](https://github.com/tenzir/vast) - Free and open-source network telemetry engine for data-driven security investigations.
- [Wireshark](https://www.wireshark.org) - Free and open-source packet analyzer useful for network troubleshooting or forensic netflow analysis.
- [Zeek](https://zeek.org/) - Powerful network analysis framework focused on security monitoring, formerly known as Bro.
- [netsniff-ng](http://netsniff-ng.org/) -  Free and fast GNU/Linux networking toolkit with numerous utilities such as a connection tracking tool (`flowtop`), traffic generator (`trafgen`), and autonomous system (AS) trace route utility (`astraceroute`).

### Security Information and Event Management (SIEM)

- [AlienVault OSSIM](https://www.alienvault.com/open-threat-exchange/projects) - Single-server open source SIEM platform featuring asset discovery, asset inventorying, behavioral monitoring, and event correlation, driven by AlienVault Open Threat Exchange (OTX).
- [Prelude SIEM OSS](https://www.prelude-siem.org/) - Open source, agentless SIEM with a long history and several commercial variants featuring security event collection, normalization, and alerting from arbitrary log input and numerous popular monitoring tools.

### Service and performance monitoring

See also [awesome-sysadmin#monitoring](https://github.com/n1trux/awesome-sysadmin#monitoring).

- [Icinga](https://icinga.com/) - Modular redesign of Nagios with pluggable user interfaces and an expanded set of data connectors, collectors, and reporting tools.
- [Locust](https://locust.io/) - Open source load testing tool in which you can define user behaviour with Python code and swarm your system with millions of simultaneous users.
- [Nagios](https://nagios.org) - Popular network and service monitoring solution and reporting platform.
- [OpenNMS](https://opennms.org/) - Free and feature-rich networking monitoring system supporting multiple configurations, a variety of alerting mechanisms (email, XMPP, SMS), and numerous data collection methods (SNMP, HTTP, JDBC, etc).
- [osquery](https://github.com/facebook/osquery) - Operating system instrumentation framework for macOS, Windows, and Linux, exposing the OS as a high-performance relational database that can be queried with a SQL-like syntax.
- [Zabbix](https://www.zabbix.com/) - Mature, enterprise-level platform to monitor large-scale IT environments.

### Threat hunting

See also [awesome-threat-detection](https://github.com/0x4D31/awesome-threat-detection).

- [CimSweep](https://github.com/PowerShellMafia/CimSweep) - Suite of CIM/WMI-based tools enabling remote incident response and hunting operations across all versions of Windows.
- [DeepBlueCLI](https://github.com/sans-blue-team/DeepBlueCLI) - PowerShell module for hunt teaming via Windows Event logs.
- [GRR Rapid Response](https://github.com/google/grr) - Incident response framework focused on remote live forensics consisting of a Python agent installed on assets and Python-based server infrastructure enabling analysts to quickly triage attacks and perform analysis remotely.
- [Hunting ELK (HELK)](https://github.com/Cyb3rWard0g/HELK) - All-in-one Free Software threat hunting stack based on Elasticsearch, Logstash, Kafka, and Kibana with various built-in integrations for analytics including Jupyter Notebook.
- [MozDef](https://github.com/mozilla/MozDef) - Automate the security incident handling process and facilitate the real-time activities of incident handlers.
- [PSHunt](https://github.com/Infocyte/PSHunt) - PowerShell module designed to scan remote endpoints for indicators of compromise or survey them for more comprehensive information related to state of those systems.
- [PSRecon](https://github.com/gfoss/PSRecon) - PSHunt-like tool for analyzing remote Windows systems that also produces a self-contained HTML report of its findings.
- [PowerForensics](https://github.com/Invoke-IR/PowerForensics) - All in one PowerShell-based platform to perform live hard disk forensic analysis.
- [rastrea2r](https://github.com/rastrea2r/rastrea2r) - Multi-platform tool for triaging suspected IOCs on many endpoints simultaneously and that integrates with antivirus consoles.
- [Redline](https://www.fireeye.com/services/freeware/redline.html) - Freeware endpoint auditing and analysis tool that provides host-based investigative capabilities, offered by FireEye, Inc.

## Threat intelligence

See also [awesome-threat-intelligence](https://github.com/hslatman/awesome-threat-intelligence).
- [Threat Hunting Fundamental - Online Workshop](https://youtu.be/d4h7GRpD44s) - [Blue Team Indonesia](https://blueteam.id/)
- [AttackerKB](https://attackerkb.com/) - Free and public crowdsourced vulnerability assessment platform to help prioritize high-risk patch application and combat vulnerability fatigue.
- [DATA](https://github.com/hadojae/DATA) - Credential phish analysis and automation tool that can accept suspected phishing URLs directly or trigger on observed network traffic containing such a URL.
- [Forager](https://github.com/opensourcesec/Forager) - Multi-threaded threat intelligence gathering built with Python3 featuring simple text-based configuration and data storage for ease of use and data portability.
- [GRASSMARLIN](https://github.com/nsacyber/GRASSMARLIN) - Provides IP network situational awareness of industrial control systems (ICS) and Supervisory Control and Data Acquisition (SCADA) by passively mapping, accounting for, and reporting on your ICS/SCADA network topology and endpoints.
- [MLSec Combine](https://github.com/mlsecproject/combine) - Gather and combine multiple threat intelligence feed sources into one customizable, standardized CSV-based format.
- [Malware Information Sharing Platform and Threat Sharing (MISP)](https://misp-project.org/) - Open source software solution for collecting, storing, distributing and sharing cyber security indicators.
- [Open Source Vulnerabilities (OSV)](https://osv.dev/) - Vulnerability database and triage infrastructure for open source projects aimed at helping both open source maintainers and consumers of open source.
- [Sigma](https://github.com/Neo23x0/sigma) - Generic signature format for SIEM systems, offering an open signature format that allows you to describe relevant log events in a straightforward manner.
- [Threat Bus](https://github.com/tenzir/threatbus) - Threat intelligence dissemination layer to connect security tools through a distributed publish/subscribe message broker.
- [ThreatIngestor](https://github.com/InQuest/ThreatIngestor) - Extendable tool to extract and aggregate IOCs from threat feeds including Twitter, RSS feeds, or other sources.
- [Unfetter](https://nsacyber.github.io/unfetter/) - Identifies defensive gaps in security posture by leveraging Mitre's ATT&CK framework.
- [Viper](https://github.com/viper-framework/viper) - Binary analysis and management framework enabling easy organization of malware and exploit samples.
- [YARA](https://github.com/VirusTotal/yara) - Tool aimed at (but not limited to) helping malware researchers to identify and classify malware samples, described as "the pattern matching swiss army knife" for file patterns and signatures.

### Fingerprinting

- [HASSH](https://github.com/salesforce/hassh) - Network fingerprinting standard which can be used to identify specific client and server SSH implementations.
- [JA3](https://ja3er.com/) - Extracts SSL/TLS handshake settings for fingerprinting and communicating about a given TLS implementation.

### Threat signature packages and collections

- [ESET's Malware IoCs](https://github.com/eset/malware-ioc) - Indicators of Compromises (IOCs) derived from ESET's various investigations.
- [FireEye's Red Team Tool Countermeasures](https://github.com/fireeye/red_team_tool_countermeasures) - Collection of Snort and YARA rules to detect attacks carried out with FireEye's own Red Team tools, first released after FireEye disclosed a breach in December 2020.
- [FireEye's Sunburst Countermeasures](https://github.com/fireeye/sunburst_countermeasures) - Collection of IoC in various languages for detecting backdoored SolarWinds Orion NMS activities and related vulnerabilities.
- [YARA Rules](https://github.com/Yara-Rules/rules) - Project covering the need for IT security researchers to have a single repository where different Yara signatures are compiled, classified and kept as up to date as possible.

## Tor Onion service defenses

See also [awesome-tor](https://github.com/ajvb/awesome-tor).

- [OnionBalance](https://onionbalance.readthedocs.io/) - Provides load-balancing while also making Onion services more resilient and reliable by eliminating single points-of-failure.
- [Vanguards](https://github.com/mikeperry-tor/vanguards) - Version 3 Onion service guard discovery attack mitigation script (intended for eventual inclusion in Tor core).

## Transport-layer defenses

- [Certbot](https://certbot.eff.org/) - Free tool to automate the issuance and renewal of TLS certificates from the [LetsEncrypt Root CA](https://letsencrypt.org/) with plugins that configure various Web and e-mail server software.
- [MITMEngine](https://github.com/cloudflare/mitmengine) - Golang library for server-side detection of TLS interception events.
- [Tor](https://torproject.org/) - Censorship circumvention and anonymizing overlay network providing distributed, cryptographically verified name services (`.onion` domains) to enhance publisher privacy and service availability.

### Overlay and Virtual Private Networks (VPNs)

- [IPsec VPN Server Auto Setup Scripts](https://github.com/hwdsl2/setup-ipsec-vpn) - Scripts to build your own IPsec VPN server, with IPsec/L2TP, Cisco IPsec and IKEv2.
- [Innernet](https://github.com/tonarino/innernet) - Free Software private network system that uses WireGuard under the hood, made to be self-hosted.
- [Nebula](https://github.com/slackhq/nebula) - Completely open source and self-hosted, scalable overlay networking tool with a focus on performance, simplicity, and security, inspired by tinc.
- [OpenVPN](https://openvpn.net/) - Longstanding Free Software traditional SSL/TLS-based virtual private network.
- [OpenZITI](https://openziti.github.io/) - Open source initiative focused on bringing Zero Trust to any application via an overlay network, tunelling applications, and numerous SDKs.
- [Tailscale](https://tailscale.com/) - Managed freemium mesh VPN service built on top of WireGuard.
- [WireGuard](https://www.wireguard.com/) - Extremely simple yet fast and modern VPN that utilizes state-of-the-art cryptography.
- [tinc](https://tinc-vpn.org/) - Free Software mesh VPN implemented entirely in userspace that supports expandable network space, bridged ethernet segments, and more.

## macOS-based defenses

See also [drduh/macOS-Security-and-Privacy-Guide](https://github.com/drduh/macOS-Security-and-Privacy-Guide).

- [BlockBlock](https://objective-see.com/products/blockblock.html) - Monitors common persistence locations and alerts whenever a persistent component is added, which helps to detect and prevent malware installation.
- [LuLu](https://objective-see.com/products/lulu.html) - Free macOS firewall.
- [Santa](https://github.com/google/santa) - Keep track of binaries that are naughty or nice in an allow/deny-listing system for macOS.
- [Stronghold](https://github.com/alichtman/stronghold) - Easily configure macOS security settings from the terminal.
- [macOS Fortress](https://github.com/essandess/macOS-Fortress) - Automated configuration of kernel-level, OS-level, and client-level security features including privatizing proxying and anti-virus scanning for macOS.

## Windows-based defenses

See also [awesome-windows#security](https://github.com/Awesome-Windows/Awesome#security) and [awesome-windows-domain-hardening](https://github.com/PaulSec/awesome-windows-domain-hardening).

- [CobaltStrikeScan](https://github.com/Apr4h/CobaltStrikeScan) - Scan files or process memory for Cobalt Strike beacons and parse their configuration.
- [HardenTools](https://github.com/securitywithoutborders/hardentools) - Utility that disables a number of risky Windows features.
- [NotRuler](https://github.com/sensepost/notruler) - Detect both client-side rules and VBScript enabled forms used by the [Ruler](https://github.com/sensepost/ruler) attack tool when attempting to compromise a Microsoft Exchange server.
- [Sandboxie](https://www.sandboxie.com/) - Free and open source general purpose Windows application sandboxing utility.
- [Sigcheck](https://docs.microsoft.com/en-us/sysinternals/downloads/sigcheck) - Audit a Windows host's root certificate store against Microsoft's [Certificate Trust List (CTL)](https://docs.microsoft.com/en-us/windows/desktop/SecCrypto/certificate-trust-list-overview).
- [Sticky Keys Slayer](https://github.com/linuz/Sticky-Keys-Slayer) - Establishes a Windows RDP session from a list of hostnames and scans for accessibility tools backdoors, alerting if one is discovered.
- [Windows Secure Host Baseline](https://github.com/nsacyber/Windows-Secure-Host-Baseline) - Group Policy objects, compliance checks, and configuration tools that provide an automated and flexible approach for securely deploying and maintaining the latest releases of Windows 10.
- [WMI Monitor](https://github.com/realparisi/WMI_Monitor) - Log newly created WMI consumers and processes to the Windows Application event log.

### Active Directory

- [Active Directory Control Paths](https://github.com/ANSSI-FR/AD-control-paths) - Visualize and graph Active Directory permission configs ("control relations") to audit questions such as "Who can read the CEO's email?" and similar.
- [PingCastle](https://www.pingcastle.com/) - Active Directory vulnerability detection and reporting tool.
- [PlumHound](https://github.com/PlumHound/PlumHound) - More effectively use BloodHoundAD in continual security life-cycles by utilizing its pathfinding engine to identify Active Directory security vulnerabilities.

## Reverse Engineering
- [Konsep Dasar dan Binary Executable](https://youtu.be/RczzwR52NYw) - Cyber Security IPB	
- [Static analysis 1](https://youtu.be/mhzp6a3KYxs) - Cyber Security IPB	
- [Static analysis 2](https://youtu.be/VCXsLvMqaBo) - Cyber Security IPB	
- [Debugging dengan IDA](https://youtu.be/qPV34Pzqv04) - Cyber Security IPB	
- [Debugging dengan GDB - PEDA](https://www.youtube.com/watch?v=ez7d3EX0yuE) - Cyber Security IPB	
- [ltrace ](https://youtu.be/WT1s3tE5Q5w) - Cyber Security IPB	
- [Static linked binary ](https://youtu.be/XVvMLyZ8b1I) - Cyber Security IPB	
- [Reverse Engineering For Blue Team - Online Workshop](https://youtu.be/yLhQM5tRiZo) - [Blue Team Indonesia](https://blueteam.id/)

## Malware Analysis
- [Pengelanan Malware Analaysis](https://youtu.be/k9ySYLcIpag) - [Blue Team Indonesia](https://blueteam.id/)
- [Basic Static Malware Analysis](https://www.youtube.com/watch?v=kNOhixlj3dk) - Ngobrol IT Bareng Teknik Komputer
------
# Bug Bounty
Bug Bounty Program adalah sebuah inisiatif perusahaan yang mengapresiasi temuan celah keamanan dari para Peretas disebut juga dengan Bughunter pada suatu aplikasi / sistem / layanan. Perusahaan dapat menemukan kerentanan lebih dini sebelum pihak yang tidak bertanggungjawab menemukan dan mengeksploitasinya. Melalui program ini juga, perusahaan dapat mengimplementasikan kontrol keamanan secara berkelanjutan. (ref//www.cyberarmy.id)

## Introduce Bug Bounty
- [Apa Itu Bug Bounty dan Sejarahnya](https://www.youtube.com/watch?v=2KHn0_UJhQg) - MrDoel
- [Pengenalan dan Benefit Bug Bounty](https://youtu.be/IdXvfHrMJSQ?t=680) - Pondok Daring Siber
- [Bug Hunting - Open redirect, XSS, IDOR](https://youtu.be/lHdfeY4RB3E) - Pondok Daring Siber
- [Essential & Favorite Bug Bounty Hunting Tools](https://www.youtube.com/watch?v=avU_QuAQQk8) - Semi Yulianto
- [Bug Hunter Muda Talk Spesialisasi XSS](https://www.youtube.com/watch?v=Dy6_QVxgkUo) - Orang Siber Channel
- [Bug Bounty Untuk Pemula - Asset Discovery](https://youtu.be/_1To4mAZeIc) - [MrDoel Hacking](https://www.youtube.com/channel/UCdrjciKY9Rwch6aUoo51VEw)
- [5 Bug Bounty Program](https://youtu.be/n9n3Y4qKgoc) - Doddy Ferdiansyah 
- [DAPETIN REWARD DENGAN SKILLMU!!! - Yuk Pahami Tentang Bug Bounty Program](https://youtu.be/0sfVDQnIlfs) - Doddy Ferdiansyah 
- [Cara Menjadi Bug Bounty Hunter - Bug Bounty 2022](https://youtu.be/ZxVO3d-X8vc) - RootBakar Official

## Story Bug Hunting
- [Mendapat 100 Juta Dari Google Karena Melaporkan Bug](https://www.youtube.com/watch?v=XWiByCaSbAk) - Nosa Shandy
- [Bugs Bounty from Zero to Hero](https://youtu.be/zaFC8vjS0u4) - ECHO|TALK

## Resources Cyber Security From Twitter
<a href="https://spiritual-worm-485.notion.site/547a733dd61844c1a9bdf7fa5e11bebc?v=4b037e2e868844bdb17e198fda138ff1">https://spiritual-worm-485.notion.site/547a733dd61844c1a9bdf7fa5e11bebc?v=4b037e2e868844bdb17e198fda138ff1</a>

## Cyber Security Books
<table width="100%" class="table">
<tr>
<th>S.No</th>
<th>E-Book (PDF Link)</th>
<th>Total Pages</th>
</tr>
<tr><td>1.</td><td><a target="_blank" href="https://mega.nz/file/abI2jbxA#rLmfn-cda99y9VF9NaV53xQEzIY_wHVtyRodLU-qKyg">Advanced Penetration Testing</a></td><td>269 Pages</td></tr>
<tr><td>2.</td><td><a target="_blank" href="https://mega.nz/file/ieYyXDYS#F7jKWnuYmiA31vI7AcUbOJ_8bpttxz4wDIDEjxzJBDc">The Basics of Web Hacking</a></td><td>179 Pages</td></tr>
<tr><td>3.</td><td><a target="_blank" href="https://mega.nz/file/2WQ0gJIL#ctQd0e-yzb1QXoYk01yPTA9jl78TbNaZI4GoLdg6PSo">The Basics of Hacking and Penetration Testing</a></td><td>178 Pages</td></tr>
<tr><td>4.</td><td><a target="_blank" href="https://mega.nz/file/bXYQ2JoR#yR6BzKz4sva2qAzRMCju1jpHphgwe12ssZLknBNk4yc">The Art of Deception by Kevin Mitnick</a></td><td>577 Pages</td></tr>
<tr><td>5.</td><td><a target="_blank" href="https://mega.nz/file/bPYkjLhb#ZovQRMu6VMwkdLqOFhuUi4wCj7Pq0PJgiHZiItUt0DY">SQL Injection Attacks and Defense</a></td><td>761 Pages</td></tr>
<tr><td>6.</td><td><a target="_blank" href="https://mega.nz/file/mfIkHZJZ#Y6ZftkyGJc8Rw2WI63v213iIl_SMEtY1qBsb7p2nQjs">Metasploit - The Penetration Tester's Guide</a></td><td>332 Pages</td></tr>
<tr><td>7.</td><td><a target="_blank" href="https://mega.nz/file/HDYUzZAY#jQ0ohALFI2fKrO6S5JzRjOZn6YmAMqKgkCPQLM0Peew">Ethical Hacking and Penetration Testing Guide</a></td><td>523 Pages</td></tr>
<tr><td>8.</td><td><a target="_blank" href="https://mega.nz/file/6WQGAD6Z#UGry-SnTLB3s4qMfh29s6jDromDGQc8I_fkWIqAY6rc">Network Attacks and Exploitation - A Framework</a></td><td>219 Pages</td></tr>
<tr><td>9.</td><td><a target="_blank" href="https://difl.host/6e39ff5edc948cb1/09._Python_Web_Penetration_Testing_Cookbook.pdf">Python Web Penetration Testing Cookbook</a></td><td>224 Pages</td></tr>
<tr><td>10.</td><td><a target="_blank" href="https://mega.nz/file/7TRUCZCZ#ZPFmeFnccvR4ltf_2lwTdi8PqHIArRx_bkqRP9wwq4k">Wireshark for Security Professionals</a></td><td>391 Pages</td></tr>
<tr><td>11.</td><td><a target="_blank" href="https://openload.co/f/2tsVl0FU0Kc/11._Modern_Web_Penetration_Testing.pdf">Mastering Modern Web Penetration Testing</a></td><td>298 Pages</td></tr>
<tr><td>12.</td><td><a target="_blank" href="https://mega.nz/file/3OZgwT6Z#8yNyiuSHVQ3gOib4rKJYtwsCwSfqAfoFj2lQtwUyI8o">The Shellcoder's Handbook</a></td><td>745 Pages</td></tr>
<tr><td>13.</td><td><a target="_blank" href="https://mega.nz/file/SDICALSJ#3r2oy2AsGXR3P7f8K7xvL2kEVjR6ccze83cAmz9VIBc">The Little Black Book of Computer Viruses</a></td><td>183 Pages</td></tr>
<tr><td>14.</td><td><a target="_blank" href="https://mega.nz/file/3XJCyD5C#qAda14pWUjd5u4wjOYmzCI52UMa1rUFulh7V0kBGZk8">XSS Attacks - Cross Site Scripting Exploits and Defense</a></td><td>482 Pages</td></tr>
<tr><td>15.</td><td><a target="_blank" href="https://mega.nz/file/jTBwVL6T#hVGYbGKJCcbUh83yztODz-8aMZZbJMWPoCdmr5Z4C9w">The Web Application Hacker's Handbook</a></td><td>771 Pages</td></tr>
<tr><td>16.</td><td><a target="_blank" href="https://mega.nz/file/2fAyRb4C#tpFivx91Ips2rR3UnVdtlgvx1oOmi-qEtCu29DlO9uQ">Ethical Hacking and Countermeasures</a></td><td>239 Pages</td></tr>
<tr><td>17.</td><td><a target="_blank" href="https://mega.nz/file/LGRUzLIC#MB5a5s9wpaWEEGnhi5j_73kMtPIQx0rEuQXv5_Y_gd4">Reversing - Secrets of Reverse Engineering</a></td><td>619 Pages</td></tr>
<tr><td>18.</td><td><a target="_blank" href="https://mega.nz/file/mLAUEbDQ#PXzqsNN2PPc-PUVyAwbfknTHEA-QBvjwvpjjQgZnYMo">Network Security Bible</a></td><td>697 Pages</td></tr>
<tr><td>19.</td><td><a target="_blank" href="https://mega.nz/file/LCYWWRYI#QQ8O9k6lp7vmYWzrbxbs8ItSVbYpSluYfktCxWURZGs">Hacking Web Applications - Hacking Exposed</a></td><td>416 Pages</td></tr>
<tr><td>20.</td><td><a target="_blank" href="https://mega.nz/file/iKQ2jZSQ#ur1W05ChW7_ipTYtEK6QKpIlyoqLyS82RGsEUEzFQDQ">Hacking for Dummies</a></td><td>387 Pages</td></tr>
<tr><td>21.</td><td><a target="_blank" href="https://mega.nz/file/6LI20T7B#TvvIUOn5TQ4HsS4qrTAX6dOD0JG4tZ9FtLj6bEFGg2M">Hacking Wireless Network for Dummies</a></td><td>387 Pages</td></tr>
<tr><td>22.</td><td><a target="_blank" href="https://mega.nz/file/SDAikR4I#b018YKF4UZ2xRh0mqouRm6pssXd0lbWRuwCoPepxW2Q">Ninja Hacking - Unconventional Penetration Testing Tacting and Techniques</a></td><td>314 pages</td></tr>
<tr><td>23.</td><td><a target="_blank" href="https://mega.nz/file/3PYElRpL#GWFniwOY738v8URo3HsnQwVV5h957-Ppx7FxMwYmJCI">Professional Penetration Testing</a></td><td>525 Pages</td></tr>
<tr><td>24.</td><td><a target="_blank" href="https://mega.nz/file/yGYihB7I#8bmNXXPvSgIotZTsPbGaR-dSj9MfyOoNmm7iZ2me798">Gray Hat Hacking - The Ethical Hacker's Handbook</a></td><td>577 Pages</td></tr>
<tr><td>25.</td><td><a target="_blank" href="https://mega.nz/file/mGIC2TBD#pkJBqjgeN_BJWe8PRveaA4nwRICK7WQ80BUowDSVfXI">Hack Attacks Testing</a></td><td>561 Pages</td></tr>
<tr><td>26.</td><td><a target="_blank" href="https://mega.nz/file/6GIAHb4B#oh0fxNYfOqiyCNoeyqayetg_e2G3B8ZF7M3lr3NMCgU">Basic Security Testing with Kali Linux</a></td><td>242 Pages</td></tr>
<tr><td>27.</td><td><a target="_blank" href="https://difl.host/ba9765fffecd1e25/27._Mastering_Kali_Linux_For_Advanced_Penetration_Testing.pdf">Mastering Kali Linux for Advanced Penetration Testing</a></td><td>356 Pages</td></tr>
<tr><td>28.</td><td><a target="_blank" href="https://difl.host/ab3e7a5e5a023fdc/28._Kali_Linux_CTF_Blueprints.pdf">Kali Linux CTF Blueprints</a></td><td>190 Pages</td></tr>
<tr><td>29.</td><td><a target="_blank" href="https://difl.host/f152e4b334a4d268/29._Kali_Linux_Cookbook.pdf">Kali Linux Cookbook</a></td><td>261 Pages</td></tr>
<tr><td>30.</td><td><a target="_blank" href="https://difl.host/670feaf53fca0080/30._Kali_Linux-_Assuring_Security_by_Penetration_Testing.pdf">Kali Linux - Assuring Security by Penetration Testing</a></td><td>454 Pages</td></tr>
<tr><td>31.</td><td><a target="_blank" href="https://mega.nz/file/uDZGSDoA#vZXeBRcG7poaDNMaNd9XXe7FYWAO8MIk4DYmglq1tBQ">Information Security  Management Handbook</a></td><td>3206 Pages</td></tr>
<tr><td>32.</td><td><a target="_blank" href="https://mega.nz/file/PfIyiRaD#wjKpxiT-qi9r5W8px3-aDqiglZMr1fyh3ThkwPPyrRQ">Computer and Information Security Handbook</a></td><td>877 Pages</td></tr>
<tr><td>33.</td><td><a target="_blank" href="https://mega.nz/file/WfRWkJIT#Z0ox5K8qeLeobE6VoBeXsrO5mxu68HeaczcCFRg5hC8">CISSP - Certified Information Systems Security Professional</a></td><td>804 Pages</td></tr>
<tr><td>34.</td><td><a target="_blank" href="https://mega.nz/file/WKAERJqY#nnLb6e1SWgEL6D3kqdY2FLmHhK8wuxHUyJM-ghiC4JI">Computer Security and Cryptography</a></td><td>542 Pages</td></tr>
<tr><td>35.</td><td><a target="_blank" href="https://mega.nz/file/6eRkDLya#BlJ7rynz9UHI74hTmlJzroUgbOiy1O-cpFun5qeNjVg">Python for Kids</a></td><td>348 Pages</td></tr>
<tr><td>36.</td><td><a target="_blank" href="https://mega.nz/file/TPBQyZCR#vvwYa_Z95mtaWhWSPDBot7fINfoQ8cpnH4qm9xus1TY">End to End Network Security - Defense-in-Depth</a></td><td>469 Pages</td></tr>
<tr><td>37.</td><td><a target="_blank" href="https://mega.nz/file/bXZEhTAY#Qx7oHuIWzeUjBMxRKMFo-lUkiKnliQOJUAjoFJfSLDM">A Guide to Computer Network Security</a></td><td>483 Pages</td></tr>
<tr><td>38.</td><td><a target="_blank" href="https://mega.nz/file/2CAU2JAY#R16cOg64vgZxs02bTFD7dYSXRgZDLcog2lcb5CJ33k8">Essential Computer Security</a></td><td>321 Pages</td></tr>
<tr><td>39.</td><td><a target="_blank" href="https://mega.nz/file/qbJiBJoB#6HKrc6AA3oMLl5GB5CnwmXtbH9cVkqqU-4PBdJZcNaE">Security in Wireless Mesh Networks</a></td><td>548 Pages</td></tr>
<tr><td>40.</td><td><a target="_blank" href="https://mega.nz/file/DOY2nJ6B#Lfw_qx1ljqzXmJnnl0x68v_4iR3B2AIIOr-LaPRzLm0">Hacking Windows XP (OLD)</a></td><td>379 Pages</td></tr>
<tr><td>41.</td><td><a target="_blank" href="https://mega.nz/file/aLImDJCZ#nrX0SEvIU_LJB8UNQwn7xCmnMAoELGGS69lVRehN6T4">Hacking Exposed - Windows Security, Secrets and Solutions</a></td><td>482 Pages</td></tr>
<tr><td>42.</td><td><a target="_blank" href="https://mega.nz/file/iSIgDZZQ#o3ZyT0v2NK1PjxeGtynIw8v3gS7g_0Yk4AN3ofXIWdc">Hacking Exposed - Network Security, Secrets and Solutions</a></td><td>736 Pages</td></tr>
<tr><td>43.</td><td><a target="_blank" href="https://mega.nz/file/CeIkBJKa#YmsoJD1cT0hpl3d3No7HnAFIlrdYe7qDpDP4UkgQ25U">Information Security - Principles and Pratice</a></td><td>413 Pages</td></tr>
<tr><td>44.</td><td><a target="_blank" href="https://mega.nz/file/SKAiwJxa#nu3Tm3jGmNunHmXmo4JfC42DlqFMppgvPTlD0ej_rkA">Nessus, Snort and Ethereal Power Tools</a></td><td>472 Pages</td></tr>
<tr><td>45.</td><td><a target="_blank" href="https://mega.nz/file/qLQkDDaT#xTwUl8VcecQrj7_R_HatjES5oeyVT-v0TbQlBEkHrk8">Active Defense - A Comprehensive Guide to Network Security</a></td><td>374 Pages</td></tr>
<tr><td>46.</td><td><a target="_blank" href="https://mega.nz/file/6DZQjTKa#X3pfvBocXuVnPdbX12X9vJMy3fFPf3JdRJP9fDDE6U0">Information Security Fundamentals</a></td><td>262 Pages</td></tr>
<tr><td>47.</td><td><a target="_blank" href="https://mega.nz/file/vGBGTZxT#NdoHXh5mnLFVk6e1_qtXiofBOId35IdhgZw-84f856E">Wireless Network Security</a></td><td>422 Pages</td></tr>
<tr><td>48.</td><td><a target="_blank" href="https://mega.nz/file/2PQAyBjI#C26PIIc3-vbTdX0LkULGKce4Pfn8Z7jlVxKYQJIYdSk">Red Hat Linux Security and Optimization</a></td><td>721 Pages</td></tr>
<tr><td>49.</td><td><a target="_blank" href="https://mega.nz/file/rGIkCTBI#ZCrYRdy5fXF6RwrDu8XsQoE0xXGkH88iTNcTg9Zlv6U">Windows Forensics Analysis</a></td><td>386 Pages</td></tr>
<tr><td>50.</td><td><a target="_blank" href="https://mega.nz/file/XeA0jLJa#9jGzTWQUVkyIHRKaSLH5ej6kiR6s0CKAsU76zuA32q4">Mobile and Wireless Network Security and Privacy</a></td><td>232 Pages</td></tr>
<tr><td>51.</td><td><a target="_blank" href="https://mega.nz/file/7fB0VLqY#LPhI_QegpdRxB_t1W4YuijNKYFFP94K2ThPBkEAw8Pc">Firewalls and Internet Security</a></td><td>456 Pages</td></tr>
<tr><td>52.</td><td><a target="_blank" href="https://mega.nz/file/KSImAZbL#2aXpT4q-ss7HKdjTuljomvQ4pwVOfCQ928MdWrFmCL0">An Introduction to Computer Security - The NIST Handbook</a></td><td>290 Pages</td></tr>
<tr><td>53.</td><td><a target="_blank" href="https://mega.nz/file/6PRQFD5D#k47HRaTvm0IOkHZqrFDwjah6wtOg35bGXuM38vpEXck">Unauthorized Access - Physical Penetration Testing for IT Security Teams</a></td><td>309 Pages</td></tr>
<tr><td>54.</td><td><a target="_blank" href="https://mega.nz/file/yTYmwJwC#XoUx3tZk7uX3WHY60YCLH0Qsvb_88QdpLl984LLnXgk">Testing Web Security</a></td><td>297 Pages</td></tr>
<tr><td>55.</td><td><a target="_blank" href="https://mega.nz/file/GeAiyLza#jenzhkq4xcn6M2fZ2RtSJYV_I52FRrDcnCG2HHVSSjE">Maximum Security - A Hacker's Guide to Protecting Your Internet Site and Network</a></td><td>670 Pages</td></tr>
<tr><td>56.</td><td><a target="_blank" href="https://mega.nz/file/rKRAURbS#7kBBxcTv8NRqaRiimLdxoqXORmnq8d5C0baVXQf4AVE">Information Resource Guide - Computer, Internet and Network Systems Security</a></td><td>325 Pages</td></tr>
<tr><td>57.</td><td><a target="_blank" href="https://mega.nz/file/ybQigTIR#2DaRXVbMiWQsog2xnVMX0ElX6YmyVImE9rqK64HB5PQ">The Hacker's Underground Handbook</a></td><td>116 Pages</td></tr>
<tr><td>58.</td><td><a target="_blank" href="https://mega.nz/file/nCIUSR5L#I41OmN3rv9n5ifBzrHoZ02DM2XoI-K3xJrilFxBctzY">Guide to SCADA and Industrial Control Systems Security</a></td><td>164 Pages</td></tr>
<tr><td>59.</td><td><a target="_blank" href="https://mega.nz/file/SHJk3ZCA#FVNddZM0-iP-WEQfQoCYCAp9YRYQXJcr6z6n4FfeRV0">The International Handbook of Computer Security</a></td><td>274 Pages</td></tr>
<tr><td>60.</td><td><a target="_blank" href="https://mega.nz/file/CXRC0BII#AGo4nnpU0JESKz3OmWZaq1rU4g6KC0GozwKFlBLY8do">The Code Book - How to Make It, Break It, Hack It, Crack It</a></td><td>273 Pages</td></tr>
<tr><td>61.</td><td><a target="_blank" href="https://mega.nz/file/vGREHD4J#Hnbv6rpt_R9Vbww3VGj2507gLHK_sdrz-9cv1eyj0Lk">Linux 101 Hacks</a></td><td>271 Pages</td></tr>
<tr><td>62.</td><td><a target="_blank" href="https://mega.nz/file/iDIgmJzS#hI1QQb-6eEa46XNpU1Wy8Erz6OWJD9VvyWw0E71h8Xg">Introduction to Linux - A Hands on Guide</a></td><td>223 Pages</td></tr>
<tr><td>63.</td><td><a target="_blank" href="https://mega.nz/file/zHYknB4b#5aeBTH-YmZeI_HlQSHil8CXKk38QFLJY3UTNWeA5UF4">Bluetooth Security</a></td><td>222 Pages</td></tr>
<tr><td>64.</td><td><a target="_blank" href="https://mega.nz/file/CbYCBDqK#eeKiqsxKtDPiGOcci26M1gB5AGBtu5P-iQCbuCKSfsU">IT Governance - A Manager's Guide to Data Security and ISO 27001/27002</a></td><td>385 Pages</td></tr>
<tr><td>65.</td><td><a target="_blank" href="https://mega.nz/file/6GJwlBAY#xdHC7XD5-yH839juAeihmmPjCQTY7tx7Up8Re5-x8jQ">Batch File Programming</a></td><td>155 Pages</td></tr>
<tr><td>66.</td><td><a target="_blank" href="https://mega.nz/file/ubZEgTSJ#7q1yWyxagK0a07qBYsDR3u1vC8IHPqmLF82qxL9TKg8">Cracking the Coding Interview</a></td><td>310 Pages</td></tr>
<tr><td>67.</td><td><a target="_blank" href="https://mega.nz/file/LCR0hJ4S#tzDutdj0jmhAA2CZkkQaQNw5EduFuCgAaHoe-F_ABy0">Dictionary of Networking</a></td><td>465 Pages</td></tr>
<tr><td>68.</td><td><a target="_blank" href="https://mega.nz/file/zOYSyBib#zxFJRXbRIWytm79bVKgEYPwjEf6Re5Km-OgBDwe9KHk">Hacking Gmail</a></td><td>310 Pages</td></tr>
<tr><td>69.</td><td><a target="_blank" href="https://mega.nz/file/TSYWAbba#aWtutgKTLfqFzQJcylqiofD0ax0est96Md2sxqEs90c">Linux Complete Command Reference</a></td><td>1528 Pages</td></tr>
<tr><td>70.</td><td><a target="_blank" href="https://mega.nz/file/eLJQzJwZ#C1h-JhJu-4IQK36hF3ZbU2cJpPZol2nSP-vt_eeSr48">Practical Hacking Techniques and Countermeasures</a></td><td>752 Pages</td></tr>
<tr><td>71.</td><td><a target="_blank" href="https://mega.nz/file/naRCFZRA#IoR3Q7iX680RdEFmIjllNFoLlBFxuJ7SR-L26W-yYg0">The Art of Intrusion by Kevin Mitnick</a></td><td>291 Pages</td></tr>
<tr><td>72.</td><td><a target="_blank" href="https://mega.nz/file/LHRADDQa#ShdnfmCy3cOCe3Mxzmo2fy3cbwul2XffCbc2DWHm_SY">Hack Notes - Windows Security Portable Reference</a></td><td>289 Pages</td></tr>
<tr><td>73.</td><td><a target="_blank" href="https://mega.nz/file/fDRG3TbA#Ut6N4uuAfTNDc7EEJnvqjGp9CBn-cDafT4dI48UzM5M">Hacking - The Next Generation</a></td><td>298 Pages</td></tr>
<tr><td>74.</td><td><a target="_blank" href="https://mega.nz/file/qDISDJYD#iFdVoIfY91zn4tlVsiDVgjC2XoLnge6Zy0_FaRpZSkw">Hacking the Cable Modem</a></td><td>330 Pages</td></tr>
<tr><td>75.</td><td><a target="_blank" href="https://mega.nz/file/7GRGiRRK#sg_WqSUwKcpYjWrmeERZHkxh8qK5cUUV0KBXEWo8ux4">Hackers Beware - Defending Your Network From The Wiley Hacker</a></td><td>817 Pages</td></tr>
<tr><td>76.</td><td><a target="_blank" href="https://mega.nz/file/7TRSRRjB#R7baBKxN7Y7WgNMd1AJu8Qe_VCsW6xuk5sTMhoZCmRU">Hack Proofing Your Network</a></td><td>826 Pages</td></tr>
<tr><td>77.</td><td><a target="_blank" href="https://mega.nz/file/6DAGAJzS#J4ui9cgeR-LU1GWYVyPjPOcSpdvKjmhY-NwI1qW-kb8">Hack Attacks Revealed</a></td><td>837 Pages</td></tr>
<tr><td>78.</td><td><a target="_blank" href="https://mega.nz/file/2OZCRZBJ#Dc20fhN8vX6Lhla2hkjdaGAPTf4Z6SIZsU9VgqoKLXo">Dissecting the Hack - The F0rb1dd3n Network</a></td><td>441 Pages</td></tr>
<tr><td>79.</td><td><a target="_blank" href="https://mega.nz/file/3aQGXB4b#Pzp2QuDtNQHMux7uqOEWf3Y6mCZVpvwfVuxFIlP2Gks">TCP/IP Guide</a></td><td>1671 Pages</td></tr>
<tr><td>80.</td><td><a target="_blank" href="https://mega.nz/file/vWZmwbxY#TsY57So4OXdyniAQdnmtajPBxZAXvsdXaPI3wl9zFYg">Offensive Security - Wireless Attacks - WiFu</a></td><td>385 Pages</td></tr>
<tr><td>81.</td><td><a target="_blank" href="https://mega.nz/file/yWRATJAb#z15nwhT4MsCvJAY0GxZBgQ2sglEgF0faAWDNid7pMxo">Google Hacking - For Penetration Testers</a></td><td>529 Pages</td></tr>
<tr><td>82.</td><td><a target="_blank" href="https://mega.nz/file/uTIWzLDS#7B6swnmDKJnKxkVCCF_y_bHGGgWmFoJNpjWQPLlsrgs">Computer Forensics Investigating Network Intrusions and Cyber Crime</a></td><td>394 Pages</td></tr>
<tr><td>83.</td><td><a target="_blank" href="https://mega.nz/file/ieYEQTaZ#BWMBUXPw77XN5ikocb61z21s54aeWmY3w73Q4kX5KZk">Hakin9 Bible</a></td><td>207 Pages</td></tr>
<tr><td>84.</td><td><a target="_blank" href="https://mega.nz/file/ODIkGbZQ#JO331oy2Dk-IkACgAQOaGGE26LX421QDTcgahMFlq1o">Network Forensics - Tracking Hackers Through Cyberspace</a></td><td>574 Pages</td></tr>
<tr><td>85.</td><td><a target="_blank" href="https://mega.nz/file/TKRkTJjB#82Vp2yxE0J2MSQ6iPDViLagrSti08ON6LT45HcSRQdw">Computer Forensics - Investigating Data and Image Files</a></td><td>227 Pages</td></tr>
<tr><td>86.</td><td><a target="_blank" href="https://mega.nz/file/qTISGbQZ#sD-gNbVyS_kh30hY4RP85p2e5fnmcA8gGkpc1TvNdx8">Penetration Testing and Network Defense</a></td><td>625 Pages</td></tr>
<tr><td>87.</td><td><a target="_blank" href="https://mega.nz/file/iSZWkLYB#5-xIqpaX3ZKlcWKDcKUvAiBlnhS0PJIcdE8JpQBy7cQ">Hacking Exposed - Malware and Rootkits</a></td><td>401 Pages</td></tr>
<tr><td>88.</td><td><a target="_blank" href="https://mega.nz/file/6HB0DRaR#YsRYTHeedcLohNpj8HmrIB86VZIRYd_MQIoOaUlhelk">Malware Analyst's Cookbook</a></td><td>746 Pages</td></tr>
<tr><td>89.</td><td><a target="_blank" href="https://mega.nz/file/nLRG3LAb#1J8CWb2F8QQ7tM2IoehHdj4d0zqtZC35BW4UhKntAIY">Mobile Malware - Attacks and Defense</a></td><td>386 Pages</td></tr>
<tr><td>90.</td><td><a target="_blank" href="https://mega.nz/file/abREkLaQ#VP02L9eUYydimUUecNgmfAGmy27lkKYCu3vd-2XBe4Y">Java 2 Network Security</a></td><td>702 Pages</td></tr>
<tr><td>91.</td><td><a target="_blank" href="https://mega.nz/file/zTZwAJwL#DIDP_AtW5044Ec7chE70SAcwDgjim1nP_-iCPhsVRr4">A Bug Hunter's Diary</a></td><td>212 Pages</td></tr>
<tr><td>92.</td><td><a target="_blank" href="https://mega.nz/file/2TZwUbSb#k54v8jyljDLp5UFit1a0wYdovy4l-t5hFXhdRGRA-Z4">Viruses Revealed - Understand and Counter Malicious Software</a></td><td>721 Pages</td></tr>
<tr><td>93.</td><td><a target="_blank" href="https://mega.nz/file/6CR2RZhA#rFBGgNWmQRrMbwuBbL4QlNUUtWJmaZ5hLzG7QrNvVAk">Figital Forensics With Open Source Tools</a></td><td>289 Pages</td></tr>
<tr><td>94.</td><td><a target="_blank" href="https://mega.nz/file/jWYQgBrC#vdRejQKWoOBB5ADpsciwODys4EszjWFNjTaltJcyQ7w">SSH, The Secure Shell - The Definitive Guide</a></td><td>438 Pages</td></tr>
<tr><td>95.</td><td><a target="_blank" href="https://mega.nz/file/WWBAHZYT#KuLXrn9rqzRxHVqygUSIkThb1HS0iHCDRRiuqNHLa9o">Pro PHP Security</a></td><td>369 Pages</td></tr>
<tr><td>96.</td><td><a target="_blank" href="https://mega.nz/file/SfJAEDKR#f9u2h1diOMm2b1eD00DdEF8EyVAdrIgzz4V_JHrqtTo">Zero Day Exploit - Countdown to Darkness</a></td><td>363 Pages</td></tr>
<tr><td>97.</td><td><a target="_blank" href="https://difl.host/ffa6915892383ac4/97._Metasploit_Penetration_Testing_Cookbook.pdf">Metasploit Penetration Testing Cookbook</a></td><td>269 Pages</td></tr>
<tr><td>98.</td><td><a target="_blank" href="https://mega.nz/file/6SY2wJhS#Tla1GsHPg6NzxdExbd03jK5--hr62-R_xG6aHaI4374">24 Deadly Sins of Software Securtiy</a></td><td>433 Pages</td></tr>
<tr><td>99.</td><td><a target="_blank" href="https://mega.nz/file/rLQCHZLA#hUk6UqVzfcfyPL3ftYx7HR6d9HNo7p8IdUQjNMlOCTQ">Botnets - The Killer Web App</a></td><td>482 Pages</td></tr>
<tr><td>100.</td><td><a target="_blank" href="https://mega.nz/file/OaIkUbbS#WXfTCl5-quuooEq1xf-MOtm3iMaDLOt8v9X3hTm4rA8">Hacker Highschool - Hack School for Beginners (ZIP)</a></td><td>12 Books</td></tr>
</table>

## OSCP Resources
- <a href="https://github.com/rewardone/OSCPRepo">OSCP Repo</a>
- <a href="https://www.netsecfocus.com/oscp/2019/03/29/The_Journey_to_Try_Harder-_TJNulls_Preparation_Guide_for_PWK_OSCP.html">TJnull OSCP Prep Guide</a>

<b>sumber :</b>
- <a href="https://github.com/johnazzam/Cyber-Security-Books">https://github.com/johnazzam/Cyber-Security-Books</a>
- <a href="https://github.com/yeahhub/Hacking-Security-Ebooks">https://github.com/yeahhub/Hacking-Security-Ebooks</a>
- <a href="https://github.com/screetsec/Cybersecurity-Indonesia">https://github.com/screetsec/Cybersecurity-Indonesia</a>
- <a href="https://github.com/an4kein/awesome-red-teaming">https://github.com/an4kein/awesome-red-teaming</a>
- <a href="https://github.com/fabacab/awesome-cybersecurity-blueteam">https://github.com/fabacab/awesome-cybersecurity-blueteam</a>