# 共享带宽插入EIP<a name="eip_apisharedbandwidth_0004"></a>

## 功能介绍

共享带宽插入EIP。

## 接口约束

在共享带宽中批量插入EIP时，一次可批量操作100个EIP。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=AddPublicipsIntoSharedBandwidth)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/insert

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|project_id|是|String|项目ID，获取项目ID请参见获取项目ID|
|bandwidth_id|是|String|带宽唯一标识|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


**表 3**  请求Body参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|bandwidth|是|AddPublicipsIntoSharedBandwidthOption object|带宽对象|


**表 4**  AddPublicipsIntoSharedBandwidthOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|publicip_info|是|Array of InsertPublicipInfo objects|功能说明：要插入共享带宽的EIP信息或者IPv6端口- 约束：WHOLE类型的带宽支持多个EIP或者IPv6端口，跟租户的配额相关，默认一个共享带宽的配额为20|


**表 5**  InsertPublicipInfo

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|publicip_type|否|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最大长度：**36**|
|publicip_id|是|String|功能说明：带宽对应的EIP或者IPv6端口PORT的唯一标识最大长度：**36**|


## 响应参数

**状态码： 200**

**表 6**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|bandwidth|BandwidthRespInsert object|带宽对象|


**表 7**  BandwidthRespInsert

|参数|参数类型|描述|
|--|--|--|
|bandwidth_type|String|功能说明：带宽类型，共享带宽默认为share。取值范围：share，bgp，sbgp等。share：共享带宽bgp：动态bgpsbgp：静态bgp最小长度：**1**最大长度：**36**|
|charge_mode|String|功能说明：按流量计费,按带宽计费还是按增强型95计费。取值范围：bandwidth（按带宽计费），traffic（按流量计费），95peak_plus（按增强型95计费）不返回或者为空时表示是bandwidth。约束：只有共享带宽支持95peak_plus（按增强型95计费），按增强型95计费时需要指定保底百分比，默认是20%。枚举值：**bandwidth****traffic****95peak_plus**|
|id|String|功能说明：带宽唯一标识最大长度：**36**|
|name|String|功能说明：带宽名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最小长度：**1**最大长度：**64**|
|publicip_info|Array of PublicipInfoResp objects|功能说明：带宽对应的弹性公网IP信息约束：WHOLE类型的带宽支持多个弹性公网IP，PER类型的带宽只能对应一个弹性公网IP|
|billing_info|String|功能说明：账单信息 如果billinginfo不为空，说明是包周期的带宽最小长度：**0**最大长度：**255**|
|share_type|String|功能说明：带宽类型，标识是否是共享带宽取值范围：WHOLE，PERWHOLE表示共享带宽PER表示独享带宽枚举值：**WHOLE****PER**|
|size|Integer|功能说明：带宽大小。- 取值范围：默认5Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。|
|tenant_id|String|功能说明：用户所属租户ID最大长度：**36**|
|enterprise_project_id|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建共享带宽时，给共享带宽绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。最大长度：**36**|
|status|String|功能说明：带宽的状态取值范围：FREEZED：冻结NORMAL：正常枚举值：**FREEZED****NORMAL**|


**表 8**  PublicipInfoResp

|参数|参数类型|描述|
|--|--|--|
|publicip_address|String|功能说明：EIP或者IPv6端口的地址最大长度：**15**|
|publicip_id|String|功能说明：带宽对应的EIP或者IPv6端口的唯一标识最大长度：**36**|
|publicip_type|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最大长度：**36**|
|publicipv6_address|String|功能说明：IPv4时无此字段，IPv6时为申请到的EIP地址最大长度：**39**|
|ip_version|Integer|IP版本信息取值范围：4：IPv46：IPv6枚举值：**4****6**|


**状态码： 400**

**表 9**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 401**

**表 10**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 403**

**表 11**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 404**

**表 12**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 405**

**表 13**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 406**

**表 14**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 407**

**表 15**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 408**

**表 16**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 409**

**表 17**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 500**

**表 18**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 501**

**表 19**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 502**

**表 20**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 503**

**表 21**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 504**

**表 22**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


## 请求示例

```
{
  "bandwidth" : {
    "publicip_info" : [ {
      "publicip_id" : "d91b0028-6f6b-4478-808a-297b75b6812a",
      "publicip_type" : "5_dualStack"
    }, {
      "publicip_id" : "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f"
    } ]
  }
}
```

## 响应示例

**状态码： 200**

POST操作正常返回

```
{
  "bandwidth" : {
    "tenant_id" : "8b7e35ad379141fc9df3e178bd64f55c",
    "billing_info" : "CS1712121146TSQOJ:0616e2a5dc9f4985ba52ea8c0c7e273c:southchina:35f2b308f5d64441a6fa7999fbcd4321",
    "size" : 10,
    "share_type" : "WHOLE",
    "bandwidth_type" : "share",
    "publicip_info" : [ {
      "publicip_id" : "d91b0028-6f6b-4478-808a-297b75b6812a",
      "ip_version" : 4,
      "publicip_type" : "5_dualStack",
      "publicip_address" : "::ffff:192.168.89.9"
    }, {
      "publicip_id" : "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f",
      "ip_version" : 4,
      "publicip_type" : "5_bgp",
      "publicip_address" : "99.xx.xx.82"
    } ],
    "name" : "bandwidth123",
    "enable_bandwidth_rules" : false,
    "rule_quota" : 0,
    "bandwidth_rules" : [ ],
    "charge_mode" : "bandwidth",
    "id" : "3fa5b383-5a73-4dcb-a314-c6128546d855"
  }
}
```

## 状态码

|状态码|描述|
|--|--|
|200|POST操作正常返回|
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

