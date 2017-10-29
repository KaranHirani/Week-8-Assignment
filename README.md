# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: __________________

Vulnerability #2: __________________


## Green

Vulnerability #1: Username Enumeration: This vulnerability makes it such that if you type in a known username and type in any wrong password, they error message will be in bold.  If you type in a unknown username, or a username not in the SQL database, then the error message will not be in bold.  This exploit makes it easy for a hacker to find what usernames are actually in the system and which ones are not.  If you type in a username like: jmonroe99, this will show up as bold, but if you type in a username like: test, this will not show up as bold.

GIF Walkthrough:  <img src="https://github.com/KaranHirani/Week-7-Project/blob/master/assignment7_3.gif?raw=true" alt="Girl in a jacket">

Vulnerability #2:  Cross-Site Scripting: This vulnerability causes the browser to create a popup when you click on the feedback link in the login page.  To recreate this exploit, go to the feedback page and type in any name and email and type in the following code:   `<script>alert('Karan found the XSS!');</script>` When you go to the login page and click feed back, you will get a popup from the browser.

GIF Walkthrough:  <img src="https://github.com/KaranHirani/Week-7-Project/blob/master/assignment7_3.gif?raw=true" alt="Girl in a jacket">

## Red

Vulnerability #1: Insecure Direct Object Reference: This vulnerability allows you to view sales people who should not be on the page.  If you go to the blue or green site and click on any of the sales people and change the id to 10 or 11, nothing will pop up.  If you go to the red site, however, and click on a sales person and change id to 10 or 11, you will see two sales people who should not be visible.

GIF Walkthrough:  <img src="https://github.com/KaranHirani/Week-7-Project/blob/master/assignment7_3.gif?raw=true" alt="Girl in a jacket">

Vulnerability #2: __________________


## Notes

Describe any challenges encountered while doing the work
