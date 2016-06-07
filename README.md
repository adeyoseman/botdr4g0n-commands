# botdr4g0n-commands
command line for botdrag0n ssh


root@siftworkstation:~# cd day5/
root@siftworkstation:~/day5# git clone https://github.com/mh4x0f/botdr4g0n.git
Cloning into 'botdr4g0n'...
remote: Counting objects: 158, done.
remote: Total 158 (delta 0), reused 0 (delta 0), pack-reused 158
Receiving objects: 100% (158/158), 34.91 KiB | 0 bytes/s, done.
Resolving deltas: 100% (63/63), done.
Checking connectivity... done.
root@siftworkstation:~/day5# cd botdr4g0n
root@siftworkstation:~/day5/botdr4g0n# pip install -r requirements.tx
Could not open requirements file: [Errno 2] No such file or directory: 'requirements.tx'
Storing debug log for failure in /root/.pip/pip.log
root@siftworkstation:~/day5/botdr4g0n# dir
botdr4g0n.py  common  helpers  lincese.txt  README.md  requirements.txt
root@siftworkstation:~/day5/botdr4g0n# dir
botdr4g0n.py  common  helpers  lincese.txt  README.md  requirements.txt
root@siftworkstation:~/day5/botdr4g0n# pip install -r requirements.tx
Could not open requirements file: [Errno 2] No such file or directory: 'requirements.tx'
Storing debug log for failure in /root/.pip/pip.log
root@siftworkstation:~/day5/botdr4g0n# pip install requirements.tx
Downloading/unpacking requirements.tx
  Could not find any downloads that satisfy the requirement requirements.tx
Cleaning up...
No distributions at all found for requirements.tx
Storing debug log for failure in /root/.pip/pip.log
root@siftworkstation:~/day5/botdr4g0n# ls
botdr4g0n.py  common  helpers  lincese.txt  README.md  requirements.txt
root@siftworkstation:~/day5/botdr4g0n# ./botdr4g0n.py 
Traceback (most recent call last):
  File "./botdr4g0n.py", line 2, in <module>
    from common.ConsoleUI import Console
  File "/root/day5/botdr4g0n/common/ConsoleUI.py", line 25, in <module>
    from tabulate import tabulate
ImportError: No module named tabulate
root@siftworkstation:~/day5/botdr4g0n# chmod +x botdr4g0n.py 
root@siftworkstation:~/day5/botdr4g0n# ./botdr4g0n.py 
Traceback (most recent call last):
  File "./botdr4g0n.py", line 2, in <module>
    from common.ConsoleUI import Console
  File "/root/day5/botdr4g0n/common/ConsoleUI.py", line 25, in <module>
    from tabulate import tabulate
ImportError: No module named tabulate
root@siftworkstation:~/day5/botdr4g0n# chmod +x requirements.tx
chmod: cannot access ‘requirements.tx’: No such file or directory
root@siftworkstation:~/day5/botdr4g0n# pip install requirements.tx
Downloading/unpacking requirements.tx
  Could not find any downloads that satisfy the requirement requirements.tx
Cleaning up...
No distributions at all found for requirements.tx
Storing debug log for failure in /root/.pip/pip.log
root@siftworkstation:~/day5/botdr4g0n# pip install requirements.tx
Downloading/unpacking requirements.tx
  Could not find any downloads that satisfy the requirement requirements.tx
Cleaning up...
No distributions at all found for requirements.tx
Storing debug log for failure in /root/.pip/pip.log
root@siftworkstation:~/day5/botdr4g0n# pip install -r requirements.txt
Downloading/unpacking tabulate (from -r requirements.txt (line 1))
  Downloading tabulate-0.7.5.tar.gz
  Running setup.py (path:/tmp/pip_build_root/tabulate/setup.py) egg_info for package tabulate
    
Requirement already satisfied (use --upgrade to upgrade): pexpect in /usr/lib/python2.7/dist-packages (from -r requirements.txt (line 2))
Requirement already satisfied (use --upgrade to upgrade): pysqlite in /usr/lib/python2.7/dist-packages (from -r requirements.txt (line 3))
Installing collected packages: tabulate
  Running setup.py install for tabulate
    
    Installing tabulate script to /usr/local/bin
  Could not find .egg-info directory in install record for tabulate (from -r requirements.txt (line 1))
