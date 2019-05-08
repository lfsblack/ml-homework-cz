# 实现快速最近邻算法

## K-Means实现矢量量化
- 如果构造的数据确实存在明显的聚类效应, 可以通过修改 gendata.py 中的 mu 参数的系数实现, 当mu即均值无法区分(将系数置0),那么最近邻搜索的误差很大;如果跟实际聚类相似,那么最近邻搜索精度很高,几乎就是真实的结果
- 聚类数目的影响: 假设聚类数目和数据真实的类数目保持一致, 聚类数目越多, 检索速度就越快, 当然如果考虑不一致性, 那么检索精度会下降, 所以需要在速度和精度之间做一个tradeoff