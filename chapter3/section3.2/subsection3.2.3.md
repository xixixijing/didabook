<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >3. 询价</font>

**功能**    价格预估<br>
**URL:**   /3rd_taxi/price<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| phone       | String     | Y  |  乘客手机号(base64编码)   |
| start_lon         | String     | Y  |  起点经度           |
| start_lat         | String     | Y  |  起点纬度           |
| end_lon         | String     | Y  |  终点经度           |
| end_lat         | String     | Y  |  终点纬度           |
| coorinate_system | String | Y  | 使用的坐标系，参见[坐标系定义](../../chapter5/section5.4.md) |
 
**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误消息|
| price       | [TaxiPrice](../../chapter6/section6.4.md)   |估价信息|