# V - 编程语言

V 将于2019年6月开放。4月15日提前开放访问。 

https://vlang.io

文档: https://vlang.io/docs

推特: https://twitter.com/v_language


&nbsp;

## 快速编译
V 每个CPU核心每秒可编译150万行代码。

这种速度是通过直接生成机器代码来实现的。 

```
wc -l doom3.v     # 458 713
time v doom3.v    # 0.5s
```
[关于编译速度基准和与其他语言的比较](https://vlang.io/compilation_speed)

## 安全
- 没有全局状态
- 没有null
- 没有未定义的值
- 类型可选
- 泛型支持
- 默认不可变
- 部分纯函数

## C/C++编译

V 可以编译整个C/C++项目，并为您提供安全、简单和高达200倍的编译速度。 

```
std::vector<std::string> s;
s.push_back("V is ");
s.push_back("awesome");
std::cout << s.size();
```

```
s := []string 
s << 'V is '
s << 'awesome'
println(s.len)
```
阅读关于翻译 Doom & Doom 3, LevelDB, SQLite (四月推出).	

## 400 KB的零依赖编译器
整个V语言及其标准库小于400KB。你可以在0.3秒内构建V程序。


## 性能
- 和C一样快
- 最低分配额
- 无反射的内置序列化 

## 代码热加载

立即获取更改，无需重新编译！

因为在每次编译之后，您也不必浪费时间到达正在处理的状态，这可以节省大量宝贵的开发时间。

[阅读关于热加载的文档](https://volt-app.com/img/lang.webm)

## 构建可维护程序

您可以在半小时内通过查阅文档来学习整个V语言。

尽管很简单，但它给开发人员很大的权力。其他语言能做的任何事，用V语言都可以做。

## REPL
```
 v
 >> data := http.get('https://vlang.io/utc_now')? 
 >> data 
 '1551205308' 
```

## 本地交叉平台界面库
快速构建交叉平台的本地应用，你再不需要嵌入一个浏览器。

## 到处运行
V能够编译成为(方便阅读)的C代码，这样你就能通过gcc和clang等获取更多平台的支持和优化。
