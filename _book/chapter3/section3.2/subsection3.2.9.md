<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >9. 支付</font>

**功能**    订单支付通知<br>
**URL:**   /3rd_taxi/ride/{order_id}/pay<br>
**Request Methos:**  `POST`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---              | :-----:|:----:|  ---   |
| order            | String   | Y  |  订单id，通过path传入     |
| phone            | String   | Y  |  乘客手机号(base64编码)   |
| coorinate_system | String   | Y  | 使用的坐标系，参见坐标系定义 |
| price            | Integer  | Y  | 订单总金额（即司机收到的金额）|
| couponId         | Long     | N  |优惠券ID|
| couponPrice      | Integer  | N  |优惠券抵扣金额（分）|



**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer  | 返回码|
| message     | String   |错误消息|

