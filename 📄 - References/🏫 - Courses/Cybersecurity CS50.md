---
Tags: Course
Topic: Cybersecurity, "Computer Science"
Institution: Harvard
---
Related topics: [[Computer Science]], [[Cybersecurity]]

# What will I learn?

We'll learn how to write some code in [[python]] and learn about different topics of cyber security such as passwords and how to keep them save. 

"Cybersecurity is the art of protecting networks, devices, and data from unauthorized access or criminals use and practice of ensuring confidentially and integrity, and availability of information"

---

# Introduction class

+ What is cybersecurity about?
+ Hackers
	Hackers are the adversaries or people who try to attack us or brake our security for whatever reason
+ Trade off
	We could create a complete secure device, but if we get it it would probably lose usability, so the cybersecurity can be thought as a trade off of security and usability.
	
	So our goal is to make our security enough secure to make the adversary work harder and so that discourage them. 
+ We're in disadvantage
	Is necessary to understand that that we're in constant disadvantage, we can have security tools, but if we forget to use them, then we'll lost, whilst the hacker or adversary just needs to find one unique mistake they've won, we have to be perfect, while the adversary just needs to find one mistake. 

## Authentication

Authentication is a process where we determinate whether you are who you say you are, in internet you determinate whether or not you are the owner of you account, because isn't enough with just typing you're username, commonly you also have to validate that you're the owner of the account in other ways, such as using a passwords (the most common), double factor-authentication and so on. 

So this second way to authenticate your self is actually really important to make it secure. 

### Password

Is really important to have a secure password, and that's not often well supplied by the users, indeed the most popular password world wide, are sequences of numbers such as 1234, or alike, which of course isn't secure, someone could try this because it is such simple and popular that can make you be hacked easily. 

Other common error is to use the same password for your accounts, which exposes us to the threat that if some one figures out our password in one account in whatever way, then they can try that same password on the another accounts and then we have a worse case. 

Other problem is to use short passwords, because there can be people who knows how to program and they could just use a program which tries all the possibilities and then hack us quickly. So is important to make our passwords of a considerable long and not just that but mix them with several options such as letters, numbers and special characters, the explication is simple and that just [[mathematics]], specifically that's a permutations where we find all the possibilities and we run through them. 

# Lecture 0 - Securing accounts

## Authorization

Often isn't enough with just authenticating ourselves, we have talk about authorization to know where and what we have access to, what actions, what can we see and so on. 

## Attacks

There are several kind of attacks to try to break our security, and get our data or access to our accounts. 

### Dictionary attack

A dictionary attack is a attack which consist in using a virtual dictionary to try all the english (or any other language) words as your password, so for example if you have "banana" as a password, you are not quite secure. 

### Brute attack

This unlike the dictionary attack this attack does not use necessarily real words but it just try all the possibilities, of course it sounds as a tedious process who no one would do, but in fact that is possible thanks to the use of scripts. 

Anyone with basic knowledge in programming can easily just create a script to try all the possibilities faster and not that tedious. 

That process can be more tough for the adversary either giving more possibilities for each characters, for example instead of using just numbers also using letters and punctuation, and even instead of using for example a password of 4 characters, using 8, or 10 or even more. 

## National Institute of Standards and Technology (NIST)

Is a institute which sets some standards of cyber security. 

+ The passwords must have at least 8 characters of length 
+ The passwords must allow be at maximum at least 64, allowing blank spaces ASCII and unicode characters. 
+ The website have to verify the password and avoid you to use this ones which follows:
	+ Dictionary words
	+ Repetitive or sequential characters
	+ Context-specific words
+ The website must no accept a hints
+ Verifiers should not require change your password periodically 

## Defenses against attacks

There are multiple ways to defend our accounts, for example our phones have a method to protect our phone is to stop or disabling you to write passwords after a certain amount of tries.  

### Two-factor authentication

