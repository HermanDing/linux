### 卸载软件
找到此软件名称,然后sudo apt-get purge ......(点点为为程序名称),purge参数为彻底删除文件,然后sudo apt-get autoremove,sudo apt-get clean和dpkg -l |grep ^rc|awk '{print $2}' |sudo xargs dpkg -P 两条命令来清除残余的配置文件
```
sudo apt-get purge <program_name>
sudo apt-get autoremove
sudo apt-get clean
dpkg -l |grep ^rc|awk '{print $2}' |sudo xargs dpkg -P
```
### 快速打开各类型文件
```
xdg-open { file | URL } 
```