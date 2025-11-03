# Gene Enrichment

根据基因列表文件进行GO和KEGG富集

## 一、输入参数说明

### 1. 数据：`富集基因`

需要富集的基因，文件内每一行为一个基因，要求为基因symbol，可以根据输入框右边的辅助按钮选择文件

多类基因放在不同文件内

### 2. 参数：`基因组`

数据对应的基因组版本，选择即可。

## 二、输出文件说明

1、`txt`为富集结果，`pdf`为对应的画图

2、画图结果为前12个符合的term，p-value闽值为0.05，qvalue阔值为0.2，最少基因数量为10(Count = 10)，因此可能存在空的画图结果

3、富集结果字段说明

    - pvalue：富集的p值
    
    - p.adjust：校正之后的p值
    
    - qvalue：q值
    
    - genes：输入的做富集分析的基因中富集到这个term上面的基因
    
    - Count：输入的做富集分析的基因中富集到这个term上面的基因的数目（genes的数量，dotplot内点的大小）
    
    - GeneRatio：这里是一个分数，分子是富集到这个term上的基因的数目（genes的数量），分母是所有输入的做富集分析的gene的数目（dotplot的横轴）

## 三、任务作者

winter <winter_lonely@foxmail.com>
