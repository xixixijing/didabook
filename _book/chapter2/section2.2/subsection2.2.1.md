<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---
###<font color=#8E8E8E >1. 获取token</font>
**URL:**  /auth/access_token<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| grant_type  | String | Y    |固定传client_credentials|
| client_id   | String | Y    |分发的client id|
| client_secret|String | Y    |分发的client secret|

**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误信息|
| AuthInfo    | [AuthInfo](../../chapter6/section6.1.md) | 授权信息|

