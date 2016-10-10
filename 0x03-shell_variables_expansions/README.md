Create a script that creates an alias.

Name: ls
Value: rm *
julien@ubuntu:/tmp/0x03$ ls
0-alias  file1  file2
julien@ubuntu:/tmp/0x03$ ./0-alias 
julien@ubuntu:/tmp/0x03$ ls
julien@ubuntu:/tmp/0x03$ \ls
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 0-alias
  Done?  

Help!
1. Hello you mandatory

Create a script that prints hello user, where user is the current Linux user.

julien@ubuntu:/tmp/0x03$ id
uid=1000(julien) gid=1000(julien) groups=1000(julien),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),113(lpadmin),128(sambashare)
julien@ubuntu:/tmp/0x03$ ./1-hello_you 
hello julien
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 1-hello_you
  Done?  

Help!
2. The path to success is to take massive, determined action mandatory

Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.

julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ source ./2-path 
julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/action
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 2-path
  Done?  

Help!
3. If the path be beautiful, let us not ask where it leads mandatory

Create a script that counts the number of directories in the PATH.

julien@ubuntu:/tmp/0x03$ echo $PATH
/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
julien@ubuntu:/tmp/0x03$ . ./3-paths 
11
julien@ubuntu:/tmp/0x03$ PATH=/home/julien/bin:/home/julien/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:::::/hello
julien@ubuntu:/tmp/0x03$ . ./3-paths 
12
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 3-paths
  Done?  

Help!
4. Global variables mandatory

Create a script that lists environment variables.

julien@ubuntu:/tmp/0x03$ source ./4-global_variables
CC=gcc
CDPATH=.:~:/usr/local:/usr:/
CFLAGS=-O2 -fomit-frame-pointer
COLORTERM=gnome-terminal
CXXFLAGS=-O2 -fomit-frame-pointer
DISPLAY=:0
DOMAIN=hq.garrels.be
e=
TOR=vi
FCEDIT=vi
FIGNORE=.o:~
G_BROKEN_FILENAMES=1
GDK_USE_XFT=1
GDMSESSION=Default
GNOME_DESKTOP_SESSION_ID=Default
GTK_RC_FILES=/etc/gtk/gtkrc:/nethome/franky/.gtkrc-1.2-gnome2
GWMCOLOR=darkgreen
GWMTERM=xterm
HISTFILESIZE=5000
history_control=ignoredups
HISTSIZE=2000
HOME=/nethome/franky
HOSTNAME=octarine.hq.garrels.be
INPUTRC=/etc/inputrc
IRCNAME=franky
JAVA_HOME=/usr/java/j2sdk1.4.0
LANG=en_US
LDFLAGS=-s
LD_LIBRARY_PATH=/usr/lib/mozilla:/usr/lib/mozilla/plugins
LESSCHARSET=latin1
LESS=-edfMQ
LESSOPEN=|/usr/bin/lesspipe.sh %s
LEX=flex
LOCAL_MACHINE=octarine
LOGNAME=franky
[...]
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 4-global_variables
  Done?  

Help!
5. Local variables mandatory

Create a script that lists all local variables.

julien@ubuntu:/tmp/0x03$ . ./5-local_variables
BASH=/bin/bash
BASHOPTS=checkwinsize:cmdhist:complete_fullquote:expand_aliases:extglob:extquote:force_fignore:histappend:interactive_comments:progcomp:promptvars:sourcepath
BASH_ALIASES=()
BASH_ARGC=()
BASH_ARGV=()
BASH_CMDS=()
BASH_COMPLETION_COMPAT_DIR=/etc/bash_completion.d
BASH_LINENO=()
BASH_REMATCH=()
BASH_SOURCE=()
BASH_VERSINFO=([0]="4" [1]="3" [2]="46" [3]="1" [4]="release" [5]="x86_64-pc-linux-gnu")
BASH_VERSION='4.3.46(1)-release'
CLUTTER_IM_MODULE=xim
COLUMNS=133
COMPIZ_CONFIG_PROFILE=ubuntu
COMP_WORDBREAKS=$' \t\n"\'><=;|&(:'
DBUS_SESSION_BUS_ADDRESS=unix:abstract=/tmp/dbus-Fg27Lr20bq
DEFAULTS_PATH=/usr/share/gconf/ubuntu.default.path
DESKTOP_SESSION=ubuntu
[...]
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 5-local_variables
  Done?  

