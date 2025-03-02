#
```
```

- pipiline與 redirection

https://dylan237.github.io/linux-basic.html

- [Linux 命令大全](https://www.runoob.com/linux/linux-command-manual.html)
- [Linux 常用命令全拼](https://www.runoob.com/w3cnote/linux-command-full-fight.html)

# 資料夾|目錄 與 檔案 處理
```
/  ==> 根目錄(linux最上層目錄)
.  ==> 表示該層目錄
.. ==> 表示上層目錄
-  ==> 表示前一個工作目錄
~  ==> 表示『目前使用者身份』所在的家目錄
```
## 
- [mkdir(Make Directory) ==>建立資料夾]()
- [rmdir(Remove Directory)==>刪除資料夾]()
- [rm(remove) ==>刪除檔案或資料夾]()
- [cp ==> 複製檔案]

## 資料顯示[顯示檔案或資料夾的內容(content)]

- ls(list directory content)列出資料夾下內容[包括檔案與子目錄]
- more ==> 以全螢幕的方式 按頁 顯示文字檔案的內容
- less ==>
- [head ==> 顯示檔案的開頭的內容]()
- [tail ==> 輸入檔案中的尾部內容]()
- [file ==> 檔案類型]
- echo ==> 印出一行文本

- sort ==>將檔案內容依排列，再輸到終端[預設是使用 ASCII 碼的次序排列]


## 文字編輯工具|寫程式也可以用
- nano
- vim
- gedit

## 搜尋檔案...
- find ==>找尋吻合條件的檔案
- locate
- which
- grep ==> 用關鍵字找尋檔案

## 檔案壓縮解壓縮與打包
- gzip
- tar

## file descriptors and redirection
- File descriptors are integers associated with the input and output streams. 

| name | Full name  | file descriptors |
| ----| -------|-------|
|stdin  |  standard input  |  0 |
|stdout |  standard output   |  1 |
|stderr| standard error   |  2 |

```
echo "This is a sample text 1" > temp.txt

echo "This is sample text 2" >> temp.txt

cat temp.txt

redirect stderr to one file and stdout to another file.
==>  cmd 2>stderr.txt 1>stdout.txt

https://www.packtpub.com/product/linux-shell-scripting-cookbook-third-edition/9781785881985
```
# 使用者(user)與群組(group)管理
```
建立+移除+更新 使用者  .....

https://www.runoob.com/linux/linux-user-manage.html
```
- adduser == > 新增使用者(user)帳號

- useradd == > 建立使用者(user)帳號
- userdel == > 刪除使用者(user)帳號
- usermod == > 修改使用者(user)帳號


- groupdel(group delete) ==> 刪除群組。
- groupmod(group modify) ==> 更改群組識別碼或名稱。


- id ==> 顯示使用者(user)的ID，以及所屬群組(group)的ID。
- whoami==> 顯示使用者(user)名稱

- passwd ==> 更改密碼
- su(super user|Swith user) ==> 變更使用者(user)身份
- sudo ==> 以其他身份來執行指令。


# 權限管理

- chmod ==> 變更文件或目錄的權限
- chown ==> 變更文件或目錄的擁有者或所屬群組
- chgrp ==> 變更文件或目錄的所屬群組。

# 網路連線指令

- telnet | ssh
- ftp | sftp
- wget
- netstat

# 軟體管理(套件管理) package management tools
```
安裝+移除+更新 軟體  .....
不同發行版本會提供不同套件管理工具
centos  ==> yum
debian  ==> dpkg | apt(Advanced Package Tool)
red hat ==> rpm
```

- [Ubuntu Server Guide指令](https://ubuntu.com/server/docs)

- insmod(Install module)
- rmmod(Remove module)
- lsmod(List module)

# 硬體管理

## 磁碟管理

- df(disk full)  ==>  列出檔案系統的整體磁片使用量
- du(disk usage) ==> 檢查磁碟空間使用量
- fdisk ==> 用於磁碟分割


# 行程(process)管理

- ps(process status) ==> 報告程序狀況
- pstree(process status tree) ==> 以樹狀圖顯示程序
- top  ==> 顯示，管理執行中的程序

- kill ==>刪除執行中的程序或工作

- chsh(change shell) ==> 更換登入系統時使用的shell。
- exit ==> 退出目前的shell。

# 行程調校

# 系統管理

- uname ==> 顯示系統信息

- date ==> 顯示或設置系統時間與日期

- free ==> 顯示記憶體狀態。

- halt ==> 關閉系統
- shutdown ==> 系統關機指令
- reboot ==> 重新開機



- w   ==> 顯示目前登入系統的使用者(user)信息。
- who ==> 顯示目前登入系統的使用者(user)信息。

- last ==> 列出目前與過去登入系統的用戶相關信息
- lastb ==> 列出登入系統失敗的用戶相關信息

# environment variables環境變數

```
PATH=/usr/bin;/bin 
LD_LIBRARY_PATH=/usr/lib;/lib
```
```
export PATH=/opt/myapp/bin:$PATH 
export LD_LIBRARY_PATH=/opt/myapp/lib;$LD_LIBRARY_PATH
```
```
PATH=/opt/myapp/bin:/usr/bin:/bin 
LD_LIBRARY_PATH=/opt/myapp/lib:/usr/lib;/lib
```


procinfo(process information)




