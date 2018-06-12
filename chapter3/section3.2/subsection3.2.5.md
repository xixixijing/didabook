<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >5. 下单</font>
**功能**    订单请求<br>
**URL:**   /3rd_taxi/price<br>
**Request Methos:**  `POST`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| order_id          | String     | Y  |  订单id，通过path传入   |
| partner_cid       | String     | Y  |  第三方标识，接入方标识，双方协定           |
| phone             | String     | Y  |  乘客手机号(base64编码)           |
| start_lon         | String     | Y  |  起点经度           |
| start_lat         | String     | Y  |  起点纬度           |
| start_long_addr   | String     | Y  |  起点长地址         |
| start_short_addr  | String     | Y  |  起点短地址         |
| end_lon           | String     | Y  |  终点经度           |
| end_lat           | String     | Y  |  终点纬度           |
| end_long_addr     | String     | Y  |  终点长地址         |
| end_short_addr    | String     | Y  |  终点短地址         |
| tipping           | Integer    | Y  |  调度费(分)         |
| plan_start_time   | String     | N  |  预约出发时间(yyyyMMddHHmmss，不传为实时单)  |
| coorinate_system  | String     | Y  | 使用的坐标系，参见[坐标系定义](../../chapter5/section5.4.md) |
 
**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误消息|