Help!
6. Local variable mandatory

Create a script that creates a new local variable.

Name: BETTY
Value: Holberton
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 6-create_local_variable
  Done?  

Help!
7. Global variable mandatory

Create a script that creates a new global variable.

Name: HOLBERTON
Value: Betty
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 7-create_global_variable
  Done?  

Help!
8. Every addition to true knowledge is an addition to human power mandatory

Write a script that adds 128 to the value stored in the environment variable TRUEKNOWLEDGE, and prints the result, followed by a new line.

julien@production-503e7013:~$ export TRUEKNOWLEDGE=1209
julien@production-503e7013:~$ ./8-true_knowledge | cat -e
1337$
julien@production-503e7013:~$
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 8-true_knowledge
  Done?  

Help!
9. Divide and rule mandatory

Write a script that divides POWER by DIVIDE and prints the result, followed by a new line.

POWER and DIVIDE are environment variables
julien@production-503e7013:~$ export POWER=42784
julien@production-503e7013:~$ export DIVIDE=32
julien@production-503e7013:~$ ./9-divide_and_rule | cat -e
1337$
julien@production-503e7013:~$
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 9-divide_and_rule
  Done?  

Help!
10. Love is anterior to life, posterior to death, initial of creation, and the exponent of breath mandatory

Write a script that computes and displays the result of BREATH to the power LOVE

BREATH and LOVE are environment variables
The script should display the result, followed by a new line
julien@production-503e7013:~/$ export BREATH=4
julien@production-503e7013:~/$ export LOVE=3
julien@production-503e7013:~/$ ./10-love_exponent_breath
64
julien@production-503e7013:~/$
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 10-love_exponent_breath
  Done?  

Help!
11. There are 10 types of people in the world -- Those who understand binary, and those who don't mandatory

Write a script that converts a number from base 2 to base 10.

The number in base 2 is stored in the environment variable BINARY
The script should display the number in base 10, followed by a new line
julien@production-503e7013:~/$ export BINARY=10100111001
julien@production-503e7013:~/$ ./11-binary_to_decimal
1337
julien@production-503e7013:~/$
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 11-binary_to_decimal
  Done?  

Help!
12. Combination mandatory

Create a script that prints all possible combinations of two letters, except oo.

Letters are lower cases, from a to z
One combinaison per line
The output should be alpha ordered, starting with aa
Do not print oo
Your script file should contain maximum 64 characters
julien@ubuntu:/tmp/0x03$ echo $((26 ** 2 -1))
675
julien@ubuntu:/tmp/0x03$ ./12-combinations | wc -l
675
julien@ubuntu:/tmp/0x03$ 
julien@ubuntu:/tmp/0x03$ ./12-combinations | tail -303 | head -10
oi
oj
ok
ol
om
on
op
oq
or
os
julien@ubuntu:/tmp/0x03$ 
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 12-combinations
  Done?  

Help!
13. Floats mandatory

Write a script that prints a number with two decimal places.

The number will be stored in the environment variable NUM.

ubuntu@ip-172-31-63-244:~/0x03$ export NUM=0
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
0.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=98
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
98.00
ubuntu@ip-172-31-63-244:~/0x03$ export NUM=3.14159265359
ubuntu@ip-172-31-63-244:~/0x03$ ./13-print_float
3.14
ubuntu@ip-172-31-63-244:~/0x03$
Repo:

GitHub repository: holbertonschool-sysadmin_devops
Directory: 0x03-shell_variables_expansions
File: 13-print_float
  Done?  

Help!
14. What happens when you type `ls *.c` mandatory

Write a blog post describing step by step what happens when you type ls *.c and hit Enter in your shell. Try to explain every step you know of, and give examples. A total beginner should understand what you have written.

Have at least one picture, at the top of the blog post
Publish your blog post on Medium or LinkedIn
Share your blog post at least on Twitter and LinkedIn
When done, please fill this form

  Done?  

Help!
15. What is the difference between a hard link and a symbolic link? mandatory

Write a blog post explaining what are hard and symbolic links on Linux, how to create them, and what is the difference between the two. Use examples to illustrate.

Have at least one picture, at the top of the blog post
Publish your blog post on Medium or LinkedIn
Share your blog post at least on Twitter and LinkedIn
When done, please fill this form