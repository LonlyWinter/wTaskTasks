# Download From GEO

根据GEO ID从GEO下载数据

## 一、输入参数说明

### 1. 数据：`GEO_ID文件`

文件内为需要下载的GSM_ID或GSE_ID，每行一个GSM_ID/GSE_ID
下载fastq文件时，每一行的GSM_ID后可以增加一列（利用制表符分隔开）作为样本文件名称


#### 示例1：下载`GSE243517`和`GSM7789822`的所有`GSM`样本

``` txt
GSE243517
GSM7789822
```

#### 示例2：下载`GSM`并重命名

``` txt
GSM7789822	WT 0h 1
GSM7789823	WT 0h 2
```


## 二、输出文件说明

各个下载的文件

## 三、任务作者

winter <winter_lonely@foxmail.com>
