# my_Server

## adam@adam-HP-EliteBook-840-G3:~$ ssh root@157.173.105.219
root@157.173.105.219's password: 
Welcome to Ubuntu 22.04.4 LTS (GNU/Linux 5.15.0-25-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro
New release '24.04.1 LTS' available.
Run 'do-release-upgrade' to upgrade to it.

  _____
 / ___/___  _  _ _____ _   ___  ___
| |   / _ \| \| |_   _/ \ | _ )/ _ \
| |__| (_) | .` | | |/ _ \| _ \ (_) |
 \____\___/|_|\_| |_/_/ \_|___/\___/

Welcome!

This server is hosted by Contabo. If you have any questions or need help,
please don't hesitate to contact us at support@contabo.com.

Last login: Tue Sep 10 17:50:24 2024 from 197.250.224.82
root@vmi2137201:~# mkdir client
root@vmi2137201:~# cd client/
root@vmi2137201:~/client# git clone git@github.com:AdamMashaka/livescore_yetu.git
Command 'git' not found, but can be installed with:
apt install git
root@vmi2137201:~/client# sudo apt update
Hit:1 http://asi-fs-d.contabo.net/ubuntu jammy InRelease
Hit:2 http://asi-fs-d.contabo.net/ubuntu jammy-updates InRelease
Hit:3 http://asi-fs-d.contabo.net/ubuntu jammy-backports InRelease
Get:4 http://security.ubuntu.com/ubuntu jammy-security InRelease [129 kB]
Fetched 129 kB in 0s (289 kB/s)                        
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
8 packages can be upgraded. Run 'apt list --upgradable' to see them.
root@vmi2137201:~/client# sudo apt-get install git
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  git-man libcurl3-gnutls liberror-perl patch
Suggested packages:
  git-daemon-run | git-daemon-sysvinit git-doc git-email git-gui gitk gitweb
  git-cvs git-mediawiki git-svn diffutils-doc
The following NEW packages will be installed:
  git git-man libcurl3-gnutls liberror-perl patch
0 upgraded, 5 newly installed, 0 to remove and 8 not upgraded.
Need to get 4,539 kB of archives.
After this operation, 22.0 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://asi-fs-d.contabo.net/ubuntu jammy-updates/main amd64 libcurl3-gnutls amd64 7.81.0-1ubuntu1.17 [284 kB]
Get:2 http://asi-fs-d.contabo.net/ubuntu jammy/main amd64 liberror-perl all 0.17029-1 [26.5 kB]
Get:3 http://asi-fs-d.contabo.net/ubuntu jammy-updates/main amd64 git-man all 1:2.34.1-1ubuntu1.11 [955 kB]
Get:4 http://asi-fs-d.contabo.net/ubuntu jammy-updates/main amd64 git amd64 1:2.34.1-1ubuntu1.11 [3,165 kB]
Get:5 http://asi-fs-d.contabo.net/ubuntu jammy/main amd64 patch amd64 2.7.6-7build2 [109 kB]
Fetched 4,539 kB in 0s (21.0 MB/s)
Selecting previously unselected package libcurl3-gnutls:amd64.
(Reading database ... 67850 files and directories currently installed.)
Preparing to unpack .../libcurl3-gnutls_7.81.0-1ubuntu1.17_amd64.deb ...
Unpacking libcurl3-gnutls:amd64 (7.81.0-1ubuntu1.17) ...
Selecting previously unselected package liberror-perl.
Preparing to unpack .../liberror-perl_0.17029-1_all.deb ...
Unpacking liberror-perl (0.17029-1) ...
Selecting previously unselected package git-man.
Preparing to unpack .../git-man_1%3a2.34.1-1ubuntu1.11_all.deb ...
Unpacking git-man (1:2.34.1-1ubuntu1.11) ...
Selecting previously unselected package git.
Preparing to unpack .../git_1%3a2.34.1-1ubuntu1.11_amd64.deb ...
Unpacking git (1:2.34.1-1ubuntu1.11) ...
Selecting previously unselected package patch.
Preparing to unpack .../patch_2.7.6-7build2_amd64.deb ...
Unpacking patch (2.7.6-7build2) ...
Setting up libcurl3-gnutls:amd64 (7.81.0-1ubuntu1.17) ...
Setting up liberror-perl (0.17029-1) ...
Setting up patch (2.7.6-7build2) ...
Setting up git-man (1:2.34.1-1ubuntu1.11) ...
Setting up git (1:2.34.1-1ubuntu1.11) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for libc-bin (2.35-0ubuntu3.8) ...
root@vmi2137201:~/client# git clone git@github.com:AdamMashaka/livescore_yetu.git
Cloning into 'livescore_yetu'...
The authenticity of host 'github.com (140.82.121.3)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
remote: Enumerating objects: 9894, done.
remote: Counting objects: 100% (9894/9894), done.
remote: Compressing objects: 100% (6480/6480), done.
remote: Total 9894 (delta 2287), reused 9869 (delta 2270), pack-reused 0 (from 0)
Receiving objects: 100% (9894/9894), 18.41 MiB | 12.27 MiB/s, done.
Resolving deltas: 100% (2287/2287), done.
root@vmi2137201:~/client# ls
livescore_yetu
root@vmi2137201:~/client# 

