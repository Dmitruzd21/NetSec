# **Сетевая безопасность**

**Ссылка на задание/требования:** https://github.com/netology-code/ibqa-homeworks/blob/main/5.%20Network_Security/homework_lecture5.md

**Анализируемый хост:** scanme.nmap.org

Используемая команда: nmap -A scanme.nmap.org

## **Задание 1**

![Количество служб](/Zenmap1.png)

Количество сетевых служб, запущенных на указанном хосте: 4

## **Задание 2**

![Web-сервер](/Zenmap2.png)

В качестве web-сервера используется: Apache 2.4.7

## **Задание 3**

![ОС](/Zenmap3.png)

Скорее всего на сервере используется ОС: Linux (версии: 2.6.32; 2.6.39; 3.10-3.12)

Дополнительное использование --osscan-guess (--fuzzy) не помогло.

## **Задание 4**

![ExploitDatabaseExploits1](/ExploitDatabaseExploitsForPenetrationTester1.png)

![Apache Httpd mod_proxy - Error Page Cross-Site Scripting](/ApacheHttpdMod_proxyErrorPageCrossSiteScr.png)

![Apache Httpd mod_rewrite - Open Redirects](/ApacheHttpdMod_rewriteOpenRedirectsMultip.png)

![ExploitDatabaseExploits2](/Exploit%20DatabaseExploitsForPenetrationTester2.png)

Уязвимости, которым подвержен данный сервер (проверено при помощи сайта exploit.db):

- Apache Httpd mod_proxy - Error Page Cross-Site Scripting
- Apache Httpd mod_rewrite - Open Redirects
- Apache 2.4.7 mod_status - Scoreboard Handling Race Condition
- Apache 2.4.7 + PHP 7.0.2 - 'openssl_seal()' Uninitialized Memory Code Execution

Уязвимостей со стороны других сервисов не обнаружено.
