---
Tags: LandingTopic
Topic: ComputerScience
---
Related topics: [[Computer Science]]

When we want to send a message to someone else or keep a message for us and for any reason we don't want any want else to know it or even be able to understand it, then we can implement some methods.

If we want to send a message to someone else, then we have to set a way in which we both can understand the message, but someone else can't. To do that we can code or **cypher** our message, therefore no one else will be able to understand it, but we also need to ensure that the other person will be able to **decipher** that code and recover the original message. 

The cryptography is the field of study which deals with this kind of interaction or processes of encryption and 

# Encryption

Is the process of cypher or code a message, so we can't understand it at first sight. And of course we can do the following [[abstraction]]: 

![[Encryption abstraction.png]]

Beside the text which we want to cypher we also use a key, that is a value which shifts or modifies the behavior of the encryption [[Functions|function]]. For example a simple encryption [[Algorithms|algorithm]] is to move some number of position to one direction each letter (the number of positions is the key), so if we got the letter "a" and we use a key of 2, we would move a->b->c, and finally the a would be replaced by c. 

# Decryption

The decryption is the opposite of the encryption, in the most of the times we want not to encrypt, but also decrypt the message so we can get the real message back, and the decryption consist in the same as encryption but the [[Algorithms|algorithm]] is reversed, so we get the cyphered text and the key and we do the opposite.

for example, instead of moving 2 positions to the right, we move two positions to the left. so we receive c->b->a, and we get back the a. 