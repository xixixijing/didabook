<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---
###<font color=#8E8E8E >2. 签名&令牌传递</font>

签名和令牌信息通过Header传递，请在每个请求的头部添加:

| Header Name | Value | 说明 |
| ----        |----   |----  |
|Authorization|Beare+<font color=#00BB00 >" "</font>+{token} | {token}通过/access_token获取
|Sign         |sign+<font color=#00BB00 >" "</font>+unixtimestamp | sign参照[参数签名](subsection2.2.2.md)，unixtimstamp与签名时使用同一个时间戳|

