# 借贷风险预测

## 任务
* 给定银行用户信息，建立分类模型，预测银行用户的信用好坏

## 数据

* 数据主要包括银行用户信息的脱敏信息。 数据分为训练数据和测试数据，分别保存在train.csv和test_noLabel.csv两个文件中。 字段说明如下： （1）uid：编号 （2）x0-x19：银行用户的具体信息，已脱敏处理 （3）y：银行用户的信用好坏，1表示信用好，0表示信用差。

## 评分标准

* 评分算法为准确率，准确率越高，说明正确预测出银行用户的信用的效果越好

## 解决方案

* 本赛题给出了20个匿名数字特征，本方案未做任何特征工程，直接将三个模型均值融合