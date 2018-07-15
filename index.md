### OS security
Linux may be more secure largely due to fewer exploits being discovered in Linux than in Windows. 
Windows is the most used OS, therefore to get the most bang for their buck, most cyber researchers and attackers
focus their effort on Windows.

![why linux is more secure](/images/os-secure.png)


As we can see from exploit-db, Linux, like Windows, has vulnerabilities, 

![exploit db](/images/exploit-db1.png)

To manage cyber threats the priority is to patch it regularly and harden it with layers of defence 
, i.e. browser blocker plug-in, sandbox the browser, run the broswer in VM to better secure the system.

### Sandbox
Sandboxie is one sandbox application in Windows. It separate programs from the OS to prevent unwanted changes from happening to data and applications. Therefore programs in Sandboxie can only modify the contents of the sandbox.
The yellow border around the application window shows that the application is being sandboxed, adding another layer of defence in the system. 

![sandbox 1](/images/sandbox1.png)

For Linux, I use the simple firejail to sandbox applications.

### Verify File Authencity and Integrity
To ensure the authenticity and integrity of our download files, we could verify digital signatures to ensure that it was created by the person who signed it and that the contents of the file have not been tampered with by a third party. PGP can be used to verify the master signing key, release signing key and download file. Downside is digital signatures cannot prove that the signed file is not malicious. 

![gpg 1](/images/gpg 1.png)
![gpg 2](/images/gpg 2.png)
