# haveibeenpwned

Python script to verify single or multiple email addresses for *pwnage* :fire:

## **Usage**:

> - python3 haveibeenpwned.py [-h] [-a ADDRESS] [-f FILENAME]

> - -h, --help   show help message 
> - -a ADDRESS   Single email address to be checked
> - -f FILENAME  File to be checked with one email addresses per line

This tool respects the rate limit (HTTP 429) and adjusts accordingly.
Output is in color to show the differences between breached and not breached.

This tool also display all the breaches associated with an address, and the data leaked for each breach.

Example output:
```python
[!] info@example.com has been breached 16 times!

[1]     Service Name: Adobe
        Breach Date: 2013
        Data leaked: Email addresses, Password hints, Passwords, Usernames



[2]     Service Name: Anti Public Combo List
        Breach Date: 2016
        Data leaked: Email addresses, Passwords



[3]     Service Name: Dropbox
        Breach Date: 2012
        Data leaked: Email addresses, Passwords



[4]     Service Name: Evony
        Breach Date: 2016
        Data leaked: Email addresses, IP addresses, Passwords, Usernames



[5]     Service Name: Exploit.In
        Breach Date: 2016
        Data leaked: Email addresses, Passwords

```

EOF:w
