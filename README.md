# Custom-Kali-Server-Cli

- ## What is it ?
It is a simple customised linux for home lab or server , it is alternative of ubuntu server but minimal , It is based on debian based kali linux and it is mininmal install of kali and made for VMs .

- ## Tools Included
    - git
    - ssh
    - ftp 
    - samba
    - curl
    - wget
    - parted
    - python3
    - python3-full
    - net-tools

- ## Default Account(user) / Settings / Configs
    
    - ### Default Account
        - Default Username : `n`
        - Sudo user : `n`
        - Default password : `1`  
            change password using `passwd` command  
        - > **Warning:** SSH is enabled by default on port : `22`     
    - ### samba
        - default config `/etc/samba/smb.conf`
        - edited lines
        - ``` 
            [server-def]
            comment = server-def
            path = /home/n
            broseable = yes
            guest ok = yes
            create mask = 777
            directory mask = 777
            writable = yes
            public = yes
            read only = no 
        -   As home directory is exposed for setup with guest allowed (change this  for security)
