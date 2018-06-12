<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >1. 获取配置</font>
**功能**    获取配置类信息，例如开通城市，取消原因等。配置变更<br>可通过配置更新回调进行通知<br>
**URL:**   /3rd_taxi/config<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| -           | -      | -    |  -     |
 
**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误消息|
| config      | [TaxiConfig](../../chapter6/section6.8.md) | 配置信息，包括城市配置（开通城市列表及调度费<br>规则），取消原因，投诉原因|


