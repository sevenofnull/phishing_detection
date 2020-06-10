# Phishing detection

Just for clarification, this will help to catch mass phishing emails.  
Not customized for you (your company).

If it looks like a duck,  
walks like a duck and  
sounds like a duck.  
Hover over the link...  
It's a phish.  

The list will be updated every now and then  

## Sender contains the following regex

##### will catch @m1crosoft or g0ogle or @c0mpany or @your-c0mpany  
```
@([a-z]+[01]([01])?[a-z]+|[a-z]+\-[a-z]+[01]([01])?[a-z]+)
```

## Subject contains the following regex

### English
##### shared using onedrive for business  
(S|s|\W)h(a|\W)r(e|\W)d\s(U|u|\W)s(i|\W)ng\s(O|o|\W)n(e|\W)(\s)?(D|d)r(i|\W)v(e|\W)\s(F|f)(o|\W)r\s(B|b)(u|\W)(s|\W)(i|\W)n(e|\W)(s|\W)(s|\W)?
##### Security - Alert or Security Alert or Security Warning or Security Info or Security - Information
(S|s|\W)(e|\W)(c|\W)(u|\W)r(i|\W|1)t(y|\W)((\s)?|-|(\s)?-(\s)?)?((A|a|\W)(l|1)(e|\W)rt|(W|w|\W)(a|\W)rn(i|\W|1)ng|(I|i|1|\W)nf(o|\W)(rm(a|\W)t(i|\W|1)(o|\W|0)n)?)
##### New Messages or Missed Message
((N|n)(e|\W)w\s|(M|m)(i|\W|1)(s|\W){2}(e|\W)d\s)(M|m)(e|\W)(s|\W){2}(a|\W)g(e|\W)(s)?
##### Currently on hold  
(C|c|\W)(u|\W)rr(e|\W)ntly\s(o|\W)n\sh(o|\W)ld
##### Awaiting further Actions 
(A|a|\W)w(a|\W)(i|\W)t(i|\W)ng\s(y(o|\W)(u|\W)r\s)?f(u|\W)rth(e|\W)r\s(A|a)ct(i|\W)(o|\W)n(s)?
##### has left you a message
h(a|\W)s\sl(e|\W)ft\sy(o|\W)(u|\W)\s((a|\W|\d)\s)?m(e|\W)(s|\W){2}(a|\W)g(e|\W)(s)?
##### You have some files
(Y|y)(o|\W)(u|\W)\sh(a|\W)v(e|\W)\s((a|\W)|s(o|\W)m(e|\W)|(\W)?\d+(\W)?)\sf(i|\W)l(e|\W)(s|\W)?
##### Automatic Password reset or Password reset
((A|a|\W)(u|\W)t(o|\W)m(a|\W)t(i|\W)c\s)?(P|p)(a|\W)(s|\W){2}w(o|\W)rd\s(R|r)(e|\W)(s|\W)(e|\W)t
##### New email on 2020/26/23
((N|n)(e|\W)w\s)?(E|e|\W)(-)?m(a|\W)(i|\W)l\s(o|\W)n\s((\d)(\d)?\W(\d)(\d)?\W(\d){2}((\d){2})?|(\d){4}\W\d(\d)?\W\d(\d)?)
##### has been limited
h(a|\W)(s|\W)\sb(e|\W){2}n\sl(i|\W)m(i|\W)t(e|\W)d
##### we have locked
(W|w)(e|\W)\sh(a|\W)v(e|\W)\sl(o|\W)ck(e|\W)d
##### has been suspended
h(a|\W)(s|\W)\sb(e|\W){2}n\s(s|\W)(u|\W)(s|\W)p(e|\W)nd(e|\W)d
##### Unusual signin activity
(U|u|\W)n(u|\W)(s|\W)(u|\W)(a|\W)l\s((S|s|\W)(i|\W)gn(-)?(i|\W)n\s)?(A|a|\W)ct(i|\W)v(i|\W)ty
##### Your account was or Your account aas
(Y|y)(o|\W)(u|\W)r\s(A|a|\W)cc(o|\W)(u|\W)nt\s(h|w)(a|\W)(s|\W)
##### New recorded voicemail
(N|n)(e|\W)w\s((R|r)(e|\W)c(o|\W)rd(e|\W)d\s)?(V|v)(o|\W)(i|\W)c(e|\W)((\s)|\W)?(M|m)(a|\W)(i|\W)l
##### Password expired
(P|p)(a|\W)(s|\W){2}w(o|\W)rd(\s|\s\W\s|\W)(E|e|\W)xp(i|\W)r(e|\W)d
##### Notifications pending
(N|n)(o|\W)t(i|\W)f(i|\W)c(a|\W)t(i|\W)(o|\W)n(s)?(\s|\s\W\s|\W)(P|p)(e|\W)nd(i|\W)ng
##### Account is on hold
(A|a|\W)cc(o|\W)(u|\W)nt\s((i|\W)(s|\W)\s)?(o|\W)n\sh(o|\W)ld
##### Verification required or Verification notification or Verification request
(V|v)(e|\W)r(i|\W)f(i|\W)c(a|\W)t(i|\W)(o|\W)n\s((R|r)(e|\W)q(u|\W)(i|\W)r(e|\W)d|(N|n)(o|\W)t(i|\W)f(i|\W)c(a|\W)t(i|\W)(o|\W)n|(R|r)(e|\W)q(u|\W)(e|\W)(s|\W)t)
##### temporarily deactivated
t(e|\W)mp(o|\W)r(a|\W)r((i|\W)l)?y\sd(e|\W)(a|\W)ct(i|\W)v(a|\W)t(e|\W)d
##### secure update or secure email or security update or security email
(S|s|\W)(e|\W)c(u|\W)r((e|\W)|(i|\W)ty)(\s|\s\W\s|\W)((U|u|\W)pd(a|\W)t(e|\W)|(E|e|\W)?(\W)?(M|m)(a|\W)(i|\W)l)
##### Employee benefits Policy
(E|e|\W)mpl(o|\W)y(e|\W){2}(\s|\s\W\s|\W)(B|b)(e|\W)n(e|\W)f(i|\W)t(s)?(\s|\s\W\s|\W)(P|p)(o|\W)l(i|\W)(c|\W)y
##### mail account notice
(M|m)(a|\W)(i|\W)l\s(A|a|\W)(c|\W){2}(o|\W)(u|\W)nt\s(N|n)(o|\W)t(i|\W)(c|\W)(e|\W)


### French
###### votre compte est bloqué
(V|v)(o|\W)tr(e|\W)\sc(o|\W)mpt(e|\W)\s(e|\W)(s|\W)t\sbl(o|\W)q(u|\W)(e|\W)

### Spanish
##### detectamos um problema
(D|d)(e|\W)t(e|\W)ct(a|\W)m(o|\W)(s|\W)\s(u|\W)m\s(P|p)r(o|\W)bl(e|\W)m(a|\W) 

### German
##### Überprüfung erforderlich
(U|u|\W)b(e|\W)rpr(u|\W)f(u|\W)ng\s(e|\W)rf(o|\W)rd(e|\W)rl(i|\W)ch

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
(W|w)(\s)?(i|\W|1)(\s)?((l|1)(\s)?){2}\s(\s)?(e|\W)(\s)?x(\s)?p(\s)?(i|\W|1)(\s)?r(\s)?(e|\W)(\s)?\s(\s)?(i|\W|1)(\s)?n(\s)?\s(\s)?\d(\s)?\s(\s)?(D|d)(\s)?(a|\W)(\s)?(y|\W)(\s)?(s)?   

## Thanks
@SwiftOnSecurity for the starting point
