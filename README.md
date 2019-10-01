# 家国梦辅助脚本
按键精灵的语法蛋疼，并且复制出来代码的时候中文会乱码！  
~有人有办法复制代码出来中文不乱码的话欢迎issues里面提供给我，多谢！~  
代码在`trainer.txt`文件中

## 演示
https://www.bilibili.com/video/av69603157/

## 脚本需求
- windows
- 安卓模拟器
- 按键精灵手机助手
- 分辨率 540 × 960

## 自定义
> `自定`下面的是可以修改成自己需要的配置

## 格子

> 九宫格, 从左到右从上到下, 格子序号从0开始

| 6 | 7 | 8 |  
| 3 | 4 | 5 |  
| 0 | 1 | 2 |  

## 已实现功能
- [x] 自动收集金币
- [x] 自动按需升级建筑
- [x] 自动按需收集货物
- [x] 收集货物跳过时加速火车运行速度

## 待完善功能
- [ ] 自动升级政策

## 待做功能
- [ ] 人性化配置
- [ ] 使用其他语言做成APP且可配置

## 关于误差
自动收集货物有一定误差率, 简单测试准确度大概在`90%`

## 自定义

### 升级间隔, 默认120秒
Dim autoUpdateInterval = `120`

### 不需要收集的货物
> 每行一条数据, 可设置多条
格式为 `buildings(**格子序号**, 2) = False` 每行一条
https://github.com/liasica/JiaGuoMengTrainer/blob/master/trainer.txt#L36

### 要升级的建筑
> 每行一条数据, 可设置多条

https://github.com/liasica/JiaGuoMengTrainer/blob/master/trainer.txt#L44

格式为
```
buildings(格子序号, 3) = True
buildings(格子序号, 4) = 1
```
