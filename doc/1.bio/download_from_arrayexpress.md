# Download From ArrayExpress

ArrayExpress数据下载

## 一、输入参数说明

### 1. 数据：`ArrayID文件`

文件内为需要下载的`ArrayID`，如`E-MTAB-14170`，每行一个`ArrayID`，即可以下载该ArrayID下的所有样本

如需下载特定样本，每一行的`ArrayID`后可以增加一列（利用制表符分隔开）作为样本名称(`Source Name`)

#### 示例1：下载`E-MTAB-14170`和`E-MTAB-14171`的所有样本

``` txt
E-MTAB-14170
E-MTAB-14171
```

#### 示例2：下载`E-MTAB-14170`的部分样本和`E-MTAB-14171`的所有样本

``` txt
E-MTAB-14170	P4 DP47 4h
E-MTAB-14170	P4 EpCAM TCB 48h
E-MTAB-14171
```



## 二、输出文件说明

各个下载的文件

## 三、任务作者

winter <winter_lonely@foxmail.com>
