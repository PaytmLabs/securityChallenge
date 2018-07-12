# Security Challenge

You are a Security Engineer at an e-commerce company. The company is running a public facing marketing website.

The following is the website's technology stack:

HTML/CSS and JavaScript

PHP

MySQL

Linux with Apache

## Scenario
The CEO of the company notifies you that the website is down. Upon an investigation, you notice the following:

The company's public website was defaced, there's now a black background with green text instead.
You notice unknown files on the server's doc root folder.
You notice the following entries in the web server access log file:

82.2.5.25 - - [16/Apr/2018:20:21:56 +0100] "GET /config/sql.conf HTTP/1.1" 404 3804 "-" "curl/7.37.0"
82.2.5.25 - - [16/Apr/2018:20:21:58 +0100] "GET /config/mssql.conf HTTP/1.1" 404 3804 "-" "curl/7.37.0"
82.2.5.25 - - [16/Apr/2018:20:21:59 +0100] "GET /config/postgres.conf HTTP/1.1" 404 3804 "-" "curl/7.37.0"
82.2.5.25 - - [16/Apr/2018:20:22:00 +0100] "GET /config/mysql.conf HTTP/1.1" 200 3804 "-" "curl/7.37.0"
84.155.41.27 - - [16/Apr/2018:21:20:56 +0100] "POST /phpmyadmin/login HTTP/1.1" 200 3804 "-" "Mozilla/5.0 (Windows NT 6.0; WOW64; rv:45.0) Gecko/20100101 Firefox/45.0"
84.155.41.27 - - [16/Apr/2018:22:50:05 +0100] "GET / HTTP/1.1" 200 3804 "-" "Mozilla/5.0 (Windows NT 6.0; WOW64; rv:45.0) Gecko/20100101 Firefox/45.0
84.155.41.27 - - [16/Apr/2018:22:56:56 +0100] "POST /uploads/c99.php HTTP/1.1" 200 3804 "-" "Mozilla/5.0 (Windows NT 6.0; WOW64; rv:45.0) Gecko/20100101 Firefox/45.0"

## Question
Given this scenario, answer the following questions:

Describe what most likely happened based on the information you have.

Calculate the CVSSv3 scores for the vulnerabilities that could have led to the defacement of the website, explain the rational of each vector.

Describe how you would recover the system safely.

Provide the company with security improvements.
