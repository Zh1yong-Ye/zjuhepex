# CMS@zju
For new zju hep-ex student

# Computing Resource
## zju clutser
目前组内有四台计算服务器和一台存储服务器。

服务器的基本信息：

- IP：10.22.81.166
- SSH端口映射：10122~14122

SSH以及硬件管理需用路由器拨号的静态IP+端口号访问，例如：

连接node1的ssh：ssh user@10.22.81.166 -p 11122

可以通过修改`.ssh/config`以及 [设置SSH免密登陆](https://atomlab.org/posts/code/ssh-trick/)在VScode上获得比较好的登陆体验。
```
Host node1
    HostName 10.22.81.166
    User User
    Port 11122
```
### Tips
- 因为我们是小作坊，没有使用HTcondor协调作业。运行大作业的时候需要提前看服务器运行状况，和组内成员协商任务。
- 可以通过`htop`查看服务器状态和任务运行情况。
    - 不要让单个任务的磁盘读写超过150M。
    - 不要占用超过80%的内存。
    - 不要在node1上运行长时间的任务。
- 保证你`/storage`目录下不要存超过15T的内容。

## lxplus
lxplus是CERN的计算平台，核心数非常多，建议在lxplus上交condor任务。但是由于主要的访问节点在欧洲，延迟有些高，可以通过ihep中继。

申请lxplus computing account: https://cms-secretariat.web.cern.ch/cms-registration-and-computing-account

# useful tools

[ROOT](https://root.cern.ch) 

[CMSSW](https://github.com/cms-sw/cmssw)
# coming to CERN
\todo

# TODO before come to zju
\todo