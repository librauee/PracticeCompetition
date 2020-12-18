# 客户流失判断

## 赛题来源

* [DC竞赛](https://js.dclab.run/v2/cmptDetail.html?id=356)

## 任务
* 给定企业客户信息，建立分类模型，判断企业客户是否会流失

## 数据

* 数据主要包括企业客户样本信息。 数据分为训练数据和测试数据，分别保存在train.csv和test_noLabel.csv两个文件中。 字段说明如下： （1）ID：编号 （2）Contract：是否有合同 （3）Dependents：是否有家属 （4）DeviceProtection：是否有设备保护 （5）InternetService：是否有互联网服务 （6）MonthlyCharges：月度费用 （7）MultipleLines：是否有多条线路 （8）Partner：是否有配偶 （9）PaymentMethod：付款方式 （10）PhoneService：是否有电话服务 （11）SeniorCitizen：是否为老年人 （12）TVProgram：是否有电视节目 （15）TotalCharges：总费用 （16）gender：用户性别 （17）tenure：任期年数 （18）Churn：用户是否流失

## 评分标准

* 评分算法为准确率，准确率越高，说明正确预测出企业客户流失情况的效果越好

## 解决方案

* 本赛题未做特征工程（人工特征反而掉分），只用原始数据直接使用lgb预测得到结果