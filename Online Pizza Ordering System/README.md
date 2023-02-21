# Online Pizza Ordering System has XSS vulnerability

## XSS vulnerability

BUG_Author: Murasaki

URL：http://localhost/php-opos/index.php?page=checkout

Link:https://www.sourcecodester.com/php/16166/online-pizza-ordering-system-php-free-source-code.html

There is a stored XSS vulnerability in the order submission,attackers can use XSS injection to steal the identity authentication of administrative users, and perform some background operations as administrators to achieve CSRF attacks. Attackers can also hang horses on websites, so that visitors' browsers can be controlled by attackers.

![image](https://github.com/1MurasaKi/PizzeXSS_Pic/blob/main/order.png?raw=true)

![image](https://github.com/1MurasaKi/PizzeXSS_Pic/blob/main/admin.png?raw=true)

## How to fix it
* Filter dangerous characters

* Set CSP (Content Security Policy)
