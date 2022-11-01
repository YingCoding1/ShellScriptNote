# lecture1

https://missing.csail.mit.edu/2020/course-shell/

## what's shell?

A **Shell** provides you with an interface to the Unix system. Shell is an environment in which we can run our commands, programs, and shell scripts. There are different flavors of a shell, just as there are different flavors of operating systems.

![image-20221031200944204](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20221031200944204.png)

![image-20221031201705601](C:\Users\Lenovo\AppData\Roaming\Typora\typora-user-images\image-20221031201705601.png)

There are several shells are available for Linux systems like –

- [BASH (Bourne Again SHell)](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) – It is most widely used shell in Linux systems. It is used as default login shell in Linux systems and in macOS. It can also be installed on Windows OS.
- [CSH (C SHell)](https://en.wikipedia.org/wiki/C_shell) – The C shell’s syntax and usage are very similar to the C programming language.
- [KSH (Korn SHell)](https://en.wikipedia.org/wiki/Korn_shell) – The Korn Shell also was the base for the POSIX Shell standard specifications etc.

## Shell script introduction

#### first shell script: new a shell script and print helloworld

```
touch helloworld.sh
vim helloworld.sh
```



```sh
#!/bin/bash 
# to set the interpreter,alert the system that a shell script is being started.

# Author : 
# Script follows here:
echo "helloworld"
```

execute the script

method 1

```
//relative path
sh helloworld.sh
//or
bash helloworld.sh  
//or
//absolute path
sh /balabala/balabala/helloworld.sh 
//or
bash /balabala/balabala/helloworld.sh
```

method2

```
chmod 777 helloworld.sh //give the permision
$ ./helloworld.sh
or
$ /home/balabla/helloworld.sh
```

because the method 1 is using the bash interpreter so it don't need the permission of the script but the method 2 is execute the script by it self so it needs the permission



#### second shell script : new a peace.txt in /home/bala/ and add "i love you" in peace.txt



```
touch batch.sh
vim batch.sh

```



```sh
#!/bin/bash
cd /home/bala/
touch peace.txt
echo "i love you" >> peace.txt 

```

```
bash batch.sh
```

then we go to that directory and cat peace.txt 

it will be i love you



























































