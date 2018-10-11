# 微证券线上问题处理手册 版本v1.1

### 询问用户具体问题，尽可能的拿到问题截图，根据具体的截图类型，参考具体的解决方案：

| 截图类型 | 问题说明                                                     | 解决方案 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------ |
| ![企业微信截图_15390528202004](https://raw.githubusercontent.com/latel/tuchuang/master/%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_15390528202004.png) | 出现这种截图，一般是前端问题，需要反馈给前端开发             | <a href="#blank">参考页面白屏问题解决方案</a> |
| ![企业微信截图_15390528388631](https://raw.githubusercontent.com/latel/tuchuang/master/%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_15390528388631.png) | 出现这种错误一般是DNS解析错误，即网络有问题 | <a href="#network">参考网络问题解决方案</a>   |
| ![image-20181009152901789](https://raw.githubusercontent.com/latel/tuchuang/master/5KOM%7E5QA3JTAE%24T4_YE\)D\(2.png) | 出现这种错误一般是DNS解析错误，即网络有问题 | <a href="#network">参考网络问题解决方案</a>   |
| ![](https://raw.githubusercontent.com/latel/tuchuang/master/20181010105213.png) | 一般是数据加载问题，即拉取不到自选列表数据 | <a href="#null_list">参考自选列表为空解决方案</a> |
| ![](https://raw.githubusercontent.com/latel/tuchuang/master/%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_15392403698631.png) | 一般是网络有问题 | <a href="#other">参考其他问题解决方案</a>     |
| 其他截图或未提供截图 | 具体情况具体分析 | <a href="#other">参考其他问题解决方案</a>     |

<a name="network"></a>
## 网络问题解决方案 

1. 引导用户访问理财通<a href="https://qian.tenpay.com/mb/v4/index.shtml">`https://qian.tenpay.com/mb/v4/index.shtml`</a>是否正常，如果同样打不开则意味着用户的手机网络有问题，直接引导用户切换网络，否则继续步骤2
2. 引导用户进行系统探测，即访问<a href="https://wzq.tenpay.com/mp/v1/abnormal/analysis.shtml">`https://wzq.tenpay.com/mp/v1/abnormal/analysis.shtml`</a>或者在公众号输入“问题反馈”并选择“**首页或资产打不开**”
3. 收集相关信息至如下[问题收集表格][]，并反馈相关情况至前端和后端。

<a name="blank"></a>
## 页面白屏问题（中间显示微证券商标）解决方案

1. 引导用户上传**前端日志**
2. 如果是**ios机器**则直接跳到步骤5
3. 如果是**安卓机器**，用户配合意愿好的话引导用户上传**X5详细内核日志**，并将用户拿到的uuid记录下来
4. 如果是**安卓机器**，但用户配合意愿不好的话引导用户上传**X5内核日志**，并将用户拿到的uuid记录下来
3. 收集相关信息至如下[问题收集表格][]，并反馈相关情况至前端

<a name="null_list"></a>
## 自选列表为空解决方案

1. 引导用户上传**前端日志**
2. 收集相关信息至如下[问题收集表格][]，并反馈相关情况至前端

<a name="other"></a>
## 其他问题解决方案

1. 引导用户使用系统自带的浏览器（不要使用微信打开）访问<a href="https://wzq.tenpay.com/mp/v1/abnormal/log.shtml?auto=1">`https://wzq.tenpay.com/mp/v1/abnormal/log.shtml?auto=1`</a>上传**前端日志**
2. 收集相关信息至如下[问题收集表格][]，并反馈给前端

## 附录：各种类型日志的获取方法

| 日志类型       | 详细步骤                                                     |
| -------------- | ------------------------------------------------------------ |
| 前端日志       | 引导用户访问<a href="https://wzq.tenpay.com/mp/v1/abnormal/log.shtml?auto=1">`https://wzq.tenpay.com/mp/v1/abnormal/log.shtml?auto=1`</a>，或者在公众号输入框输入“问题反馈”并选择"**其他问题**" |
| X5内核日志     | 访问<a href="http://x5tools.wsd.com/">`http://x5tools.wsd.com/`</a>，日志拉取->livelog->发送二维码给用户->用户反馈uuid |
| X5内核详细日志 | ![企业微信截图_15390517016824](https://raw.githubusercontent.com/latel/tuchuang/master/%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_15390517016824.png) |



[问题收集表格]: https://docs.qq.com/sheet/DdXR0amRpQUVNdWJS?opendocxfrom=admin&tab=BB08J2#tab=BB08J2
