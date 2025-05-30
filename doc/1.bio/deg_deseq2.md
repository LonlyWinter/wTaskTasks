# DEG DESeq2

利用DeSeq2计算差异表达基因，DeSeq2利用counts文件计算差异表达基因


## 一、输入参数说明

## 1. 数据：`表达矩阵`

所有样本的counts，每一列为一个样本。多个counts文件利用英文逗号间隔，将利用每个文件的第一列合并

## 2. 参数：`基因组`

文件对应的基因组版本，选择即可。

## 3. 参数：`样本meta`，[模板文件](./docs/deg_deseq2/DEG.meta.xlsx)

sample列为样本名字，需要与counts文件内的名字对应

tag列为样本标签，标签相同的则认为是重复

type列为a或b

比如type为a的tag有tag1和tag2，type为b的tag有tag3和tag4，
则最终差异基因计算结果为4种tag1_vs_tag3、tag1_vs_tag4、tag2_vs_tag3、tag2_vs_tag4

## 4. 参数: `log2fc阈值`

foldchange为差异倍数，log2fc为1时差异倍数为2，log2fc为2时差异倍数为4

## 二、输出文件说明

### 1. `counts`和`deseq2`文件夹

每一类差异基因分析时用的counts，及对应的结果

### 2. `plot`和`genes`文件夹

差异分析结果的火山图及对应的上下调的基因，`genes`文件夹内有`summary.txt`文件为基因数量的统计

### 3. `enrich`文件夹

差异基因的富集结果


## 三、任务作者

winter <winter_lonely@foxmail.com>
