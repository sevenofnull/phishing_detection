# Phishing detection

Just for clarification, this will help to catch mass phishing emails.  
Not customized for you (your company).

If it looks like a duck,  
walks like a duck and  
sounds like a duck.  
Hover over the link...  
It's a phish.  

The list will be updated every now and then  

## Subject contains the following regex

### English
(S|s)hared\s(U|u)sing\s(O|o)ne(D|d)rive\s(F|f)or\s(B|b)usiness  
(S|s)ecurity(\s|-|\s-\s)?((A|a)lert|(W|w)arning|(I|i)nfo(rmation)?)  
((N|n)ew|(M|m)issed)\s(M|m)essage(s)?  
(C|c)urrently\son\shold  
(A|a)waiting\s(your\s)?further\s(A|a)ction(s)?  
(Y|y)ou\shave\s(a\s)?(some\s)?file(s)?  
((A|a)utomatic\s)?(P|p)assword\s(R|r)eset  
((N|n)ew\s)?(E|e)mail\son\s\d{2}(\/)?\d{2}\/\d{2}(\/)?\d{2}  
has\sbeen\slimited  
(W|w)e\shave\slocked  
has\sbeen\ssuspended  
(U|u)nusual\s((S|s)ign(-)?in\s)?(A|a)ctivity  
(Y|y)our\s(A|a)ccount\\s(has|was)  
(N|n)ew\s((R|r)ecorded\s)?(V|v)oice(\s)?(M|m)ail  
(P|p)assword(\s|\s-\s)(E|e)xpired  
(N|n)otifications(\s|\s-\s)(P|p)ending  
(A|a)ccount\s(is\s)?on\shold  
(V|v)erification(s)?\s((R|r)equired|(N|n)otification|(R|r)equest)  
temporar(il)?y\sdeactivated  
secure\supdate  
(S|s)ecure(-|\s)(E|e)?(M|m)ail  
(E|e)mployee\s(B|b)enefits\s(P|p)olicy
((E|e)-)?(M|m)ail\s(A|a)ccount\s(N|n)otice  

### French
(V|v)otre\scompte\sest\sbloqu(é|e)  

### Spanish
(D|d)etectamos\sum\s(P|p)roblema  

### German
(Ü|ü)berprüfung\serforderlich

### Swedish
(D|)u\shar\s\((\d+\)\s)?hållit\se(-)?postmeddelande(n)?

### Chinese
安全警报  
需要操作  
郵箱已滿  

## Mail-Body contains the following

/wp-admin/  
/wp-incude/  
\.xyz/  

## Mail-Body contains the following regex

### English
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
(W|w)(\s)?(i|\W|1)(\s)?((l|1)(\s)?){2}\s(\s)?(e|\W)(\s)?x(\s)?p(\s)?(i|\W|1)(\s)?r(\s)?(e|\W)(\s)?\s(\s)?(i|\W|1)(\s)?n(\s)?\s(\s)?\d(\s)?\s(\s)?(D|d)(\s)?(a|\W)(\s)?(y|\W)(\s)?(s)?  -> will expire in 2 days  

## Thanks
SwiftOnSecurity for the starting point
