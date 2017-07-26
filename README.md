### Nginx    
```
ps -ef | grep nginx
```
显示当前nginx的目录      
`ps` ps命令用于报告当前系统的进程状态。可以搭配kill指令随时中断、删除不必要的程序。ps命令是最基本同时也是非常强大的进程查看命令，使用该命令可以确定有哪些进程正在运行和运行的状态、进程是否结束、进程有没有僵死、哪些进程占用了过多的资源等等，总之大部分信息都是可以通过执行该命令得到的。      
`-e` 选项效果和-A相同，意为显示所有程序         
`-f` 显示UID、PPIP、C 与 STIME栏位   
`grep` grep（global search regular expression(RE) and print out the line，全面搜索正则表达式并把行打印出来）是一种强大的文本搜索工具，它能使用正则表达式搜索文本，并把匹配的行打印出来     
```
xxxx/nginx -c xxxx/nginx.conf
```
第一个参数是ps -ef | grep nginx的结果，`-c`指使用第二个参数所指的config文件去运行第一个参数所指目录下的nginx     