Consist in splitting the authentication in two factors, this is different to two-step authentication, where it can consist in simply just two passwords, while the two-factor consist in two different ways to authenticate. 

+ Knowledge
	+ Something that we know such as our password
+ Possession
	+ Something that we have, such as our cellphone, when we're ask to write a code sent to your phone, or similar
+ Inherence
	+ Something that you have inherit such as your biometrical data as our finger prints or your face features

### One time passwords

These are passwords which are used just once, these are the one sent for example to our SMS, where we receive just a code through our SMS (sometimes that's done through a native app).

#### SIM swapping

This is a attack which consist in making change your SIM, thanks to convincing our operators to change our SIM, not physically but in other ways, although it sounds weird and not a common practice, it actually is. Is common to call our telephony company and say that we've changed of number, that one's SIM is this rather to this now. Then with just giving some basic data about us is possible to change our SIM and then get our messages or codes of the two-factor authentication. 

So in the most of the cases is better to use native apps un our phone rather to the SIM authentication. 

#### Key-logging

Sometime we could have a virus in our phone, and they not necessarily make our phone behave in an odd way, rather they can just sneak in our phone and be there hiding their existence. And they can be just stealing us information quietly. Such as getting access to our SMS, our reading what we're typing an thus being able to access to our data, codes, passwords and a lot of information of our. 

## Credential Stuffing

This is other attack which consist that if someone gets our username and password in one website in any way, they'll probably 

## Social engineering

Is a method in which a figure in which we trust can get information of us, or convince us to do so. 

### Phishing 

Phishing is a method which use social engineering to try to get information of us, like sending emails pretending to be someone or something in which we trust asking us for information, like validating data, or changing or password. 

But instead of doing it we're just giving that data to the adversary and being completely at they're mercy in our accounts. 

## Machine-in-the-Middle attack

This is related to the communication, and indeed even though we think we're save we have to understand that our communication in the web isn't straight with the website we're trying to access to rather, there is a lot of machines working in the middle, and in all this process of communication we can be attacked. 

Indeed there can be people able to intercept our messaging and read our communication with the server, so to protect ourselves we have to use techniques as encryption. 

## Single Sign-On (SSO)

Single Sign-on, consists in using a single sign in for all the websites, often when we access to a website we can find an option as "log-in with google", is a good idea to use those kind of authentications, and indeed google creates the new account for us using all the good practices and creating a good/secure new password, and we don't have to create a new one or even remember it. 

## Password managers

A password manager is a app or software which does a similar work as the Single Sign-On, which creates secure password, stores them and even inserts them to automatically sign in easily but, the trade off is that is dangerous to lose the password fo the password manager. 

So we have to create a unique really strong password which in case you lose it you'll lose all the other passwords and accounts. 

## Passkeys

A passkey is a new authentication technology that uses public key cryptography to enable users to log into websites and apps without having to enter a password. Instead, users authenticate the same way they unlock their phones and tablets: with their fingerprint, face or other biometrics; by using a swipe pattern; or by entering a PIN. For purposes of convenience, most people will opt for biometric authentication.

# Lecture 1 - Securing data

Securing data is a important part of the cybersecurity for several reasons, indeed the privacy is an important aspect for everyone, and for security for the accounts too, for example is really important to storage our passwords securely.

## Store passwords

Is important so store our passwords securely, for our security and for the users, imagine that we're the developers of a website or application, if we store the passwords literally as they were written, and someone somehow access to where that information was stored, the person who accessed to it will have the password of every user, and then they may us it not just in our website but also in credential stuffing. 

So one of the most often used techniques is [[Hashing]], and we just save the hashed value of the password rather to the password literally. 

# Lecture 2 - Securing systems

[[Cryptography]] will be also a important tool when we are trying to secure systems, we'll focus in systems such as networks and internet. 

## Wi-Fi

When we're communicating through wi-fi, if we're using the current version, we're using wi-fi protected access, which uses [[Cryptography]] to communicate the interactions with servers and other computers. 

## HTTP 

When we're communicating through internet one of the most commons protocols is [[HTTP]], which stands for HyperText Transference Protocol, the problem is that when we're using HTTP alone, isn't secure itself, we're vulnerable to machine-in-the-middle attacks. 

And there are multiple threats when there is a machine-in-the-middle attacks, imagine that you're doing a request, and a machine in the middle can intercept that request, they could add things to you're request, like adding scripts of publicity or even worse adding dangerous strips to steal information or break your computer. 

Other possible attack is that in a machine-in-the-middle we're vulnerable to lose be stolen of information in the communication, imagine we're logging in or signing up in a web site, and if a machine-in-the-middle attacks you could steal that information, they could read all your HTTP's. requests and information sent there, this kind of attack is known as "package sniffing".

## Cookies

Our browsers commonly use [[Cookies]], they are often used and are really useful, but often they can be used for other sort of attacks such as session hijack.

It turns out that when we log in a website, often we receive a cookie message, which contains some information or credential so we don't have to log in again and again, rather that's a credential that we've started session, so we don't have be logging in at each action we do in the website. 

Now there exists something called super cookies, which are cookies not injected by the server you're communicating with, rather they're being injected by machine-in-the-middle attacks, with the goal of tracking you, and to give you advertisings. 

## HTTPS

Is well-know that we should intend to use websites which have a HTTPS protocol rather to a just HTTP, and that's because we're using the same HTTP protocol but, in conjunction with other one called TLS (you might be familiar with SSL, indeed TLS is like the evolution or one of the new versions of it). 

## SSL stripping 

When we try to access to a resource in internet, often we don't write the whole URL, what means that we don't add the "https://domain.com", we could just write "www.domain.com", or "http://domain.com", even just "domain.com", all these practices are common, but they have a vulnerability. 

It turns out that when we write an incomplete URL, what will happen is that a server will send us back a HTTP response which contains a code 307, what means redirecting, go to this direction rather to this other, and is commonly used to complete the URL. 

Now it turns out that some machine-in-the-middle, could intercept that communication, and send the response, so instead of receiving a redirection of the server we intend to communicate with, we're being redirected for a third party 


## HSTS

But to avoid that SSL stripping can be tedious, so to avoid it or somehow make it automatic we use **HTTP Strict Transport Security (HSTS)**, thanks to that we just have to access to the actual website with the whole URL just once. 

![[HTST message.png]]

Then the server through HSTS will tell to your browser to use always HTTPS, so even if you don't write the whole URL, or just use HTTP, then the browser will switch automatically to HTTPS. 

## VPN (Virtual Private Network)

Is a network or connection which establish a private connection between you and a network, in which all the messages you send and receive are encrypted, so if there are machine-in-the-middle they could not understand that communication. 

The VPN is commonly used to access to internet anonymous, you establish a connection with a server through VPN, and that server does the request to the rest of the internet for you, so the rest of the internet thinks that the server is who's doing the requests. 

## SSH (Secure Shell)

This is the similar to a VPN to connect with other computer but in order to write commands through Shell commands. 


## Port



### Port scanning

### Penetration testing (pen-testing)

Is the process to test or try the ports and see if there are some ports which are listening the internet when they shouldn't, that's a **Ethical Hacking**, where we search for weaknesses to find them and fix them before someone else, a possible adversary does it. 

## Firewall

A firewall is a software which scans the internet traffic and block dangerous or not allowed traffic. For example we could create a local network which just certain computers or IP addresses to access. 

The firewall could try to 

## Proxy 

A proxy server is a computer in the middle in your communication with the purpose to check every single action you're doing, which link you're visiting and so on, and check if what is being send and received is secure and if it is not, it deletes or cancels the connection, protecting you of receiving 

# Lecture 3 - Securing software

## Phishing 

---
# Link to the resource
[CS50's Cybersecurity](https://cs50.harvard.edu/cybersecurity/2023/zoom/)

