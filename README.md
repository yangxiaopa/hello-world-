# hello-world-
just  another repository 
file_path ='C:/Users/YSS/Desktop/file_Tcl/20co.tcl'
with open(file_path) as file_object: #让pyth妥善的打开和关闭文件，不占用内存！    
    for line in file_object:
        print(line.rstrip()) #rstrip()用来消除空白行


file_path1='C:/Users/YSS/Desktop/file_Tcl/Exam1.tcl'
try:
    with open(file_path1) as file_object1:
        contents=file_object1.read()        
except FileNotFoundError:
    print('sorry,the file '+file_path1+' does not exist.')
else:
    #for line in file_object1:
        print(contents)
        
#避免读取空文件夹失效！        
file_path1='C:/Users/YSS/Desktop/file_Tcl/Exam1.tcl'
try:
    with open(file_path1) as file_object1:
        contents=file_object1.read()     
except FileNotFoundError:
    print('sorry,the file '+file_path1+' does not exist.')
else:
    print(contents)
    
#jj提供脚本    
f=open('C:/Users/YSS/Desktop/file_Tcl/Exam1.tcl','r')
o=open('C:/Users/YSS/Desktop/file_Tcl/NEWexam.tcl','w')
for line in f.readlines():
	if line.startswith("node"):
		strs=line.strip().split(" ")
		slist=strs[1:]
		o.write('node ('+slist[0]+','+slist[1]+','+slist[2]+','+slist[3]+')\n')
f.close()
o.close()    
    
python impoort 用法
1.import somemodule #导入某个模块 例如 ：
	import sys #导入模块
	sys.path.append('F:\openseespy') #提供搜索路径
2.from somemodule import somefunction #导入模块的somefunction方法
3.from somemodule import function1,function2,...  #导入模块的function1，function2等方法
4.from somemodule import * #导入模块的所有方法

关键字as的用法
import somemodule as moduleA 
from somemodule import somefunction as functionA
接下来可直接调用moduleA、functionA 例如： 
import numpy as np 
from opensees import *
module: A module is a file containing python definitions and statement. 所以module就是一个.py文件 
package:包含.py文件的文件夹，文件夹中还包含一个特殊文件_.init_.py

import sys
sys.path.append('F:\openseespy')
变量sys.path是一个字符串列表，用于确定解释器的模块搜索路径。

以下为示例，查看函数的用法。
import string
help(string)







