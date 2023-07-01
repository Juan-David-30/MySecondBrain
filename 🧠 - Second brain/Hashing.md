Related topics: [[Cybersecurity]]

Hashing is the process to assign a key to a specific text or input, commonly used in cybersecurity to store passwords. 

![[Hash function.png]]

The hash is nothing more but a function, which maps a input to a output, but the interesting is that now the output will be "cryptic" or secure and not the actual password, so if someone find the hash, not necessarily will be the same as knowing the password.

And other interesting part of the hash is that it is not invertible, so even though someone access to the hash, they'll probably not have access to the actual password, and even if they have the function which hashes the password, they'll still not having the value, because its invertible characteristic.

We still being possibly attacked by a brute attack, it will take even more computational power to find or crack our password. So in this way we're increasing the effort to do for the adversary. 

Now it turns out that the hashing functions receive a input and returns a output with a fixed length, so to speak mathematically, the hash functions are functions which maps a infinite domain of possible values or texts, into a finite domain. 

![[Fixed length of the hash.png]]

So, yeah, it turns out that some outputs are repeated, what implies two things mainly:
+ Are not [[Inverse functions|invertible functions]]
+ It exists the possibility that someone find other of the inputs which map to the same output of your password and get access with a absolutely different value of your actual password 

# Salt 

Now if we apply the same process to the same input of course we will get the same value, or output, and that's a problem for some reasons: 

+ First if the adversary somehow know which algorithm of hashing we're using, they'll probably use a rainbow table, which is a table of common values or words and compare them with the passwords. 
+ At first glance someone could notice if two users have the same password, and that's a disadvantage because we're giving more information to the adversary, they could search for common information or likes which those users share in order to figure out the password. 

So to avoid it we use something called salt, it consist in simply adding fasting a random string to the original message before hashing it, so even two password equal would have different hashes.

Commonly this salt is added together with the hashed value, so we can know what is the salt in the moment in which someone tries to log in. The salt doesn't need to be secret, its purpose is just to change the hash in a way in which can't be evident at first glance if two passwords are the same or avoid the use of rainbow tables.
