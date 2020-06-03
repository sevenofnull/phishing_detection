# Phishing detection

Just for clarification, this will help to catch mass phishing emails.  
Not customized for you (your company).

If it sounds like a duck,  
walk like a duck and  
sounds like a duck.  
Hover over the link...  
It's a phish.  

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

### Chinese
安全警报  
需要操作  
郵箱已滿  


## Mail-Body contains the following regex

Working on it

