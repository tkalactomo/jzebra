(formerly jzebra)

# 1.8.7 Released.  Get it here: http://qzindustries.com/download #


# Notice:  Downloads have moved:  http://qzindustries.com/download ([why?](http://thenextweb.com/google/2013/05/22/google-codes-download-option-deprecated-due-to-misuse-only-existing-project-downloads-to-be-kept-after-january-15)) #

### <font color='red'>Java 7 Update 51 has been released.  <a href='https://www.java.com/en/download/manual.jsp'>https://www.java.com/en/download/manual.jsp</a></font> ###

### <font color='red'>OS X 10.8 users receiving <code>java.io.IOException: error=1</code>, please see <a href='https://code.google.com/p/jzebra/issues/detail?id=168'>Issue 168</a></font> ###

### <font color='red'>IIS Users, please read <a href='https://code.google.com/p/jzebra/issues/detail?id=171'>Issue 171</a></font> ###

### <font color='red'>A bulletin on Java 7 Update 45 <a href='http://qzindustries.com/j7u45'>http://qzindustries.com/j7u45</a></font> ###

```
<input type=button onClick="print()" value="Print">
<applet id="qz" name="QZ Print Plugin" code="qz.PrintApplet.class" archive="./qz-print.jar" width="100" height="100">
      <param name="printer" value="zebra">
</applet>

<script>
      function print() {
         var qz = document.getElementById('qz');
         qz.append('A37,503,0,1,2,3,N,PRINTED USING QZ-PRINT\n');
         // ZPLII
         // qz.append('^XA^FO50,50^ADN,36,20^FDPRINTED USING QZ-PRINT^FS^XZ');  
         qz.print();
      }
</script>
```

