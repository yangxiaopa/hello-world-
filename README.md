# hello-world-
just  another repository 
file_path ='C:/Users/YSS/Desktop/file_Tcl/20co.tcl'
with open(file_path) as file_object: #让pyth妥善的打开和关闭文件，不占用内存！    
    for line in file_object:
        print(line.rstrip()) #rstrip()用来消除空白行
