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
    
f=open('/home/jiangjun/Exam01.tcl','r')
o=open('/home/jiangjun/sbyangsuo.txt','w')
for line in f.readlines():
	if line.startswith("node"):
		strs=line.strip().split(" ")
		slist=strs[1:]
		o.write('node ('+slist[0]+','+slist[1]+','+slist[2]+','+slist[3]+')\n')
f.close()
o.close()    
    
