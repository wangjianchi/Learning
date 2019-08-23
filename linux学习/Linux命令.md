# Linux 命令
## 基础命令

1. type  类型 
    在文件目录下的命令  外部命令  
    shell内嵌 命令  内部命令
2. file 文件信息  
    ELF  二进制程序
3. yum  安装程序
4. ps-fe  打印进程号
5. pstree 打印进程树
6. echo 输出

## 内嵌命令  
help 查看内部命令文档

```
 job_spec [&]                                         history [-c] [-d 偏移量] [n] 或 history -anrw>
 (( 表达式 ))                                      if 命令; then 命令; [ elif 命令; then 命乾
 . 文件名 [参数]                                 jobs [-lnprs] [任务声明 ...] 或 jobs -x 命
 :                                                    kill [-s 信号声明 | -n 信号编号 | -信号>
 [ 参数... ]                                        let 参数 [参数 ...]
 [[ 表达式 ]]                                      local [option] 名称[=值] ...
 alias [-p] [名称[=值] ... ]                       logout [n]
 bg [任务声明 ...]                                mapfile [-n 计数] [-O 起始序号] [-s 计数]>
 bind [-lpvsPVS] [-m 键映射] [-f 文件名] [-q >  popd [-n] [+N | -N]
 break [n]                                            printf [-v var] 格式 [参数]
 builtin [shell 内嵌 [参数 ...]]                  pushd [-n] [+N | -N | 目录]
 caller [表达式]                                   pwd [-LP]
 case 词 in [模式 [| 模式]...) 命令 ;;]... e>  read [-ers] [-a 数组] [-d 分隔符] [-i 缓冲>
 cd [-L|[-P [-e]]] [dir]                              readarray [-n 计数] [-O 起始序号] [-s 计擾
 command [-pVv] 命令 [参数 ...]                   readonly [-aAf] [name[=value] ...] or readonly -p>
 compgen [-abcdefgjksuv] [-o 选项]  [-A 动作] [>  return [n]
 complete [-abcdefgjksuv] [-pr] [-DE] [-o 选项] [>  select NAME [in 词语 ... ;] do 命令; done
 compopt [-o|+o 选项] [-DE] [名称 ...]            set [-abefhkmnptuvxBCHP] [-o option-name] [--] [a>
 continue [n]                                         shift [n]
 coproc [名称] 命令 [重定向]                   shopt [-pqsu] [-o] [选项名 ...]
 declare [-aAfFgilrtux] [-p] [name[=value] ...]       source 文件名 [参数]
 dirs [-clpv] [+N] [-N]                               suspend [-f]
 disown [-h] [-ar] [任务声明 ...]                 test [表达式]
 echo [-neE] [参数 ...]                             time [-p] 管道
 enable [-a] [-dnps] [-f 文件名] [名称 ...]      times
 eval [参数 ...]                                    trap [-lp] [[参数] 信号声明 ...]
 exec [-cl] [-a 名称] [命令 [参数 ...]] [重㼠 真
 exit [n]                                             type [-afptP] 名称 [名称 ...]
 export [-fn] [名称[=值] ...] 或 export -p        typeset [-aAfFgilrtux] [-p] name[=value] ...
 伪                                                  ulimit [-SHacdefilmnpqrstuvx] [限制]
 fc [-e 编辑器名] [-lnr] [起始] [终结] 或 >  umask [-p] [-S] [模式]
 fg [任务声明]                                    unalias [-a] 名称 [名称 ...]
 for 名称 [in 词语 ... ] ; do 命令; done        unset [-f] [-v] [名称 ...]
 for (( 表达式1; 表达式2; 表达式3 )); do 㼠 until 命令; do 命令; done
 function 名称 { 命令 ; } 或 name () { 命令 >  variables - 一些 shell 变量的名称和含义>
 getopts 选项字符串 名称 [参数]              wait [编号]
 hash [-lr] [-p 路径名] [-dt] [名称 ...]         while 命令; do 命令; done
 help [-dms] [模式 ...]                             { 命令 ; }
 
 ```
 ## 外部命令
 man 查看帮助文档
-  环境变量
    ```/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/root/bin```  外部命令在这些目录下
-  外部命令帮助文档
```
    whereis ifconfig   
    man ls
```

- man可以查看的内容
1.     用户命令（/bin,/usr/bin,/usr/local/bin）
2.     系统调用
3.     库用户
4.     特殊文件（设备文件）
5.     文件格式（配置文件的语法）
6.     游戏
7.     杂项（Miscellaneous）
8.     管理命令（/sbin,/usr/sbin,/usr/local/sbin）



## 常用命令
1. df -h  查看分区信息和容量
2. cp - - 拷贝
3. pwd    查看路径
4. du -sh ./* 查看目录下的文件大小
5. mount /dev/cdrom /mnt 挂载分区

   
 
 
