# 1. module和project之间的关系
### 1. 在一个project中，添加一个module，比如file->new->import module,实际上是在project中的settings.gradle中加了include：
```gradle
include ':app', ':libccm_test'
```
### 并且在module目录下生成了一个.iml文件，这个暂时没研究过
### 2.module不方便从github直接导入，最好先从github clone到本地，然后在选择import module

# 2. 如何导入ssh-key相关的git仓库
### 1. 前提条件：配置好本地git，环境变量，账号，以及在git服务器添加ssh-key
### 2. 注意，一下的配置是关键：

> * file->settings->version control->git->SSH executable

### 这里的ssh executable一定要配置成native的，因为你的ssh-key使用本地的ssh生成的。
### 3. 也许可以用AS的ssh来成ssh-key，暂时未研究

