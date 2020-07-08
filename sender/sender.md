## Sender spoofing your company

Turn on spoof protection for you (or your company)
If you have services, which are "essential" (or you don't wnat to argue to much) add them to the allow list.

## Enable SPF, DKIM and DMARC

Be nice to others and enable this service for your yourself/brand/company.

## Sender contains the following regex

##### will catch @m1crosoft or g0ogle or @c0mpany or @your-c0mpany  
```
@([a-z]+[01]([01])?[a-z]+|[a-z]+\-[a-z]+[01]([01])?[a-z]+)
```
##### will catch some double tld
```
\@\w+\-(com|biz|org|net)\.\w{2,3}