Successfully installed tabulate
Cleaning up...
root@siftworkstation:~/day5/botdr4g0n# ./botdr4g0n.py 

  _           _      _      _  _          ___
 | |__   ___ | |_ __| |_ __| || |   __ _ / _ \ _ __
 | '_ \ / _ \| __/ _` | '__| || |_ / _` | | | | '_ |
 | |_) | (_) | || (_| | |  |__   _| (_| | |_| | | | |
 |_.__/ \___/ \__\__,_|_|     |_|  \__, |\___/|_| |_|
                                   |___/
    Version: 0.1.3
    Author:  Marcos Nesster (@mh4x0f)

:: 
:: register
usage: register [-h] [--host <Host>] [--pass <Password>] [-u <user>]
                [-p <Port>]

add bot on database clients

optional arguments:
  -h, --help            show this help message and exit
  --host <Host>         ipaddress/host/dns connect ssh
  --pass <Password>     password ssh client
  -u <user>, --user <user>
                        delete all bot registered
  -p <Port>, --port <Port>
                        port connect ssh
:: register --host 192.168.20.29 -u malware --pass malware -p 22
[*] Insert Data: SQL statement will insert a new row
[+] credentials ssh added with success
:: register --host 192.168.20.28 -u malware --pass malware -p 22
[*] Insert Data: SQL statement will insert a new row
[+] credentials ssh added with success
:: register --host 192.168.20.30 -u malware --pass malware -p 22
[*] Insert Data: SQL statement will insert a new row
[+] credentials ssh added with success
:: register --host 192.168.20.45 -u malware --pass malware -p 22
[*] Insert Data: SQL statement will insert a new row
[+] credentials ssh added with success
:: help

[*] Available Commands:
=======================

    Commands	 Description
    --------	 -----------
    check     	 test all agents login ssh  
    del       	 delete bot using <id>/all 
    execute   	 execute command on agents
    exit      	 exit the program.
    help      	 show this help 
    interact  	 interact with one/all agents 
    jobs      	 list/kill jobs running on agents 
    list      	 list/check/filter list agents on database 
    register  	 add bot on database 
    sysinfo   	 print information session on agents


:: check

[*] Available Bots:
===================

  Id  Host             Port  User     Password    Data                 Status
----  -------------  ------  -------  ----------  -------------------  --------
   1  192.168.20.29      22  malware  malware     2016-06-07 09:59:52  [ON]
   2  192.168.20.28      22  malware  malware     2016-06-07 10:00:09  [OFF]
   3  192.168.20.30      22  malware  malware     2016-06-07 10:00:15  [OFF]
   4  192.168.20.45      22  malware  malware     2016-06-07 10:00:21  [OFF]


[*] Online Agents: 1
:: interact -a
[*] Checking Creadentials SHH...
[*] Agent::192.168.20.29 [ON]

:: Traceback (most recent call last):
  File "./botdr4g0n.py", line 8, in <module>
    shell.cmdloop(banner(version,author))
  File "/usr/lib/python2.7/cmd.py", line 130, in cmdloop
    line = raw_input(self.prompt)
KeyboardInterrupt
root@siftworkstation:~/day5/botdr4g0n# execute 
execute: command not found
root@siftworkstation:~/day5/botdr4g0n# ./botdr4g0n.py 

  _           _      _      _  _          ___
 | |__   ___ | |_ __| |_ __| || |   __ _ / _ \ _ __
 | '_ \ / _ \| __/ _` | '__| || |_ / _` | | | | '_ |
 | |_) | (_) | || (_| | |  |__   _| (_| | |_| | | | |
 |_.__/ \___/ \__\__,_|_|     |_|  \__, |\___/|_| |_|
                                   |___/
    Version: 0.1.3
    Author:  Marcos Nesster (@mh4x0f)

:: execute
usage: execute [-h] [-c "cmd"] [-j]

execute command's on agents

optional arguments:
  -h, --help            show this help message and exit
  -c "cmd", --cmd "cmd"
                        execute command on bot
  -j, --job             running command as job
:: interact
usage: interact [-h] [-i <id>] [-a] [-s] [-q]

interact with one/all agents

optional arguments:
  -h, --help          show this help message and exit
  -i <id>, --id <id>  connect with particular agent SSH by id
  -a, --all           connect all agent Available
  -s, --shell         connect Remote shell bin/bash
  -q, --quit          quit all connections with agents
:: interact -a
[*] Checking Creadentials SHH...
\[*] Agent::192.168.20.29 [ON]

:: execute -h -c "reboot" 
usage: execute [-h] [-c "cmd"] [-j]

execute command's on agents

optional arguments:
  -h, --help            show this help message and exit
  -c "cmd", --cmd "cmd"
                        execute command on bot
  -j, --job             running command as job
:: execute -h -c "reboot"  -j
usage: execute [-h] [-c "cmd"] [-j]

execute command's on agents

optional arguments:
  -h, --help            show this help message and exit
  -c "cmd", --cmd "cmd"
                        execute command on bot
  -j, --job             running command as job
:: execute -h --c "reboot" --j
usage: execute [-h] [-c "cmd"] [-j]

execute command's on agents

optional arguments:
  -h, --help            show this help message and exit
  -c "cmd", --cmd "cmd"
                        execute command on bot
  -j, --job             running command as job
:: execute -h --cmd "reboot" --j
usage: execute [-h] [-c "cmd"] [-j]

execute command's on agents

optional arguments:
  -h, --help            show this help message and exit
  -c "cmd", --cmd "cmd"
                        execute command on bot
  -j, --job             running command as job
:: execute -cmd "reboot" 
usage: execute [-h] [-c "cmd"] [-j]
execute: error: unrecognized arguments: reboot
:: execute -cmd "shutdown -r" 
usage: execute [-h] [-c "cmd"] [-j]
execute: error: unrecognized arguments: shutdown -r
:: execute -c "shutdown -r" 

[*] HOST::192.168.20.29
=======================



Broadcast message from malware@siftworkstation
	(/dev/pts/22) at 10:14 ...

The system is going down for reboot NOW!
