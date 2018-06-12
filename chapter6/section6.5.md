<div align="center">
<img src="../dida.jpg" height="50" width="50" align="left">
<br><p align="right">北京畅行信息技术有限公司</p>
</div>


---

###<font color=#8E8E8E >5. TaxiRide</font>

| 名称              | 类型                 | 说明                                                                                |
|-------------------|----------------------|-------------------------------------------------------------------------------------|
| orderId           | String               | 订单ID                                                                              |
| status            | Integer              | 订单状态，参照[订单状态定义](../chapter5/section5.3.md)                                                         |
| fromPOI           | [MapPoint](section6.7.md)             | 订单起点                                                                            |
| ToPOI             | [MapPoint](section6.7.md)             | 订单终点                                                                            |
| planStartTime     | String               | 出发时间（yyyyMMddHHmmss）                                                          |
| planStartTime     | String               | 出发时间（yyyyMMddHHmmss）                                                          |
| price             | [TaxiPrice](section6.4.md)            | 价格信息                                                                            |
| driverInfo        | [Driver](section6.6.md)              | 司机信息                                                                            |
| driverArrivalTime | String               | 司机到达乘客起点时间（yyyyMMddHHmmss）                                              |
| cancelType        | Integer              | 取消类型（1-乘客取消 2-自动取消 3-车主取消）                                        |
| cancleReson       | String               | 取消原因                                                                            |
| cancelBlame       | Integer              | 本取消单是否有责（0-无 1-有）                                                       |
| cancelTime        | String               | 取消时间（yyyyMMddHHmmss）                                                          |
| systemClosed      | Integer              | 系统关闭状态（0-未关闭 1-已关闭），系统关闭即一段时间内订单状态无流转后系统强制关单 |
| systemCloseTime   | String               | 系统关闭时间（yyyyMMddHHmmss）                                                      |
| onboardDeadline   | String               | 上车时间deadline（yyMMddHHmmss），过后司机可无责取消                                |
| onboardTime       | String               | 上车时间（yyyyMMddHHmmss）                                                          |
| arrivalTime       | String               | 到达目的地时间（yyyyMMddHHmmss）                                                    |
| payTime           | String               | 支付时间（yyyyMMddHHmmss）                                                          |
| driverLocation    | [TaxiPosition](section6.3.md)         | 司机位置                                                                            |
