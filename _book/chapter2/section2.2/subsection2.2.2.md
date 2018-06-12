<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---
###<font color=#8E8E8E >3. 参数签名</font>

1. sign_key由嘀嗒下发
2. 签名算法:
	+ 所有参数按字典序升序排序并按照“参数=参数值”的模式用“&”字符拼接成字符串<br>
	sort_par_str.<font color=#00BB00 >"par1=value&par2=value2"</font>
	+  对排序后的参数sort_par_str拼接时间戳和sign_key加盐后求小写MD5<br> 
	sign=lower_case(md5(sort_par_str+<font color=#00BB00 >​"&timestamp="</font>​+unixtimestamp+<font color=#00BB00 >​"&si gn_key="</font>​+sign_key)) 

