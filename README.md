# Phishing detection

Just for clarification, this will help to catch mass phishing emails.  
Not customized for you (your company).

If it looks like a duck,  
walks like a duck and  
sounds like a duck.  
Hover over the link...  
It's a phish.  

The list will be updated every now and then  

Splitt the list now into different files and add different version.

Elementary:  
Intermediate:   
Advanced:  

## Sender contains the following regex

### Sender moved to folder sender/sender.txt

## Subject contains the following regex

### English moved to folder subject/subject-english.txt

### French
##### votre compte est bloqué (your account is blocked)
(V|v)(o|\W)tr(e|\W)\sc(o|\W)mpt(e|\W)\s(e|\W)(s|\W)t\sbl(o|\W)q(u|\W)(e|\W)
##### Vous avez reçu 1200 (You received 1200)
(V|v)(o|\W)(u|\W)(s|\W)\s(a|\W)v(e|\W)z\sr(e|\W)(c|\W)(u|\W)\s\d+

### Spanish
##### detectamos um problema (we detected a problem)
(D|d)(e|\W)t(e|\W)ct(a|\W)m(o|\W)(s|\W)\s(u|\W)m\s(P|p)r(o|\W)bl(e|\W)m(a|\W) 

### German
##### Überprüfung erforderlich (Review required)
(U|u|\W)b(e|\W)rpr(u|\W)f(u|\W)ng\s(e|\W)rf(o|\W)rd(e|\W)rl(i|\W)ch

### Swedish
##### Du har 5 hållit epostmeddelanden (You have 5 emails)
(D|d)(u|\W)\sh(a|\W)r\s((\d+)\s)?h(a|\W)ll(i|\W)t\se(-)?p(o|\W)(s|\W)tm(e|\W)dd(e|\W)l(a|\W)nd(e|\W)(n)?  

### Chinese
##### Security alert
安全警报
##### Need to operate
需要操作
##### Mailbox full
郵箱已滿  

## Mail-Body contains the following

/wp-admin/  
/wp-incude/  
\.xyz/  

## Mail-Body contains the following regex

### Vulnerability Outlook (replacing links with double href and img in between)
https://isc.sans.edu/diary/Broken+phishing+accidentally+exploiting+Outlook+zero-day/26254  
```
(href|HREF)\=\"(http|HTTP)(s|S)?\:(\/){2}.*?\"\>\<(img|IMG)\>\<\/(a|A)\>\<(a\shref|A\sHREF)\=\"(http|HTTP)
```

### English
##### Update your account record
((u|\W)pd(a|\W)t(e|\W)d\s)?y(o|\W)(u|\W)r\s(a|\W)cc(o|\W)(u|\W)nt\sr(e|\W)c(o|\W)rd
##### suspicious activity
(s|\W)(u|\W)(s|\W)p(i|\W)c(i|\W)(o|\W)(u|\W)s\s(a|\W)ct(i|\W)v(i|\W)t(y|ies|(i|\W)(e|\W)(s|\W))
##### blocked your online
bl(o|\W)ck(e|\W)d\s(y(o|\W)(u|\W)r\s)?(o|\W)nl(i|\W)n(e|\W)
##### sign in with your email address
sign\sin\S{0,7}(\swith)?\syour\semail\saddress
##### Securely (whatever) OneDrive,dropbox Google Drive
(S|s)ecurely\s\S{0,7}(\sto)?(\s)?one(\s|-)?drive  
(S|s)ecurely\s\S{0,7}(\sto)?(\s)?drop(\s|-)?box  
(S|s)ecurely\s\S{0,7}(\sto)?(\s)? (G|g)oogle(\s|-)?(D|d)rive  
##### Will expire in 4 Days (also W i l l  e x p i r e  i n  4  d a y s)
(W|w)(\s)?(i|\W|1)(\s)?((l|1)(\s)?){2}\s(\s)?(e|\W)(\s)?x(\s)?p(\s)?(i|\W|1)(\s)?r(\s)?(e|\W)(\s)?\s(\s)?(i|\W|1)(\s)?n(\s)?\s(\s)?\d(\s)?\s(\s)?(D|d)(\s)?(a|\W)(\s)?(y|\W)(\s)?(s)?
##### docs.google[.]com/document  
docs\.google\.com\/document\/\w\/\w\/\d\w+\-\w+(\-)?\w+\/pub
##### Others
(Y|y)our\s(A|a)pple(\s|-)?(I|i)(D|d)\swas\sused\sto\ssign(\s|-)in\sto  
that\syou\svalidate\syour\s(\w+(-\w+)?\s)?(A|a)ccount  
(I|i)nformations\shas\sbeen  
(C|c)onfirm\syour\s(I|i)nformations  
(F|f)ailed\sto\svalidate  
(U|u)nable\sto\sverify  
(A|a)ctivate\syour\s(\w+(-\w+)?\s)?(A|a)ccount  
(U|u)pdate\syour\spayment  
(M|m)ultiple\slogin\sattempt  
(T|t)rying\sto\saccess\syour\s(\w+(-\w+)?\s)?(A|a)ccount  
restricted\sif\syou\sfail\sto\supdate  
update\sin\sour\ssecurity  
update\syour\s(\w+(-\w+)?\s)?(A|a)ccount\s(I|i)nformation  
has\sfailed\sto\sload  


### SCAM 
##### Bitcoin (if you have no business with crypto-currencies)
[13][a-km-zA-HJ-NP-Z1-9]{25,34}\\s and ((B|b)itcoin|BTC)


## Thanks
@SwiftOnSecurity for the starting point  
@packet_Wire for the motivation
