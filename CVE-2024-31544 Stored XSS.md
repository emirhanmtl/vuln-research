
# CVE-2024-31544 Stored XSS in Computer Laboratory Management System
+ Exploit Author: Emirhan Mutlu
# Vendor Homepage
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Software Link
+ https://www.sourcecodester.com/php/17268/computer-laboratory-management-system-using-php-and-mysql.html
# Overview
+ A stored cross-site scripting (XSS) vulnerability in Computer Laboratory Management System v1.0 allows attackers to execute arbitrary JavaScript code by including malicious payloads into “remarks”, “borrower_name”, “faculty_department” parameters in "http://localhost/php-lms/classes/Master.php?f=save_record" endpoint.
# Vulnerability Details
+ CVE ID: CVE-2024-31544
+ Vulnerable Endpoint: /php-lms/classes/Master.php?f=save_record
+ Request Method: POST
+ Parameters: “remarks”, “borrower_name”, “faculty_department”
# Description
+ The lack of proper input validation and sanitization on the parameters allows an attacker to execute arbitrary JavaScript codes

# Proof of Concept (PoC) : 
+ Payload
+ `test1"><img src=x onerror=alert(1)>;//`
