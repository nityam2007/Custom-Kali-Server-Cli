# Kali-Server

- ## What is it ?
It is a simple customised linux for home lab or server , it is alternative of ubuntu server but minimal , It is based on debian based kali linux and it is mininmal install of kali and made for VMs . Both Cli and Gui are there pre set for your project 

- ## Default Account(user) / Settings / Configs (CLI-GUI)
    
    - ### Default Account
        - Default Username : `n`
        - Sudo user : `n`
        - Default password : `1`  
            change password using `passwd` command  
        - > **Warning:** SSH is enabled by default on port : `22`  
        - hostname : `kali`   
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


- # CLI
- ## VM requirments MIN 
    - Ram : `2GB`
    - Cpu : `2 Vcore` (depends of processor(changable))
    - storage : `20GB`
- ## VM requirments ANY
    - Ram : `4GB`
    - Cpu : `3 Vcore` (depends of processor(changable))
    - storage : `20GB` (MIN(Extendable))
- ## Tools Included **Cli only**
    - ### MIN
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
        - mkfs
        - fdisk
        - vm tools
    - ### Docker + Portainer + MIN
        - docker (sudo)
        - docker (service) 
        - docker-compose
        - Portainer CE (Not Config) `localhost:9000`
        - othere tools in min
    - ### Code-server + Docker + Portainer + MIN
        - code-server 
            - `localhost:8443`
            - password = `password`
            - sudo pass = `password`
            - Image used `lscr.io/linuxserver/code-server:latest`
        - othere tools in docker
