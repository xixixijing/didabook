<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >6. 订单查询</font>

**功能**    订单查询<br>
**URL:**   /3rd_taxi/ride/{order_id}<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---              | :-----:|:----:|  ---   |
| order            | String   | Y  |  订单id，通过path传入     |
| phone            | String   | Y  |  乘客手机号(base64编码)   |
| coorinate_system | String   | Y  | 使用的坐标系，参见[坐标系定义](../../chapter5/section5.4.md) |
 
**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer  | 返回码|
| message     | String   |错误消息|
| taxiRide    | [TaxiRide](../../chapter6/section6.5.md) |订单详情|