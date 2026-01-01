+++
date = '2026-01-01T20:09:08+08:00'
draft = true
title = '2025前端面试高频手写题'
categories = ['面试']
+++

### 
# 1、Promise.all 实现  4次
| <font style="color:rgb(38, 38, 38);">次数</font>    | 日期 | 公司 |
| --- | --- | --- |
| <font style="color:rgb(38, 38, 38);">1</font> | 11/28 | 高德一面 |
| 2 | 12/2 | 美团核心本地商业一面 |
| 3 | <font style="color:rgb(38, 38, 38);">12/18</font> | 爱奇艺三面 |
| 4 | <font style="color:rgb(38, 38, 38);">12/24</font> | 小红书二面 |




## 2、带并发限制的异步调度器  4次
| <font style="color:rgb(38, 38, 38);">次数</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">日期</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">公司</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">问题</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">写的情况   </font> |
| --- | --- | --- | --- | --- |
| <font style="color:rgb(38, 38, 38);">1</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">11/28</font> | <font style="color:rgb(38, 38, 38);">高德打车一面</font> | <font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">   </font> |
| <font style="color:rgb(38, 38, 38);">2</font> | <font style="color:rgb(38, 38, 38);">12/8</font> | <font style="color:rgb(38, 38, 38);">快手KIM 一面</font> | <font style="color:rgb(38, 38, 38);"></font> | <font style="color:rgb(38, 38, 38);"></font> |
| <font style="color:rgb(38, 38, 38);">   </font><font style="color:rgb(38, 38, 38);">3</font> | <font style="color:rgb(38, 38, 38);">   </font><font style="color:rgb(38, 38, 38);">12/12</font> | <font style="color:rgb(38, 38, 38);">   </font><font style="color:rgb(38, 38, 38);">淘天直播二面</font> | <font style="color:rgb(38, 38, 38);">   </font><font style="color:rgb(17, 124, 238);">2、淘天二面 调度器+异步请求模拟+结果收集</font> | <font style="color:rgb(38, 38, 38);">   </font><font style="color:rgb(38, 38, 38);">最后返回结果时，异步问题没解决，本来需要返回Promise实例，借助resolve来返回，我写的是同步的直接return res</font> |
| <font style="color:rgb(38, 38, 38);">4   </font> | <font style="color:rgb(38, 38, 38);">12/16</font> | Xtransfer一面（上海） |  |  |




# 3、防抖节流
| 次数 | 日期 | 公司 | 问题 | 优化项 | 写的情况 |
| --- | --- | --- | --- | --- | --- |
| 1 | 12/3 | 优酷一面 | 防抖和节流实现 | | |
| 2 | 12/16 | 字节番茄一面 | [自定义hooks useDebounceFn](https://www.yuque.com/codertcl/pgzxph/kr5q08gyngac8npy#ANydB) | 1、useEffect清理timer<br/>2、缓存返回的函数<br/>3、支持立即执行<br/>4、支持取消 | 1、忘了清理timer |


# 4、数组元素转树形层级数组  3
| <font style="color:rgb(38, 38, 38);">次数</font> | <font style="color:rgb(38, 38, 38);">日期</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">公司</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">备注</font> |
| --- | --- | --- | --- |
| 1 | 11/25 | 高途一面 | |
| 2 | 12/3 | 滴滴网约车 | |
| 3 | <font style="color:rgb(38, 38, 38);">12/22</font> | 小红书 | 二次追问，一次遍历能否实现 |


# 5、深拷贝
| <font style="color:rgb(38, 38, 38);">次数</font>    | <font style="color:rgb(38, 38, 38);">日期</font>    | <font style="color:rgb(38, 38, 38);">公司</font>    |
| --- | --- | --- |
| 1  | 字节番茄 一面 | 12/16   |


  


# 6、事件总线实现
| <font style="color:rgb(38, 38, 38);">次数</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">日期</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">公司</font><font style="color:rgb(38, 38, 38);">   </font> | <font style="color:rgb(38, 38, 38);">优化项   </font> |
| --- | --- | --- | --- |
| <font style="color:rgb(38, 38, 38);">1   </font> | <font style="color:rgb(38, 38, 38);">12/2   </font> | <font style="color:rgb(38, 38, 38);">美团一面   </font> | <font style="color:rgb(38, 38, 38);">off时无需转换为将函数字符串，直接===判断是否为同一个函数即可</font> |


<font style="color:rgb(38, 38, 38);">  
</font>

# 7、二叉树
## 1、二叉树最小深度 （猿辅导一面 12/4）
## 2、二叉树的深度 （淘天直播 一面  12/5）
## 3、二叉树层序遍历   （XTransfer 一面12/16）

