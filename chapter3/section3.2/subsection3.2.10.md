<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >10. 取消订单</font>

**功能**    取消订单<br>
**URL:**   /3rd_taxi/order/{order_id}/confirmPrice<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| order_id    | String   | Y  |  订单id，通过path传入     |
| phone            | String   | Y  |  乘客手机号(base64编码)   |
| reson            | String   | Y  |  取消原因                 |

**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误消息|
