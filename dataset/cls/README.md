## 要点检测声明数据集
该数据集是基于我们收集的app隐私协议声明信息进行切句标注，目的是判断app声明是否包含法律法规规定的必须要包含的若干部分（下称为法律法规要点），包含如下：
* 个人信息超期处理方式(ExceedLimit)
* 个人信息存储地信息(StorageRegion)
* 个人信息存储时间（StorageTime）
* 隐私政策时效性信息(Aging)
* 个人信息查询描述（Query，用户权利保障）
* 个人信息更正描述 (Correct，用户权利保障)
* 个人信息删除描述(Delete，用户权利保障)
* 注销账户时，个人信息处置方式(Logout，用户权利保障)
* SDK使用信息说明（SDK）
* 撤销授权方式说明（Repeal，用户权利保障）

## 样例
- 文本：“在以下情形中，您可以向我们提出删除个人信息的请求”
- label: [0,0,0,0,0,0,1,0,0,0], 其中1的位置对应于“个人信息删除描述(Delete，用户权利保障)”
