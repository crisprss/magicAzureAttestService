# magicAzureAttestService
针对于AzureAttestService服务的本地提权Eop，微软表示已经进行修复

# Usage
![](https://md.buptmerak.cn/uploads/upload_f0ba78d2bca28ee5c05dd7fc1e1dfbcf.png)
```
magicAzureAttestService.exe -i -c \[cmd\]
```
![](https://md.buptmerak.cn/uploads/upload_3725ac4ed634f71fe42801729de9c701.png)

# 思路
主要是针对 SQL Server 2019的特定服务magicAzureAttestService
![](https://md.buptmerak.cn/uploads/upload_f6d0e2075266ac8cdf8748f51e0142f8.png)

通过UNC欺骗实现以模拟管道的方式提权到SYSTEM用户，可以说是0Day，但是比较局限，微软已经修复:
![](https://md.buptmerak.cn/uploads/upload_b340d473b4e054f0b1bdd587c34fe9e5.png)