# Features #
  * **New!** Supports basic and **advanced** HTML labels directly to a LaserJet or PostScript compatible printer!
  * Supports Zebra, Epson, Citizen, Intermec printers and many more.
  * Prints barcodes, receipts and more from a web page.
  * Supports thermal printers, label printers, magnetic card printers
  * 100% free and [open source](http://www.gnu.org/licenses/gpl.html)
  * Free to use in commercial applications (check [license](http://www.gnu.org/licenses/gpl.html) for details)
  * Seamlessly sends commands to your EPL2, ZPLII, CHR, ASCII, RAW, ESC/P printer (and more).
  * Compatible with Windows, Mac OS X, Linux, Solaris clients (and more).
  * Tested with Firefox, Chrome, Safari, Internet Explorer, Opera.
  * Supports COM, parallel, serial, USB, socket, lpr, LPT communication.
  * AJAX compatible by using JavaScript to control print jobs

[![](http://jzebra.googlecode.com/files/download.png)](http://qzindustries.com/download)

[Download Latest](http://qzindustries.com/download)

---



# How It Works #
  1. First, QZ-PRINT loads in your web browser as a Java applet (similar to a Flash or SilverLight object).
  1. Second, QZ-PRINT interfaces with browser interactively via JavaScript.
  1. Third, QZ-PRINT gains permission to use locally installed printers via digital signature prompt.
  1. Finally, QZ-PRINT spools directly to locally installed printers, allowing hundreds of print jobs to transfer seamlessly from web code to printer.


---



# Getting Started #
  * Start using QZ-PRINT now by [downloading the latest version](http://qzindustries.com/download).
  * Learn QZ-PRINT's features step-by-step and how to integrate QZ-PRINT into your web project using the [developers guide](TutorialWebApplet.md).
  * Read more about purpose and the history of QZ-PRINT [here](About.md).
[![](http://jzebra.googlecode.com/files/tutorial.png)](http://code.google.com/p/jzebra/wiki/TutorialWebApplet)

  * For questions, feedback and updates, subscribe to the **jZebra Mailing List** on Google Groups:
> | [![](http://jzebra.googlecode.com/files/groups_logo_sm.gif)](http://groups.google.com/group/jzebra-users) |
|:----------------------------------------------------------------------------------------------------------|

---



# Configure Your Printer #
  * [Windows](TutorialRawXP.md):
[![](http://jzebra.googlecode.com/files/windows.png)](http://code.google.com/p/jzebra/wiki/TutorialRawXP#Introduction)
  * [Ubuntu](TutorialRawUbuntu.md):
[![](http://jzebra.googlecode.com/files/ubuntu.png)](http://code.google.com/p/jzebra/wiki/TutorialRawUbuntu#Introduction)
  * [Mac](TutorialRawOSX.md):
[![](http://jzebra.googlecode.com/files/mac.png)](http://code.google.com/p/jzebra/wiki/TutorialRawOSX#Introduction)


---



# Spotlight #
  * [ups-php](http://code.google.com/p/ups-php/) uses QZ-PRINT
  * [RocketShip.it](http://rocketship.it/) uses QZ-PRINT
  * [Reason Transport](http://www.reasontransport.com/) uses QZ-PRINT
  * [FedEx Developer Site](http://justtesting.biz/html/jzebra/jzdemo.html) uses QZ-PRINT
  * [Zenkraft.com](http://www.zenkraft.com) uses QZ-PRINT
  * [Store4Schools](http://store4schools.com) uses QZ-PRINT
  * Pegadaian SSIS/SDM ![http://www.wahyudiharto.com/blog_images/i_pegadaian.gif](http://www.wahyudiharto.com/blog_images/i_pegadaian.gif) [![](http://www.wahyudiharto.com/blog_images/i_sissdm.gif)](http://sdm.pegadaian.co.id/sdm/) uses QZ-PRINT
  * [Gamera Software S.R.L](http://bdemo.no-ip.biz:60000) uses QZ-PRINT
  * SoftCaribe S.A. uses QZ-PRINT
[![](http://jzebra.googlecode.com/files/bottom.png)](http://code.google.com/p/jzebra/wiki/ScreenShots)



---


# Update History #
  * `08/03/2013:` Version 1.5.3 Adds new EPL image handling (non-8-by pixels widths corrected too),  HTML fix for Java 7 Update 25, raw data uses byte[.md](.md), misc code cleanup.
  * `04/19/2013:` Version 1.4.7 fixes a bug with the Java 7 u21 update that throws "NPObject" errors.  This is due to Liveconnect not allowing trusted/untrusted code to execute side-by-side.  See [issue 126](https://code.google.com/p/jzebra/issues/detail?id=126) for more details.
  * `08/28/2012:` Version 1.4.5 sample.html improvements, image scaling/flipping support for PostScript printing, New improved HTML printing feature for HTML5 capable browsers.
  * `06/26/2012:` Version 1.4.3 Fixes with append64() NullPointerException, appendImage(url, "ZPLII") incorrectly using EPL commands.  Source for sample.html has hints for new jzebraDoneFinding, jzebraDoneAppending, jzebraDonePrinting helpers.
  * `03/15/2012:` Version 1.4.1 Adds find/set printer fixes as well as much needed browser readiness features.
  * `03/15/2012:` Version 1.3.5 Fixes some weird behavior when RegEx characters "(){}" are used with findPrinter().  Also built against JDK 1.5, since 1.3.4 was rushed against JDK 1.6 and may have broken some backwards compatibility.
  * `03/13/2012:` Version 1.3.4 Adds HTML printing support for LaserJets, InkJets, DeskJets, etc.  Also attempts to fix a print margin bug with PDFs.  See sample.html for more info.
  * `02/22/2012:` Version 1.2.3 Includes experimental image printing, including base64 printing for ZPLII capable printers.
  * `02/09/2012:` Version 1.2.1 Fixes a problem in sample.html with "List All" printers.
  * `11/09/2011:` [Version 1.1.9](http://code.google.com/p/jzebra/downloads/detail?name=jZebra%201.1.9.zip&can=2&q=#makechanges) adds experimental PDF printing, support for printing directly to file (i.e. \\server\printer)
  * `01/30/2011:` Front page & logo redesign
  * `01/12/2011:` Version 1.1.1 available (not featured, see downloads).  Adds a new `appendFile()` feature similar to original 1.0.3 and older functionality `CONFIGPATH="http://site/epl.txt"`.
  * `01/08/2011:` Version 1.1.0 available.  Fixes XML parsing error discovered in Internet Explorer.  Please note, the JavaScript in sample.html has timing improvements added in lieu.
  * `01/07/2011:` Version 1.0.9 available.  Adds experimental [Cp1252](http://en.wikipedia.org/wiki/Windows-1252) support, [XML message parsing](http://code.google.com/p/jzebra/wiki/TutorialWebApplet#XML_Printing) support.
  * `12/08/2010:` Version 1.0.7 available for improved digital signature support.  Versions 1.0.7 and higher will use the same trusted java signature: see source:/jzebra.ks.
  * `11/20/2010:` Version 1.0.6 available for download.  Added feature that allows larger print jobs to be spooled as separate jobs to the printer. (Example, every 5 labels spools a new print job)
  * `01/06/2010:` An excellent article ["RAW Printing from Web Based Application"](http://paparadit.blogspot.com/2010/06/raw-printing-from-web-based-application.html)
  * `04/13/2010:` Version 1.0.5 available for download.  Fixed "Magic Cookie" issue thank to James at ZenKraft.
  * `12/03/2009:` Updated applet tutorial for version 1.0.4.
  * `11/19/2009:` Version 1.0.4 available for download.  Note:  Code changes will need to be made to incorporate new version!!
  * `11/07/2009:` Uploaded more [screenshots](ScreenShots.md) for Ubuntu 9.10 and Windows XP.
  * `11/06/2009:` [Raw Printing from Mac OSX](TutorialRawOSX.md) created in [wiki](http://code.google.com/p/jzebra/w/list) section
  * `10/24/2009:` [ReasonTransport](http://reasontransport.com) to test Bluetooth printing capabilities
  * `01/09/2009:` [TutorialWebApplet](TutorialWebApplet.md) added to [wiki](http://code.google.com/p/jzebra/w/list) for 1.0.3 usage
  * `12/30/2008:` jZebra 1.0.3 pre-release avaiable:  Check the [downloads](http://qzindustries.com/download).
  * `11/07/2008:` jZebra 1.0.3 under development:  Check [SVN](http://code.google.com/p/jzebra/source/checkout) if curious.
  * `11/06/2008:` Added 1.0.2 Bugs/Issues: [click to review issues](http://code.google.com/p/jzebra/issues/list)


---




### Printers Reported Working ###
  * Samsung Bixolon SRP350plus
  * Telly Dascom 1125 (USB)
  * Epson Thermal Printer (COM)
  * Eltron P310i
  * Zebra GK420d
  * Zebra P310i
  * Zebra LP 2844
  * Zebra TLP2844
  * Citizen CT-S2000 (USB)
  * DOS/LPT1 Printing
  * Print directly to file:  i.e. \\server\printer
  * Nippon Primex
  * Essae PR-85j
  * Bematech MP200
### Printers that WILL NOT WORK ###
  * Zebra ZXP3

Related projects:
http://code.google.com/p/ups-php/
http://code.google.com/p/zxing/
http://www.google.com/chrome/intl/en/p/cloudprint.html
http://code.google.com/p/escprinter/

Keywords:
page description language (PDL), zpl, pcl, prn, txt, ps, eps, epl, cpcl, esim, direct, ESC k, ESC p, ESC/P, OPOS, Epson Standard Code for Printers, &H1B, HEX, (1BH), CHR(27), ESC, ASCII, CHR$, BASIC, Cloud Printing, Metapace, SLCS, PHP, ASP.NET, print dos characters from web browser, dymo, okidata, avery label printer, EasyCoder PD4, OPOS Commands, Print PRN files from web browser, fromcharcode, java, javascript, ajax, jquery, COM1, COM2, COM3, LPT1, LPT2, Virtual Serial Port, VSPE, Star TSP, Star printer, gwt, detect printer java web, print directly to the printer from applet, vbtab, vbnewline, Intermec,IBM Proprinter,EPCL,Eltron Privilege Command Language,COPY "FILENAME.TXT" LPT1, COPY "FILENAME.TXT" COM1, DOS COPY, DOS MODE, DOS LPT1, CPL (Cognitive Printing Language), CUSTOM PRINTERS, custom.biz, VKP80II, BOCA, FGL, Friendly Ghost Language (FGL), bixolon, bxl, bxl/pos, bxl / pos programming guide