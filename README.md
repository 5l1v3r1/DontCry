# DontCry
An idea to stop the WannaCry ransomware: to create a similar white-worm that uses eternalblue to hack into vulnerable machines 
and disable smb/apply patch.

Idea & Logic:

First to take a look at the eternalblue worm:
https://blog.malwarebytes.com/threat-analysis/2017/05/the-worm-that-spreads-wanacrypt0r/
And to replicate the method in python (as that's what I will be using here, hopefully)

Then enchance the ability of eternalblue.py and add in a command to run on the target Windows box after the exploit is successful,
e.g. modifying the registry/network service to disable smb port. Applying the patch will also be considered.

Unleash it into the wild... Mass port scan on 445 and run the scripts on all those machines... :)

I don't know if I have what it takes to get this done at all, or in time. Please help.
