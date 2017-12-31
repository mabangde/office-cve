# office-exploit-case-study

All samples are malware used in the real world,please study them in virtual machine.Take responsibility yourself if you use them for illegal purposes.Samples should match hash in corresponding paper if mentioned.Exploits before 2010 not included.Feel free to open issues if you have any questions.

What did Microsoft do to make office more secure?
1.Data Execution Prevention in Office 2010
2.enforce ASLR randomization natively without any additional setting on Win7 and above, even for those DLLs not originally compiled with /DYNAMICBASE flag in Office 2013
3.disable EPS in 2017.4's patch
4.disable DDE in 2017.12's patch

CVE               |Type of Vuln                             |fix time|
------------------|-----------------------------------------|--------|
CVE-2010-3333|stack overflow in RTF parser|2010.11
CVE-2012-0158|stack overflow in ActiveX|2012.4
CVE-2013-3906|array out of bounds in TIFF parser|2013.12
CVE-2014-1761|array out of bounds in RTF parser|2014.4
CVE-2015-1641|type confusion in RTF parser|2015.4
CVE-2015-2545|use after free in EPS parser|2015.9
CVE-2016-7193|array out of bounds in RTF parser|2016.10
CVE-2017-0261/CVE-2017-0262|use after free&type confusion in EPS parser|2017.5
CVE-2017-8759|logic false in .NET Framework|2017.9
CVE-2017-11826|type confusion in OOXML parser|2017.10
CVE-2017-11882|stack overflow in EQNEDT32.EXE|2017.11

tools:

[offvis](https://blogs.technet.microsoft.com/srd/2009/07/31/announcing-offvis-1-0-beta/)

[oletools](https://github.com/decalage2/oletools)

[olefileview](https://0cch.com/2015/08/03/ole-file-view-tool/)

papers:

[How Malformed RTF Defeats Security Engines](http://blog.talosintelligence.com/2017/03/how-malformed-rtf-defeats-security.html)

[Attacking Interoperability An OLE Edition](https://www.blackhat.com/docs/us-15/materials/us-15-Li-Attacking-Interoperability-An-OLE-Edition.pdf)



