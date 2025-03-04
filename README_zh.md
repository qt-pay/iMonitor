## 简介

iMonitor（冰镜 - 终端行为分析系统）是一款基于[iMonitorSDK](https://iMonitorSDK.com)的开源终端行为监控分析软件。

提供了对进程、文件、注册表、网络等系统行为的监控。支持扩展和脚本，可以轻易定制和添加更多功能。可以用于病毒分析、软件逆向、入侵检测，EDR等。

## 软件截图
![](./doc/all.gif)

![](./doc/main.png)

![](./doc/address.png)

![](./doc/detail.png)

![](./doc/snapshot.png)

![](./doc/dll.png)

## 更新说明

### 2.1（2022.10.5）

- 添加事件快照支持
  - 快照支持排序
- 添加动态库加载分析（属性 - Dependency）
  - 可以分析Dll丢失、Dll存在挟持风险
- 修复查找任意列导致的崩溃问题

感谢sagasm反馈的使用意见。

### 2.0（2022.09.14）

- 添加展示列的管理，可以定制需要显示的数据

- 添加高亮功能，可以对关键数据做高亮显示

- 支持分组合并统计 ，大大提高了分析的方便（类似于SQL中的GROUP BY效果)

- 添加工作区管理，不同的分析场景可以通过工作区快速切换

- 添加查找功能

- 添加多语言支持

- 添加更多事件支持

  - 添加对命名管道的支持
  - 添加HTTP、HTTPS的支持

- 添加插件支持

  - 支持自定义列
  - 支持自定义规则匹配
  - 支持界面交互（需要依赖Qt）

- 内置部分插件

  - 添加IP地址的归属地列
  - 添加可以自定义规则来显示的路径信息列
  - 添加进程敏感行为说明的列
  - 添加是否是文档的快速规则匹配

- 其他杂项

  - 添加丢弃掉被过滤规则的支持
  - 支持高亮规则跟过滤规则相互切换
  - 规则匹配添加增量过滤的方式，新增规则时不再需要全量匹配
  - 匹配规则添加正则表达式支持
  - 列、规则支持修改默认值
  - 添加安装包
  
  ### 1.0（2022.03.14）