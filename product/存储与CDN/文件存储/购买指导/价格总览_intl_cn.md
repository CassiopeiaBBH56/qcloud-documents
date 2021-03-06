## 计费模式
CFS 文件存储按照实际使用的存储量计费，没有最低费用，没有流量费用和请求费用。计费周期为小时，存储量按单位小时内实际使用存储空间的最大值计算（峰值）。

## 存储空间
文件系统创建时，会默认占用 3 KB 的存储空间，该存储量将被计入实际使用的存储空间。

## 支持地域
以下是 CFS 文件存储已开放使用的地区：

注：已售罄地区主机或服务若需要使用文件存储，建议在该地域下选择一个 VPC 、在其他有的资源可用区下创建子网，然后在该子网下创建 CFS 文件系统。[查看挂载帮助>>](https://cloud.tencent.com/document/product/582/9551#.E6.9F.90.E5.8F.AF.E7.94.A8.E5.8C.BA.E4.B8.8B-cfs-.E8.B5.84.E6.BA.90.E5.B7.B2.E5.94.AE.E7.BD.84.EF.BC.8C.E5.A6.82.E4.BD.95.E7.BB.A7.E7.BB.AD.E4.BD.BF.E7.94.A8.EF.BC.9F)

地域 | 可用区  | 备注
------- | ------- | -------
北京 | 北京一区 | 已售罄 
    | 北京二区 | 正常使用
    | 北京三区 | 正常使用 
上海 | 上海一区 | 已售罄 
    | 上海二区 | 已售罄 
    | 上海三区 | 正常使用 
广州 | 广州二区 | 已售罄 
    | 广州三区 | 正常使用
    | 广州四区 | 已售罄 
香港 | 香港一区 | 需审核，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category/create?level1_id=16&level2_id=200&level1_name=%E5%85%B6%E4%BB%96%E6%9C%8D%E5%8A%A1&level2_name=%E5%85%B6%E4%BB%96%E4%BA%91%E6%9C%8D%E5%8A%A1)（预计 1 ~ 3 个工作日）
上海金融 | 上海金融一区 | 已售罄 
| 上海金融二区 | 需审核，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category/create?level1_id=16&level2_id=200&level1_name=%E5%85%B6%E4%BB%96%E6%9C%8D%E5%8A%A1&level2_name=%E5%85%B6%E4%BB%96%E4%BA%91%E6%9C%8D%E5%8A%A1)（预计 1 ~ 3 个工作日）
深圳金融 | 深圳金融一区 | 需审核，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category/create?level1_id=16&level2_id=200&level1_name=%E5%85%B6%E4%BB%96%E6%9C%8D%E5%8A%A1&level2_name=%E5%85%B6%E4%BB%96%E4%BA%91%E6%9C%8D%E5%8A%A1)（预计 1 ~ 3 个工作日）
| 深圳金融二区 | 需审核，请提交 [工单申请](https://console.cloud.tencent.com/workorder/category/create?level1_id=16&level2_id=200&level1_name=%E5%85%B6%E4%BB%96%E6%9C%8D%E5%8A%A1&level2_name=%E5%85%B6%E4%BB%96%E4%BA%91%E6%9C%8D%E5%8A%A1)（预计 1 ~ 3 个工作日）

## 免费套餐

截止到 2019 年 1 月 31 日，每个 CFS 的用户（主账户和协作者账户视为一个用户 - 相同 APPID）可以享受 10 GB 的免费存储量（不区分是 NFS 文件系统还是 CIFS/SMB 文件系统），每个计费周期内若用量超出免费额度，超出部分将按阶梯价格收取费用。

## 价格详情
自 2017 年 11 月 10 日凌晨起，中国大陆所有地区执行以下最新价格。
> NFS 文件系统及 CIFS/SMB 文件系统统一价格。

地区 | 中国大陆 | 香港
------- | ------- | -------|
阶梯价格| 0 ~ 10TB  0.35 元/GB/月 (0.00048611 元/GB/时) | 1 TB 以内  0.63 元/GB/月 (0.00087500 元/GB/时)
       | 10 TB以上 0.33 元/GB/月 (0.00045833 元/GB/时) | 1 TB - 10 TB  0.58 元/GB/月 (0.00080556 元/GB/时)
       |  | 10 TB - 50TB  0.52 元/GB/月 (0.00072222 元/GB/时)
       |  | 50 TB 以上  0.46 元/GB/月 (0.00063889 元/GB/时)

## 计费案例
某企业拥有 20 台云服务器（CVM），分别访问 2 个中国大陆地区的文件系统。 文件系统 A 用于做冷数据存储，存储量为 500 GB, 且无增长。文件系统 B 用于企业云盘， 当前该小时中峰值存储量为 105.6 GB。 

该小时 CFS 总费用 = （500+105.6-10）\* 0.00048611= 0.29 元


