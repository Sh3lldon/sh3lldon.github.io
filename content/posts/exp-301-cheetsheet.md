+++
title = 'EXP-301 Cheetsheet'
date = 2024-08-23T18:01:41+05:00
draft = false
tags = ["EXP-301", "OSED", "OffSec"]
categories = ["Cheatsheet"]
+++
## Links
[Prep](#prep)🔗\
[Tools](#tools)🔗\
[Scripts](#scripts)🔗\
[Vanilla buffer overflow](#vanilla-buffer-overflow)🔗\
[SEH](#seh)🔗\
[Egghunter](#egghunter)🔗\
[Shellcoding](#shellcoding)🔗\
[DEP](#dep)🔗\
[ASLR](#aslr)🔗

## Prep
- [EXP-301 syllabus](https://www.offsec.com/documentation/EXP301-syllabus.pdf)
- [EXP-301 some open-free materials](https://github.com/CyberSecurityUP/OSCE3-Complete-Guide#osed)
- [Corelan free exploit development articles](https://www.corelan.be/index.php/articles/)
- [x86 Architecture](https://docs.microsoft.com/en-us/windows-hardware/drivers/debugger/x86-architecture)
- [x86 Assembly course](https://www.udemy.com/course/x86-assembly-programming-from-ground-uptm/)
- [Intro to Reversing (Beginners)](https://youtube.com/playlist?list=PLMB3ddm5Yvh3gf_iev78YP5EPzkA3nPdL)
- [Reversing training by Ricardo Narvaja](http://ricardonarvaja.info/WEB/EXPLOITING%20Y%20REVERSING%20USANDO%20HERRAMIENTAS%20FREE/INGLES/)
- [Exploit-DB](https://www.exploit-db.com/)
- [Vulnserver (github)](https://github.com/stephenbradshaw/vulnserver)
- [Vulnserver (blog)](https://fluidattacks.com/blog/tags/vulnserver/)
- [Tryhackme BOF Prep room](https://tryhackme.com/room/bufferoverflowprep)
- [Tryhackme Brainstorm room](https://tryhackme.com/room/brainstorm)
- [Tryhackme Brainpan 1 room](https://tryhackme.com/room/brainpan)
- [Tryhackme Gatekeeper room](https://tryhackme.com/room/gatekeeper)


## Tools
- [WinDdb](https://developer.microsoft.com/zh-tw/windows/downloads/windows-sdk/) : debugger
- [WinDdb cheatsheet](https://blog.lamarranet.com/wp-content/uploads/2021/09/WinDbg-Cheat-Sheet.pdf) : windbg user mode cheat sheet
- [WinDdb themes](https://github.com/lololosys/windbg-theme) : dark and white themes
- [Pykd](https://github.com/Sh3lldon/EXP-301-cheat-sheets) : allowing to deploy Python scripts
- [Mona.py](https://github.com/corelan/mona) : multiple task solution tool
- [Narly](https://code.google.com/archive/p/narly/) : displaying protection of each module
- [IDA](https://hex-rays.com/) : disassembler
- [rp++](https://github.com/0vercl0k/rp) : displaying gadgets for ROP chain
- [Ropper](https://github.com/sashs/Ropper) : displaying gadgets for ROP chain
- [TCPView](https://learn.microsoft.com/en-us/sysinternals/downloads/tcpview) : show TCP and UPD endpoints
- [code_caver](https://github.com/nop-tech/code_caver) : python script that finds code caves for your exploit

## Scripts
- [Scripts from epi052](https://github.com/epi052/osed-scripts)
- [Scripts from sebastian93921](https://github.com/sebastian93921/OSED-Code-Snippets)
- [Scripts from bugzzzhunter](https://github.com/bugzzzhunter/OSEDscripts)

## Vanilla Buffer Overflow
>  **Writeups**
- [Stack BOF part 1](https://www.corelan.be/index.php/2009/07/19/exploit-writing-tutorial-part-1-stack-based-overflows/) by corelan
- [Stack BOF part 2](https://www.corelan.be/index.php/2009/07/23/writing-buffer-overflow-exploits-a-quick-and-basic-tutorial-part-2/) by corelan
- [Vulnserver TRUN](https://fluidattacks.com/blog/vulnserver-trun/) by fluidattacks
- [BOF prep Tryhackme](https://infosecwriteups.com/tryhackme-oscp-buffer-overflow-prep-overflow-1-19e000482f27) by infosecwriteups
- [Brainstorm](https://steflan-security.com/tryhackme-brainstorm-walkthrough/) by steflan-security
- [Brainpan1](https://dorian5.medium.com/tryhackme-com-brainpan-1-walkthrough-3c9648a18c31) by medium
- [Gatekeeper](https://steflan-security.com/tryhackme-gatekeeper-walkthrough/) by steflan-security

> **Binaries**
- [Tryhackme BOF Prep room](https://tryhackme.com/room/bufferoverflowprep)
- [Tryhackme Brainstorm room](https://tryhackme.com/room/brainstorm)
- [Tryhackme Brainpan 1 room](https://tryhackme.com/room/brainpan)
- [Tryhackme Gatekeeper room](https://tryhackme.com/room/gatekeeper)
- [Vulnserver (github)](https://github.com/stephenbradshaw/vulnserver)
- [MiniShare 1.4.1](https://www.exploit-db.com/apps/9fceb6fefd0f3ca1a8c36e97b6cc925d-PCMan.7z)
- [PCMan FTP server 2.0.7](https://www.exploit-db.com/apps/9fceb6fefd0f3ca1a8c36e97b6cc925d-PCMan.7z)
- [Freefloat FTP server 1.0](https://www.exploit-db.com/apps/687ef6f72dcbbf5b2506e80a375377fa-freefloatftpserver.zip)
- [VUPlayer 2.49](https://www.exploit-db.com/apps/39adeb7fa4711cd1cac8702fb163ded5-vuplayersetup.exe)

## SEH
> **Writeups**
- [SEH Buffer Overflow](https://shelldonsblog.wixsite.com/blog/post/seh-buffer-overflow) by Shelldon
- [SEH Based Exploits](https://www.corelan.be/index.php/2009/07/25/writing-buffer-overflow-exploits-a-quick-and-basic-tutorial-part-3-seh/) by corelan
- [SEH Based Exploits](https://www.corelan.be/index.php/2009/07/28/seh-based-exploit-writing-tutorial-continued-just-another-example-part-3b/) by corelan (another example)
- [SEH Exploitation](http://www.securitysift.com/windows-exploit-development-part-6-seh-exploits/) by Securitysift
- [SEH Exploitation](http://www.fuzzysecurity.com/tutorials/expDev/3.html) by Fuzzysecurity
- [SEH Exploitation](https://www.shogunlab.com/blog/2017/11/06/zdzg-windows-exploit-4.html) by Shogun Lab
- [Kevin PG practice](https://youtu.be/wwyoh2kEO9I) by xct
- [UT99 PG practice](https://youtu.be/sLXhzxiLZ4U) by xct (another example)

> **Binaries**
- [Millenium MP3 Studio 2.0](https://www.exploit-db.com/apps/3c35dc3d6067fcc50f118500eb116c0b-millennium1.exe)
- [Free MP3 CD Ripper 2.6](https://www.exploit-db.com/apps/64215b82be8bb2e749f95fec5b51d3e4-FMCRSetup-2.6.exe)
- [Easy AVI DivX Converter 1.2.2.4](https://www.exploit-db.com/apps/5ad3e3560df85ecf6622fe3c58fb0c35-easy_avi_converter.exe)
- [My Video Converter 1.5.24](https://www.exploit-db.com/apps/0c966e74828582db6029aee6dc59bbd5-my_video_converter.exe)
- [VeryPDF Image2PDF Converter](https://www.exploit-db.com/apps/3ef2cd6c64e6d94c90c907311fb49710-img2pdf.exe)
- [ASX to MP3 Converter 3.1.2.1](https://www.exploit-db.com/apps/b31a84e79d9941d89336b6708ef52a20-ASXtoMP3Converter_3121.exe)
- [Vulnserver (GMON)](https://github.com/stephenbradshaw/vulnserver)
- [EFS Easy Chat Server 3.1](https://www.exploit-db.com/apps/c682138ebbea9af7948a3f142bbd054b-ecssetup.exe)
- [Easy File Sharing Web Server 7.2](https://www.exploit-db.com/apps/60f3ff1f3cd34dec80fba130ea481f31-efssetup.exe)
- [freeFTPD 1.0.10](https://www.exploit-db.com/apps/f7915612721b0e8dad57bdfcb29ac9bb-freeFTPd.exe)
- [FathFTP 1.8](https://www.exploit-db.com/apps/2bc586294ef5b2e4c9972152ff3bd696-fttsetup1.8.exe)
- [File Sharing Wizard 1.5.0](https://www.exploit-db.com/apps/da3a3626f99a85f9ab59ab77f083ff80-fs-wizard-setup.exe)
- [Easy Address Book Web server 1.6](https://www.exploit-db.com/apps/69f77623bb32589fb5343f598b61bbd9-eabws.exe)

## Egghunter
> **Writeups**
- [Win32 Egg hunting](https://www.corelan.be/index.php/2010/01/09/exploit-writing-tutorial-part-8-win32-egg-hunting/) by corelan
- [WoW64 Egghunter](https://www.corelan.be/index.php/2011/11/18/wow64-egghunter/) by corelan
- [Egghunter Exploitation](http://www.hick.org/code/skape/papers/egghunt-shellcode.pdf) by Skape
- [Locating Shellcode with egghunting](http://www.securitysift.com/windows-exploit-development-part-5-locating-shellcode-egghunting/) by Securitysift
- [Egghunters](http://www.fuzzysecurity.com/tutorials/expDev/4.html) by Fuzzysecurity
- [Egghunter](https://www.shogunlab.com/blog/2017/09/02/zdzg-windows-exploit-3.html) by shogunlab

> **Binaries**
- [docPrint Pro 8.0](https://www.exploit-db.com/apps/560e231d212fdaef8e52471f94a5f014-docprint_pro_setup.exe)
- [Foxit Reder 4.1.1](https://www.exploit-db.com/apps/c45f09020652e1111f83c8c8bce35427-FoxitReader411_enu_Setup.exe)
- [Audacity 1.2](https://www.exploit-db.com/apps/d59f24b86431eeb25281bce7817783f1-audacity-win-1.2.6.exe)
- [MiniShare 1.5.5](https://www.exploit-db.com/apps/90a8c5b447f3867d1d22cb599ed17b59-minishare-1.5.5.zip)
- [Free Mp3 CD Ripper 2.8](https://www.itusoft.com/download/FMCRSetup.exe)
- [Base64 Decoder 1.1.2](https://www.exploit-db.com/apps/743169f20b96c32da77e5ff7129e54db-b64dec-1-1-2.zip)
- [KiTTY Portable 0.65.0.2p](https://www.exploit-db.com/apps/ab56d0b1672747878d5325afa9c46c74-KiTTYPortable_0.65.0.2_English.paf.exe)
- [IP-Tools 2.5](https://www.exploit-db.com/apps/4a83348f18a18ba34f9747648b550307-ip-tools.exe)
- [Vulnserver (GTER, GMON, KSTET)](https://github.com/stephenbradshaw/vulnserver)
- [Easy File Sharing Web Server 7.2](https://www.exploit-db.com/apps/60f3ff1f3cd34dec80fba130ea481f31-efssetup.exe)
- [TFTP Server 1.4](https://www.exploit-db.com/apps/f07b073307052ccfb02fe1af243bb229-tftpserverspV1.4.tar.gz)
- [MinaliC WebServer 2.0.0](https://www.exploit-db.com/apps/2b0e04c048c9b84b12f742ae38136de6-minalic.zip)
- [Sysax Multi Server 5.52](https://www.exploit-db.com/apps/7b5ab39544fb296c05c6ea19ca5a3bad-sysaxserv_setup5.52.msi)
- [Savant Web Server 3.1](https://www.exploit-db.com/apps/08e770b173aa41be27db2304ac0df846-Savant31.exe)

## Shellcoding
> **Writeups**
- [Intro to win32 shellcoding](https://www.corelan.be/index.php/2010/02/25/exploit-writing-tutorial-part-9-introduction-to-win32-shellcoding/) by corelan
- [Understanding Win shellcode](http://www.hick.org/code/skape/papers/win32-shellcode.pdf) by skape
- [Writing small shellcode](https://research.nccgroup.com/wp-content/uploads/2020/07/writing_small_shellcode.pdf) by Dafydd Stuttard
- [Writig shellcode encoders](https://www.ired.team/offensive-security/code-injection-process-injection/writing-custom-shellcode-encoders-and-decoders) and decoders by ired.team
- [Writing W32 shellcode](https://www.fuzzysecurity.com/tutorials/expDev/6.html) by FuzzySecurity
- [Writing Messagebox shellcode](https://marcosvalle.github.io/re/exploit/2019/01/19/messagebox-shellcode.html) by marcosvalle
- Writing Win x32 manual shellcode [part 1](https://marcosvalle.github.io/re/exploit/2018/10/20/windows-manual-shellcode-part1.html) && [part 2](https://marcosvalle.github.io/re/exploit/2018/10/21/windows-manual-shellcode-part2.html) && [part 3](https://marcosvalle.github.io/re/exploit/2018/10/21/windows-manual-shellcode-part3.html) by marcosvalle

> **Socket reuse technique**
- [WS32_recv()](https://connormcgarr.github.io/WS32_recv()-Reuse/) resuse by Connor McGarr
- [Vulnserver](https://zflemingg1.gitbook.io/undergrad-tutorials/walkthroughs-osce/vulnserver-gter-command) - GTER by Zachary Fleming
- [Socket Reuse](https://shelldonsblog.wixsite.com/blog/post/stack-buffer-overflow-socket-reuse) by Shelldon
- [Writing a stager](https://guidedhacking.com/threads/binary-exploit-development-3-writing-an-exploit-stager.20067/) by nop

## DEP
> **Writeups**
- [Understanding DEP](https://fluidattacks.com/blog/understanding-dep/) by fluidattacks
- [Bypassing DEP with ROP](https://fluidattacks.com/blog/bypassing-dep/) by fluidattacks
- [Bypassing DEP with VirtualAlloc](https://shelldonsblog.wixsite.com/blog/post/bypassing-dep-with-virtualalloc-pushad-method) (PUSHAD method) by Shelldon
- [Bypassing DEP with VirtualProtect](https://shelldonsblog.wixsite.com/blog/post/bypassing-dep-with-custom-rop-chain-virtualprotect) by Shelldon
- [Bypassing DEP with WriteProcessMemory](https://guidedhacking.com/threads/exploit-development-5-dep-bypass-with-writeprocessmemory.20164/) by nop
- [Write a ROP decoder](https://guidedhacking.com/threads/binary-exploit-development-6-writing-a-rop-decoder.20184/) by nop
- [Changing DEP with ROP](https://www.corelan.be/index.php/2010/06/16/exploit-writing-tutorial-part-10-chaining-dep-with-rop-the-rubikstm-cube/) by corelan

> **Binaries**
- [RemoteApp](https://github.com/Sh3lldon/RemoteApp) by Shelldon
- [QuoteDB](https://github.com/bmdyy/quote_db) by bmdyy
- [Signatus](https://github.com/bmdyy/signatus) by bmdyy
- [Rainbow 1 and 2](https://github.com/xct/vulnbins) by xct
- [Easy File Sharing Web Server 7.2](https://www.exploit-db.com/apps/60f3ff1f3cd34dec80fba130ea481f31-efssetup.exe) by xct
- And other binaries (You need to turn on Data Execution Prevention in your VM)

## ASLR
> **Writeups**
- [Bypassing stack cookies, SafeSEH, SEHOP, HW, DEP and ASLR](https://www.corelan.be/index.php/2009/09/21/exploit-writing-tutorial-part-6-bypassing-stack-cookies-safeseh-hw-dep-and-aslr/) by corelan
- [Universal DEP/ASLR bypassing with msvcr71.dll and mona.py](https://www.corelan.be/index.php/2011/07/03/universal-depaslr-bypass-with-msvcr71-dll-and-mona-py/) by corelan
- [Bypassing ASLR/DEP](https://www.exploit-db.com/docs/english/17914-bypassing-aslrdep.pdf) by Vinay Katoch

> **Binaries**
- [RemoteApp](https://github.com/Sh3lldon/RemoteApp) by Shelldon
- [QuoteDB](https://github.com/bmdyy/quote_db) by bmdyy
- [Signatus](https://github.com/bmdyy/signatus) by bmdyy
- [Rainbow 1 and 2](https://github.com/xct/vulnbins) by xct
- [CoolPlayer+ Portable 2.19.6](https://www.exploit-db.com/apps/e9d68d1ad9873339d6ef0fd5a2e1f0bd-CoolPlayerPlusPortable_2.19.6.paf.exe)
- [CoolPlayer+ Portable 2.19.12](https://www.exploit-db.com/apps/f23274df165e69006a1fca2e06aeae29-CoolPlayerPlusPortable_2.19.2.paf.exe)
- [BlazeDVD 6.1](https://www.exploit-db.com/apps/1c3c56049cc1d722825c5d7635b51029-BlazeDVD_50_Professional_TRIAL.exe)
- [BlazeDVD 5.1](https://www.exploit-db.com/apps/1c3c56049cc1d722825c5d7635b51029-BlazeDVD_50_Professional_TRIAL.exe)
- [Simple Web Server 2.2-rc2](https://www.exploit-db.com/apps/142ba80cfca8f99ac36c92535728844c-sws-2.2-rc2-i686.exe)