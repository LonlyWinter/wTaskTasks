# wTaskTasks

wTask预定义任务

## 任务类型

### 1. bio

生信数据分析相关任务

1. `atac_occo`: 利用ATAC数据，分析随着时间变化的CO和OC区域。[说明文档](./doc/1.bio/atac_occo.md)

2. `callpeak_after_mergebam`: 将Bam文件Merge起来后，重新call peak。[说明文档](./doc/1.bio/callpeak_after_mergebam.md)

3. `cluster_kmeans`: 将表格数据按照列聚类K-Means聚类。[说明文档](./doc/1.bio/cluster_kmeans.md)

4. `correlation_python`: 利用python计算样本的相关性，会根据样本标签和样本分别做相关性，即每个样本之间的相关性和每类样本之间的相关性。[说明文档](./doc/1.bio/correlation_python.md)

5. `correlation_seurat`: 利用Seurat计算样本的相关性，会根据样本标签和样本分别做相关性，即每个样本之间的相关性和每类样本之间的相关性。[说明文档](./doc/1.bio/correlation_seurat.md)

6. `deg_deseq2`: 利用DeSeq2计算差异表达基因，DeSeq2利用counts文件计算差异表达基因。[说明文档](./doc/1.bio/deg_deseq2.md)

7. `download_from_arrayexpress`: ArrayExpress数据下载。[说明文档](./doc/1.bio/download_from_arrayexpress.md)

8. `download_from_geo`: 根据GEO ID从GEO下载数据。[说明文档](./doc/1.bio/download_from_geo.md)

9. `download_from_link`: 根据文件链接列表下载。[说明文档](./doc/1.bio/download_from_link.md)

10. `enrichment_plot`: 根据富集分析结果，挑选需要的term画图。[说明文档](./doc/1.bio/enrichment_plot.md)

11. `expression_heatmap`: 基因表达热图。[说明文档](./doc/1.bio/expression_heatmap.md)

12. `gene_enrichment`: 根据基因列表文件进行GO和KEGG富集。[说明文档](./doc/1.bio/gene_enrichment.md)

13. `gene_regions`: 获取基因对应的region。[说明文档](./doc/1.bio/gene_regions.md)

14. `gene_venn`: 计算不同基因之间的交集，每个文件内的基因为一类，两两做交集。[说明文档](./doc/1.bio/gene_venn.md)

15. `region_changes`: 计算不同类别之间变化的相关性：散点的密度图。[说明文档](./doc/1.bio/region_changes.md)

16. `region_enrichment`: 使用regionR计算不同Region之间的富集程度。[说明文档](./doc/1.bio/region_enrichment.md)

17. `region_motif`: 利用homer查找motif。[说明文档](./doc/1.bio/region_motif.md)

18. `region_motif_from_peak`: 使用peak和summit，利用homer查找motif。[说明文档](./doc/1.bio/region_motif_from_peak.md)

19. `region_signal_profile`: 计算region上面不同bigwig的信号值分布。[说明文档](./doc/1.bio/region_signal_profile.md)

20. `region_signal_profile_center`: 计算region中间位置两边不同bigwig的信号值分布。[说明文档](./doc/1.bio/region_signal_profile_center.md)

21. `region_specific`: 计算不同Region之间的区别。[说明文档](./doc/1.bio/region_specific.md)

22. `region_specific_withrep`: 计算两类Region之间的区别，每类Region有多个重复。[说明文档](./doc/1.bio/region_specific_withrep.md)

23. `tad_change`: 利用HiCExplorer结果，根据domain.bed计算TAD的变化：Unchanged、Separation、Fusion、EquilongShift、UnilateralShift、Resharp。[说明文档](./doc/1.bio/tad_change.md)


### 2. yb

医保风控相关任务

1. `wstatistics_export`: 导出数据库数据。[说明文档](./doc/2.yb/wstatistics_export.md)

2. `wstatistics_rule`: 通用规则预筛选。[说明文档](./doc/2.yb/wstatistics_rule.md)

3. `wstatistics_sql`: 直接运行sql筛选。[说明文档](./doc/2.yb/wstatistics_sql.md)


### 3. dev

服务器运维相关任务

1. `base_monitor`: 服务器资源监控：CPU/内存/硬盘/IP。[说明文档](./doc/3.dev/base_monitor.md)

2. `disk_monitor`: 使用du命令监控用户硬盘占用。[说明文档](./doc/3.dev/disk_monitor.md)


### 4. spider

爬虫相关任务

1. `cis_calendar`: CIS学术会议提醒。[说明文档](./doc/4.spider/cis_calendar.md)

2. `westlake_news`: 昨日新闻提醒。[说明文档](./doc/4.spider/westlake_news.md)


### 5. tool

其它工具任务

1. `img_to_gif`: 将批量PNG/JPG/JPEG图片转为GIF。[说明文档](./doc/5.tool/img_to_gif.md)

2. `power_rename_links`: 批量文件重命名。[说明文档](./doc/5.tool/power_rename_links.md)

3. `wait_cmd`: 等待其它程序完成后再运行命令。[说明文档](./doc/5.tool/wait_cmd.md)

4. `zip_dir`: 将文件夹内的所有数据压缩为zip，方便下载数据。[说明文档](./doc/5.tool/zip_dir.md)


## 使用

利用[wTask](https://github.com/LonlyWinter/wTask)平台运行任务

## 作者

winter <winter_lonely@foxmail.com>