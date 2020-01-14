# fiddler

## 工具简介

- 功能
  - 从各种浏览器中监控HTTP/HTTPS的流量
  - 查看，调试客户端流量
  - 伪造客户端请求和服务器响应
  - 测试网站或者APP的性能
  - 解码HTTPS网络会话
  - 可以安装其他fiddler插件

- 工作原理
  - 在客户端和服务器之间做一层代理，请求先经过fiddler才到服务器，响应也是先经过fiddler才到客户端
  - 代理模式
    - 流模式：有什么数据都是立即返回给客户端（更接近浏览器本身的行为）
    - 缓存模式：等整个HTTPS请求结束之后才把数据返回给客户端

- 常见使用场景
  - 开发环境host配置
  - 前后端接口调试
  - 线上bugfix
  - 性能分析和优化

## 界面操作介绍

- 工具条常用功能
  - 小消息icon：备注
  - replay按钮：回放
  - go按钮：配合断点调试
  - stream按钮：模式切换
  - decode按钮：解压请求
  - Keep按钮：保持多少会话
  - Any Process按钮：过滤请求
  - save按钮：保存会话（可以重新导入）
  - 相机icon：截图
  - 时钟icon：计时器
  - clear cache按钮：清除缓存
  - TextWizard按钮：编码/解码
  - Tearoff按钮：分离面板

- 状态栏操作
  - 命令行工具栏
  - Capturing：是否捕捉流量
  - Web Browsers：过滤会话来源
  - 计数器：计算当前会话的数量

- 监控面板的使用
  - Statistics：数据统计，可用于分析性能指标
  - Inspectors：对请求解包
  - AutoResponder:对文件进行代理，可以用于bugfix
  - Composer：前后端接口连调
  - Filters：过滤器
  - Log：日志
  - Timeline：网站性能分析

## 常用功能

- host配置：在Tools按钮里面的`HOSTS`
- 文件替换：AutoResponder
- 前后端接口连调：Composer
- 网络限速：使用FiddlerScript,修改事件，比如OnBeforeRequest

## 插件介绍

- 代码格式化插件（官方插件）
- http代理插件（第三方插件）
