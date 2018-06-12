<div align="center">
<img src="../../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---
###<font color=#8E8E8E >2. 附近出租车</font>

**功能**    获取附近出租车及轨迹。目前一条轨迹仅由两个点组成，<br>建议15s轮询该接口，刷新运动轨迹更可通过配置更新回调进行通知<br>
**URL:**   /3rd_taxi/nearby_drivers<br>
**Request Methos:**  `GET`<br>
**Request Parameters:** 

| 参数名      | 类型   |  必须 |  说明  |
| ---         | :-----:|:----:|  ---   |
| phone       | String     | Y  |  乘客手机号(base64编码)   |
| lon         | String     | Y  |  乘客位置经度             |
| lat         | String     | Y  |  乘客位置纬度             |
| coorinate_system | String | Y  | 使用的坐标系，参见[坐标系定义](../../chapter5/section5.4.md) |
 
**Request Body:** 

| 参数名      | 类型   |   说明  |
| ---         | :-----:|  ---   |
| code        | Integer | 返回码|
| message     | String  |错误消息|
| driverEta   | String  | 最近司机预计到达时间(yyyyMMddHHmmss)
| driver Tracks |List&lt;[TaxiTrack](../../chapter6/section6.2.md)&gt; | 司机轨迹 |
