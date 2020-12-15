# 识别失信企业

## 赛题来源

* [DC竞赛](https://www.dcjingsai.com/v2/cmptDetail.html?id=360)

## 任务
* 建立分类模型，识别有失信记录的企业

## 数据

* 数据给出了一些企业的基本信息，分为训练数据和测试数据，分别保存在train和test_noLabel两个文件夹中。 字段说明如下：

ID：企业ID

Code：类型编码

Investment：获得投资

Capital：注册资本

Stock：股票 

Income：收入 

assets_1：类型1资产

assets_2：类型2资产

expenditure_1：类型1支出

expenditure_2 ：类型2支出

expenditure_3 ：类型3支出

tax：缴税

debt：负债 

loan：借款

Label：标签

## 评分标准

* 标准的macro F1

## 解决方案

* 本赛题的评分标准值得注意，是macro F1, 求的是类别的F1均值
* 因为这是一个样本不均衡的问题，这里采用了随机过采样，直接将正样本数量随机选择扩充至与负样本数量相当
* 做了部分空值处理，以及一些简单的特征工程
* 采用多种子平均作为最后方案