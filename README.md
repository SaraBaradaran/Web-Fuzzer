# Wuzzer

## General info
> Simple Web Fuzzer
  1. **Crawling** : Collects All Internal URL ( [Crawler.py](https://github.com/mheidari98/Web-Fuzzer/blob/main/Wuzzer/Crawler.py) )
  2. Uses **Selenium** And **BeautifulSoup** to Detect Form & Input Params For Fuzzing
  3. Injects Payloads
  4. Checks Responses to Detect Vulnerabilities
---

## Requirements
- Python3
- Use Virtual Environments & Install Requirements Packages ([gist](https://gist.github.com/mheidari98/8ae29b88bd98f8f59828b0ec112811e7)) 
- Chrome Web Driver : Download It From The Address Below And Put It in The **Wuzzer** Folder
  ```
  Chrome:    https://sites.google.com/a/chromium.org/chromedriver/downloads
  ```

 ---

## Usage
  For Test on DVWA :
  ```bash
  cd Wuzzer
  python Wuzzer.py --test --XSSi --SQLi --BSQLi --CMDi --BCMDi 
  ```
  For More Options :
  ```bash
  python Wuzzer.py -h
  ```

---

## Test on [DVWA Docker](https://hub.docker.com/r/vulnerables/web-dvwa/)  
  + Run Image
    ```bash
    docker run --rm -it -p 80:80 vulnerables/web-dvwa
    ```
  + Database Setup
    > http://127.0.0.1/setup.php
  + Login with Default Credentials
    - Username: **admin**
    - Password: **password**

---

## Task-Lists
- [x] Xss Injection Attack
- [x] SQL Injection Attack
- [x] Blind SQL Injection Attack
- [x] Command Injection Attack
- [x] Blind Command Injection Attack
- [ ] Complete Document
- [ ] Threading Support
- [ ] Use Proxy

---

## Related Link 
### Vulnerable Web Applications
* OWASP Vulnerable Web Applications Directory ([github](https://github.com/OWASP/OWASP-VWAD)) ([owasp](https://owasp.org/www-project-vulnerable-web-applications-directory/))
* Web Vulnerability Collection ([github](https://github.com/lotusirous/vulnwebcollection)) 

### Payloads
* Cheatsheet_XSS_Vectors.txt ([Cheatsheet-God github](https://github.com/OlivierLaflamme/Cheatsheet-God/blob/master/Cheatsheet_XSS_Vectors.txt))
* XSS_Alert.txt ([PayloadsAllTheThings github](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/XSS%20Injection/Intruders/xss_alert.txt))
* SQL.txt ([wfuzz github](https://github.com/xmendez/wfuzz/blob/master/wordlist/Injections/SQL.txt))
* Blind_Sqli.txt ([sql-injection-payload-list github](https://github.com/payloadbox/sql-injection-payload-list/blob/master/Intruder/detect/Generic_TimeBased.txt))

### XSS
* Cross-Site Scripting (XSS) Cheat Sheet ([portswigger](https://portswigger.net/web-security/cross-site-scripting/cheat-sheet))
* XSS Injection ([PayloadsAllTheThings github](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/XSS%20Injection))
* Cross-Site Scripting (XSS) ([Resources-for-Beginner-Bug-Bounty-Hunters github](https://github.com/nahamsec/Resources-for-Beginner-Bug-Bounty-Hunters/blob/master/assets/vulns.md#cross-site-scripting-xss))

### Related Work
* Most Advanced XSS Scanner ([XSStrike](https://github.com/s0md3v/XSStrike)) 
* Automatic SQL Injection and database takeover tool ([sqlmap](https://github.com/sqlmapproject/sqlmap)) 
* Web Fuzzers Review ([pentestbook](https://pentestbook.six2dez.com/others/web-fuzzers-comparision))

### Security Game
* XSS Game By Google ([xss-game](https://xss-game.appspot.com))
* [xssgame](https://www.xssgame.com/)
* Alert(1) to Win ([alf.nu](https://alf.nu/alert1))
* Prompt(1) to Win ([prompt.ml](http://prompt.ml/0))
* Prompt("sibears") to Win ([xss school](http://xss.school.sibears.ru/easy/0))
