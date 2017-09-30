# IR - Cheat Sheet

This is a cheatsheet of shortcuts and tips for digital forensics and malware analysis.
It is a personal repository with handy cheatsheets to use when inspecting a machine for digital artifacts.

# Linux
  
  # Places to look at:
    /etc - primary configurations
    /var/log - equivalent to windows event logs
    /home/$USER - user data, info and config
    
    /etc/*-release - 
    /etc/ssh/ssh_host_*_key files - check for dates
    /etc/hostname & /var/log - host name
    /etc/hosts - static i[ assigments 
    /var/lib/dhclient, /var/log/* - dhcp

    /etc/localtime - timezone
    /usr/share/zoneinfo - use zdump
    
    /etc/passwd - UID 0 for admin
    /etc/shadow - md5's 
    /etc/sudoers
    /etc/group
    
    /var/log/wtmp - logins - view with "last"
    
    /var/log/auth.log 
    /var/log/secure
    /var/log/audit/audit.log
    
    Hidden files/dirs names starting with "."
    
    $HOME/.mozilla /firefox/*.default - browsing data
    $HOME/.config/chromium/Default - browsing data
    
    $HOME/.recently-used.xbel - recent files
    $HOME/.thumbnails - thumbnails
    
    $HOME/.bash_history - Note, it can be modified/deleted
    
    /var/log/auth.log - sudo history
    /var/log/sudo.log - sudo history

    $HOME/.ssh:
      known_hosts – hosts user connected to from here
      authorized_keys – public keys used for logins to here
      id_rsa – private keys used to log in elsewhere
      
    # Persistence
      Service start-up scripts:
        /etc/inittab, /etc/init.d, /etc/rc.d (traditional)
        /etc/init.conf, /etc/init (Upstart)
      Scheduled tasks / cron jobs
        /etc/cron*
        /var/spool/cron/*
        
    /etc/inetd.conf
    /etc/xinetd.conf, /etc/xinetd.d
    
  # Windows

    ![Alt text](/ctrl-alt-de1/IR/blob/master/Screen%20Shot%202017-09-30%20at%204.45.32%20PM.png?raw=true "Optional Title")


