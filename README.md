# Python
Python Scripting code

#!/usr/bin/env python3
import subprocess
value = subprocess.call("root_inode=$(df -i|xargs -n1|grep -xB1 '/'|head -1|tr -d %)", shell=True)
#print(value)
if  (value <=  1) and (value == 0):
        print("value is 0")
else:
        print("value is not 0")
