# CTFs

# Hack The Box CTF Adventures

## 1. Cryptic Chronicles: A Cryptographic Journey

### Introduction

Greetings fellow ethical hackers! In this detailed account, I share my experiences with the "Cryptic Chronicles" Capture The Flag (CTF) challenge on Hack The Box. This cryptographic journey led me through deciphering messages, unveiling hidden keywords, and ultimately decrypting the flag.

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
