# DontCry
An idea to stop the WannaCry ransomware: to create a similar white-worm that uses eternalblue to hack into vulnerable machines 
and disable smb/apply patch.

Idea & Logic:

First to take a look at the eternalblue worm:
https://blog.malwarebytes.com/threat-analysis/2017/05/the-worm-that-spreads-wanacrypt0r/
And to replicate the method in python (as that's what I will be using here, hopefully)

First scans the Windows machine and see if it's vulnerable (either with python or with something like this: https://github.com/3gstudent/Smbtouch-Scanner)

Then enchance the ability of eternalblue.py and add in a command to run on the target Windows box after the exploit is successful,
e.g. modifying the registry/network service to disable smb port. Applying the patch will also be attempted.

Admins feel free to modify it to suit ur own internal networks / intranets, might help find the little unpatched dark corners.

I don't know if I have what it takes to get this done at all, or in time. Please help.
