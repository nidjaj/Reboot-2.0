## Problem #7 :    create a shell script 

- create a shell script named /root/delvex.sh 
- Make sure it will run /bin/sh shell 
- A user will be running this script my using a command name opensource
- When a user  run like  "opensource  time" it must give current time only
- when it runs like "opensource user"  it will give list of interactive shell users only
- When run like "opensource 100"  it must print "Hello Delvex" 100 times in interval of 1 sec
- If runs like  "opensource windows"  then it must shutdown OS
- If run opensource command without any parameter  then it must show out --
             i)   name of kernel 
             ii)   version of kernel 
             iii)  current date in the format of  /DD/MM/YY
             iv)  name of OS 
             v)   last reboot time 
 
 ##### Note:    each output for last option must be in a separate line   
 
 >vim /root/delvex.sh
```
#!/bin/sh
if [[ $1   ==   "time" ]]
then
        echo "current time `date +%T` "
elif [[ $1   ==   "user" ]]
then
        echo "$SHELL"
elif [[ $1  -eq   100 ]]
then
        i=0
        while [ i -lt 100 ]
        do
                echo "hello delvex"
                sleep 1
                i++
        done
elif [[ $1  ==  "windows" ]]
then
        echo "`/sbin/shutdown -r now `"
else
        echo " kernel is`uname` "        
        echo " version is`uname -r `"
        echo " current date is`date +%x `"
        echo " name of os`uname -o`"
        echo "last reboot time`who -b`"
fi
```



