# CTFs

# Hack The Box CTF Adventures

## 1. Cryptic Chronicles: A Cryptographic Journey

### Introduction

In this detailed account, I share my experiences with the "Cryptic Chronicles" Capture The Flag (CTF) challenge on Hack The Box. This cryptographic journey led me through deciphering messages, unveiling hidden keywords, and ultimately decrypting the flag.

#### Getting Started

Upon joining the CTF, I encountered an encrypted message, setting the stage for a cryptographic puzzle.

#### Cryptographic Conundrum

I utilized frequency analysis and identified a Caesar cipher, leading to the revelation of a Vigenere cipher.

#### Web Exploitation: Unveiling the Keyword

Exploring the web interface, I discovered a hidden page, downloaded a keyword, and prepared for the next phase.

#### Decrypting the Flag

Applying the Vigenere cipher with the obtained keyword resulted in the triumphant decryption of the flag.

### Conclusion

The "Cryptic Chronicles" CTF provided an engaging exploration of cryptography and web exploitation, reinforcing the importance of interdisciplinary knowledge in cybersecurity.

## 2. Web Wonders: Navigating Web Application Security

### Overview

Welcome to my Hack The Box Capture The Flag (CTF) write-up! This journey, named "Web Wonders," explores the fascinating realm of web application security challenges. In this adventure, we'll navigate through login pages, uncover SQL injection vulnerabilities, exploit weaknesses, and ultimately claim the elusive flag.

#### Introduction

"Web Wonders" promises a captivating blend of challenges centered around web application security. As we step into the virtual arena, the goal is clear: navigate through web vulnerabilities, exploit weaknesses, and seize the elusive flag.

#### The Web Wonderland

The CTF adventure begins with a seemingly innocent login page, hiding potential vulnerabilities waiting to be uncovered.

#### Exploring the Login Page

- **Initial Reconnaissance**: A careful examination of the login page's source code and inspecting network requests using browser developer tools.

```html
<!-- Relevant snippet from the login page source code -->
<form action="/login" method="POST">
    <input type="text" name="username" placeholder="Username">
    <input type="password" name="password" placeholder="Password">
    <button type="submit">Login</button>
</form>

```
SQL Injection Discovery: Closer inspection reveals susceptibility to SQL injection, leading to an interesting error message.
```
SQL Error: You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax...
```
Exploiting SQL Injection
Crafting the Payload: A payload is crafted to bypass authentication.
```
' OR '1'='1'--
```
Successful Login: Submitting the payload as the username successfully bypasses authentication.
Locating the Flag

Directory Traversal: Navigating through the application, a directory traversal vulnerability in the file download functionality is discovered.

```
https://webwonders.ctf/files/download?file=../../flag.txt
```
Claiming the Flag: The contents of the flag.txt file are revealed, and victory is within reach.
```
HTB{w3b_app_mast3r}

```
Conclusion
"Web Wonders" provides a thrilling adventure into the realm of web application security. From uncovering SQL injection vulnerabilities to exploiting directory traversals, the challenges reinforce the significance of robust web security practices. This CTF not only hones penetration testing skills but also highlights the critical importance of securing web applications in the real world.

