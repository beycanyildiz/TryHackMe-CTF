# [Linux PrivEsc] (https://tryhackme.com/room/linuxprivesc)

> Practice your Linux Privilege Escalation skills on an intentionally misconfigured Debian VM with multiple ways to get root! SSH is available. Credentials: user:password321


## Task 1: Deploy the Vulnerable Debian VM

### Deploy the machine and login to the "user" account using SSH.
```
No answer needed
```

### Run the "id" command. What is the result?
```
uid=1000(user) gid=1000(user) groups=1000(user),24(cdrom),25(floppy),29(audio),30(dip),44(video),46(plugdev)
```

## Task 2: Service Exploits

### Read and follow along with the above.
```
No answer needed
```

## Task 3: Weak File Permissions - Readable /etc/shadow

### What is the root user's password hash?
```
$6$Tb/euwmK$OXA.dwMeOAcopwBl68boTG5zi65wIHsc84OWAIye5VITLLtVlaXvRDJXET..it8r.jbrlpfZeMdwD3B0fGxJI0
```

### What hashing algorithm was used to produce the root user's password hash?
```
sha512crypt
```

### What is the root user's password?
```
password123
```

## Task 4: Weak File Permissions - Writable /etc/shadow

### Read and follow along with the above.
```
No answer needed
```

## Task 5: Weak File Permissions - Writable /etc/passwd

### Run the "id" command as the newroot user. What is the result?
```
uid=0(root) gid=0(root) groups=0(root)
```

## Task 6: Sudo - Shell Escape Sequences

### How many programs is "user" allowed to run via sudo? 
```
11
```

### One program on the list doesn't have a shell escape sequence on GTFOBins. Which is it?
```
apache2
```

### Consider how you might use this program with sudo to gain root privileges without a shell escape sequence.
```
No answer needed
```

## Task 7: Sudo - Environment Variables

### Read and follow along with the above.
```
No answer needed
```

## Task 8: Cron Jobs - File Permissions

### Read and follow along with the above.
```
No answer needed
```

## Task 9: Cron Jobs - PATH Environment Variable

### What is the value of the PATH variable in /etc/crontab?
```
/home/user:/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin
```

## Task 10: Cron Jobs - Wildcards

### Read and follow along with the above.
```
No answer needed
```

## Task 11: SUID / SGID Executables - Known Exploits

### Read and follow along with the above.
```
No answer needed
```

## Task 12: SUID / SGID Executables - Shared Object Injection

### Read and follow along with the above.
```
No answer needed
```

## Task 13: SUID / SGID Executables - Environment Variables

### Read and follow along with the above.
```
No answer needed
```

## Task 14: SUID / SGID Executables - Abusing Shell Features (#1)

### Read and follow along with the above.
```
No answer needed
```

## Task 15: SUID / SGID Executables - Abusing Shell Features (#2)

### Read and follow along with the above.
```
No answer needed
```

## Task 16: Passwords & Keys - History Files

### What is the full mysql command the user executed?
```
mysql -h somehost.local -uroot -ppassword123
```

## Task 17: Passwords & Keys - Config Files

### What file did you find the root user's credentials in?   
```
/etc/openvpn/auth.txt
```

## Task 18: Passwords & Keys - SSH Keys

### Read and follow along with the above.
```
No answer needed
```

## Task 19: NFS

### What is the name of the option that disables root squashing?
```
no_root_squash
```

## Task 20: Kernel Exploits

### Read and follow along with the above.
```
No answer needed
```

## Task 21: Privilege Escalation Scripts

### Experiment with all three tools, running them with different options. Do all of them identify the techniques used in this room?
```
No answer needed
```
