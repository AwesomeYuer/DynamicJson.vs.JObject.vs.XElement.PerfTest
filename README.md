# DynamicJson.vs.JObject.vs.XElement.PerfTest

对比如下三种写法

1. JObject.Parse 好像最差
2. DynamicJson 其实就是 XElement.Load
3. JsonConvert.DeserializeXNode 转 XElement

全都基本是每增加 200K 报文, 增加 100毫秒解析成本

添加性能计数器
![image](https://github.com/Microshaoft/DynamicJson.vs.JObject.vs.XElement.PerfTest/blob/master/ConsoleApp1/Images/PerformanceCounter1.jpg)

监控性能计数器
![image](https://github.com/Microshaoft/DynamicJson.vs.JObject.vs.XElement.PerfTest/blob/master/ConsoleApp1/Images/PerformanceCounter2.jpg)



