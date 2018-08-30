### Neural network password meter

Most existing client-side password checkers rely on simple heuristics like counting the number of characters or character classes in a password. Artificial neural networks have been used to model resistance to password guessing, outperforming traditional rule based methods like hashcats. 

By leveraging on natural language, tokenized models, or other neural networks ar chitectures, we should be able to see passwords being guessed more effectively, develop better password meters and improve password creations for the mass. The network can also be compressed to portable size like few hundred kilobytes, making it suitable for mobile devices or on a web page.


### Machine learning based AV
Machine learning can offer a generalised way of identifying malicious activiies. For e.g. port scanning which stands out from normal network traffic, administrator account logging in to large numbers of workstations, huge data transfers to unfamiliar IP addresses would be easily identifiable as anomalous.

Consider the other side: a user falls for a spear phishing attack, his valuable documents and emails  are immediately stolen. These do not represent large data volumes and hence not flagged. Compromised helpdesk support access workstations on a daily basis and in a manner correlated with user phone calls and support requests. This account is unlikely to be seen as anomalous. Google Chat is used as the command and control channel and only makes connections when in use. It’s likely that many systems on the network are already actively using this service. Therefore, the machine learning AV would not flag these scenarios as malicious.

### OS security
Linux may be more secure largely due to fewer exploits being discovered in Linux than in Windows. 
Windows is the most used OS, therefore to get the most bang for their buck, most cyber researchers and attackers
focus their effort on Windows.

![why linux is more secure](/images/os-secure.png)

As we can see from exploit-db, Linux, like Windows, has vulnerabilities, 

![exploit db](/images/exploit-db1.png)


### Patch
To manage cyber threats, the priority is to patch software regularly. Consider using password managers to store strong, unique passwords. Antivirus may give a false sense of security as some attacks bypass it.

![Google security practices](/images/sec_practices-v6.png)

### Sandbox
Harden the system with layers of defence , e.g. install browser blocker plug-in, sandbox the browser, run the broswer in VM to better secure the system.

Sandboxie is one sandbox application in Windows. It separate programs from the OS to prevent unwanted changes from happening to data and applications. Therefore programs in Sandboxie can only modify the contents of the sandbox.
The yellow border around the application window shows that the application is being sandboxed, adding another layer of defence in the system. 

![sandbox 1](/images/sandbox1.png)

For Linux, I use the simple firejail to sandbox applications.
![firejail](/images/firejail2.png)

### Verify Downloads
To ensure the authenticity and integrity of our download files, we could verify digital signatures, master signing keys, release signing keys to ensure that the files were created by the person who signed them and that the contents of the files have not been tampered with by a third party.  
![gpg 1](/images/gpg-1.png)
![gpg 2](/images/gpg-2.png)
Downside is digital signatures cannot prove that the signed file is not malicious. 

### Wipe Files
The normal delete or rm command will leave data behind. There are some tools that help to wipe and overwrite the space used by the deleted files.  srm is the secure version of rm. 
![srm](/images/srm.png)
Data may be present in memory after the system shuts down, sdmem command wipes the RAM. One pass with zeroes is good enough.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
