# 查询EIP<a name="eip_api_0002"></a>

## 功能介绍

查询指定的EIP。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=ShowPublicip)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

GET /v1/\{project\_id\}/publicips/\{publicip\_id\}

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|project_id|是|String|项目ID，获取项目ID请参见获取项目ID|
|publicip_id|是|String|EIP唯一标识最大长度：**36**|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


## 响应参数

**状态码： 200**

**表 3**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|publicip|PublicipShowResp object|EIP对象|


**表 4**  PublicipShowResp

|参数|参数类型|描述|
|--|--|--|
|bandwidth_id|String|EIP对应带宽ID最大长度：**36**|
|bandwidth_name|String|带宽名称最小长度：**1**最大长度：**64**|
|bandwidth_share_type|String|表示共享带宽或者独享带宽 取值范围：PER，WHOLE。 WHOLE表示共享带宽 PER表示独享带宽 约束：其中IPv6暂不支持WHOLE类型带宽。枚举值：**WHOLE****PER**|
|bandwidth_size|Integer|带宽大小，单位为Mbit/s。最小值：**0**|
|create_time|String|EIP申请时间（UTC）|
|enterprise_project_id|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建弹性公网IP时，给弹性公网IP绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。最大长度：**36**|
|id|String|EIP唯一标识最大长度：**36**|
|port_id|String|功能说明：端口id。约束：只有绑定了的EIP查询才会返回该参数最大长度：**36**|
|private_ip_address|String|功能说明：绑定弹性公网IP的私有IP地址约束：只有绑定了的弹性公网IP查询才会返回该参数|
|profile|ProfileResp object|功能说明：额外参数，包括订单id、产品id等信息约束：如果profile不为空，说明是包周期的EIP|
|public_ip_address|String|IPv4时是申请到的EIP地址，IPv6时是IPv6地址对应的IPv4地址最大长度：**15**|
|status|String|功能说明：弹性公网IP的状态- 取值范围：冻结FREEZED，绑定失败BIND_ERROR，绑定中BINDING，释放中PENDING_DELETE， 创建中PENDING_CREATE，创建中NOTIFYING，释放中NOTIFY_DELETE，更新中PENDING_UPDATE， 未绑定DOWN ，绑定ACTIVE，绑定ELB，绑定VPN，失败ERROR。枚举值：**FREEZED****BIND_ERROR****BINDING****PENDING_DELETE****PENDING_CREATE****NOTIFYING****NOTIFY_DELETE****PENDING_UPDATE****DOWN****ACTIVE****ELB****ERROR****VPN**|
|tenant_id|String|项目ID最大长度：**36**|
|type|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最大长度：**36**|
|public_ipv6_address|String|IPv4时无此字段，IPv6时为申请到的EIP地址最大长度：**39**|
|ip_version|Integer|IP版本信息，取值范围是4和6 4：表示IPv4 6：表示IPv6枚举值：**4****6**|
|public_border_group|String|功能说明：表示中心站点资源或者边缘站点资源,对接了边缘站点的区域才会返回该字段取值范围： center、边缘站点名称 约束：publicip只能绑定该字段相同的资源最小长度：**1**最大长度：**64**|
|allow_share_bandwidth_types|Array of strings|功能说明：表示此publicip可以加入的共享带宽类型列表，如果列表为空，则表示该publicip不能加入任何共享带宽约束：publicip只能加入到有该带宽类型的共享带宽中最大长度：**64**|
|alias|String|功能说明：弹性公网IP名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最大长度：**64**|


**表 5**  ProfileResp

|参数|参数类型|描述|
|--|--|--|
|order_id|String|订单的id最大长度：**36**|
|product_id|String|产品的id最大长度：**36**|
|region_id|String|region的id最大长度：**36**|
|user_id|String|用户的id最大长度：**36**|


**状态码： 400**

**表 6**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 401**

**表 7**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 403**

**表 8**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 404**

**表 9**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 405**

**表 10**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 406**

**表 11**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 407**

**表 12**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 408**

**表 13**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 409**

**表 14**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 500**

**表 15**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 501**

**表 16**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 502**

**表 17**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 503**

**表 18**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 504**

**表 19**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


## 请求示例

无

## 响应示例

**状态码： 200**

GET和PUT操作正常返回

```
{
  "publicip" : {
    "tenant_id" : "8b7e35ad379141fc9df3e178bd64f55c",
    "bandwidth_name" : "bandwidth-test",
    "public_ip_address" : "161.xx.xx.12",
    "create_time" : "2015-07-16 04:32:50",
    "profile" : {
      "user_id" : "35f2b308f5d64441a6fa7999fbcd4321",
      "product_id" : "00301-48027-0--0",
      "region_id" : "xxx",
      "order_id" : "xxxxxxxxx"
    },
    "type" : "5_bgp",
    "bandwidth_id" : "49c8825b-bed9-46ff-9416-704b96d876a2",
    "bandwidth_size" : 10,
    "enterprise_project_id" : "b261ac1f-2489-4bc7-b31b-c33c3346a439",
    "ip_version" : 4,
    "private_ip_address" : "192.168.10.5",
    "bandwidth_share_type" : "PER",
    "id" : "2ec9b78d-9368-46f3-8f29-d1a95622a568",
    "status" : "ACTIVE",
    "port_id" : "4977b983-cd4f-4ecc-93a1-cb52d848a9b3",
    "public_border_group" : "center",
    "allow_share_bandwidth_types" : [ "share" ]
  }
}
```

## 状态码

|状态码|描述|
|--|--|
|200|GET和PUT操作正常返回|
|400|服务器未能处理请求|
|401|被请求的页面需要用户名和密码|
|403|对被请求页面的访问被禁止|
|404|服务器无法找到被请求的页面|
|405|请求中指定的方法不被允许|
|406|服务器生成的响应无法被客户端所接受|
|407|用户必须首先使用代理服务器进行验证，这样请求才会被处理|
|408|请求超出了服务器的等待时间|
|409|由于冲突，请求无法被完成|
|500|请求未完成。服务异常|
|501|请求未完成。服务器不支持所请求的功能|
|502|请求未完成。服务器从上游服务器收到一个无效的响应|
|503|请求未完成。系统暂时异常|
|504|网关超时|


## 错误码

请参见[错误码](错误码.md)。

