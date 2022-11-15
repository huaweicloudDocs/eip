# 申请EIP\(包年/包月\)<a name="eip_api_0006"></a>

## 功能介绍

申请包年包月的EIP。在成功调用本接口申请包年包月的EIP后：- 如果您需要支付订单，请参考[“支付包周期产品订单”](https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746561.html)进行支付。若想使用优惠券，请将请求中的is\_auto\_pay字段设置为false，参考[“查询订单可用优惠券”](https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0092953630.html)进行支付，或者在华为云官网页面使用优惠券进行支付。- 如果您需要退订该包周期资源，请参考[“退订包周期资源”](https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html)。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=CreatePrePaidPublicip)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

POST /v2.0/\{project\_id\}/publicips

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|project_id|是|String|项目ID，获取项目ID请参见获取项目ID|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


**表 3**  请求Body参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|publicip|是|CreatePrePaidPublicipOption object|EIP对象|
|bandwidth|是|CreatePublicipBandwidthOption object|带宽对象|
|extendParam|否|CreatePrePaidPublicipExtendParamOption object|扩展参数，用于包周期资源申请|
|enterprise_project_id|否|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建弹性公网IP时，给弹性公网IP绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。缺省值：**0**最小长度：**0**最大长度：**36**|


**表 4**  CreatePrePaidPublicipOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|type|是|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最小长度：**0**最大长度：**36**|
|ip_version|否|Integer|功能说明：EIP的版本取值范围：4、6，分别表示创建ipv4和ipv6约束：必须是系统具体支持的类型不填或空字符串时，默认创建ipv4缺省值：**4**枚举值：**4****6**|
|alias|否|String|功能说明：EIP名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最大长度：**64**|
|port_id|否|String|功能说明：端口id 约束：必须是存在的端口id，如果该端口不存在或端口已绑定EIP则会提示出错。最小长度：**36**最大长度：**36**|


**表 5**  CreatePublicipBandwidthOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|charge_mode|否|String|功能说明：按流量计费还是按带宽计费。- -取值范围：bandwidth，traffic，不填或者为空时默认是bandwidth。其中IPv6国外默认是bandwidth，国内默认是traffic。--缺省值：**bandwidth**枚举值：**bandwidth****traffic**|
|id|否|String|功能说明：带宽ID,创建WHOLE类型带宽的EIP时可以指定之前的共享带宽创建取值范围：WHOLE类型的带宽ID最大长度：**36**|
|name|否|String|功能说明：带宽名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）如果share_type是PER，该参数必须带,如果share_type是WHOLE并且id有值，该参数会忽略。最小长度：**1**最大长度：**64**|
|share_type|是|String|功能说明：带宽类型-取值范围：PER，WHOLE（PER为独占带宽，WHOLE是共享带宽）。-- 约束：该字段为WHOLE时，必须指定带宽ID。枚举值：**WHOLE****PER**|
|size|否|Integer|功能说明：带宽大小-取值范围：默认1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。- 约束：share_type是PER，该参数必须带，如果share_type是WHOLE并且id有值，该参数会忽略。- 注意：调整带宽时的最小单位会根据带宽范围不同存在差异。   - 小于等于300Mbit/s：默认最小单位为1Mbit/s。   - 300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。   - 大于1000Mbit/s：默认最小单位为500Mbit/s。|


**表 6**  CreatePrePaidPublicipExtendParamOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|charge_mode|否|String|功能说明：付费方式（预付费、按需付费；预付费，即包周期付费）取值范围：prePaid -预付费，即包年包月；postPaid-后付费，即按需付费；后付费的场景下，extendParam的其他字段都会被忽略。缺省值：**postPaid**枚举值：**prePaid****postPaid**|
|period_type|否|String|功能说明：订购资源的周期类型（包年、包月等）取值范围：month-月year-年约束：如果用包周期共享带宽创建时（即携带共享带宽id创建EIP）此字段可不填。付费方式是预付费且不是使用共享带宽创建IP时，该字段必选； 使用共享带宽创建IP时，带宽资源到期时间与IP的到期时间相同。枚举值：**month****year**|
|period_num|否|Integer|功能说明：订购周期数取值范围：(后续会随运营策略变化)period_type为month时，为[1,9]period_type为year时，为[1,3]约束：同period_type约束。最小值：**1**最大值：**9**|
|is_auto_renew|否|Boolean|功能说明：是否自动续订取值范围： false：不自动续订 true：自动续订约束：到期后，默认自动续订1个月（自动续订时间后续可能会变化），详情可联系客服咨询。缺省值：**false**|
|is_auto_pay|否|Boolean|功能说明：下单订购后，是否自动从客户的账户中支付取值范围：true：自动支付，从账户余额自动扣费false：只提交订单不支付，需要客户手动去支付约束：自动支付时，只能使用账户的现金支付；如果要使用代金券，请选择不自动支付，然后在用户费用中心，选择代金券支付。缺省值：**false**|


## 响应参数

**状态码： 200**

**表 7**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|publicip|PublicipCreateResp object|EIP对象（后付费场景返回对象）|
|order_id|String|订单号（预付费场景返回该字段）最小长度：**0**最大长度：**36**|
|publicip_id|String|EIP的ID（预付费场景返回该字段）最小长度：**0**最大长度：**36**|


**表 8**  PublicipCreateResp

|参数|参数类型|描述|
|--|--|--|
|bandwidth_size|Integer|带宽大小，单位为Mbit/s。|
|create_time|String|EIP申请时间（UTC时间）|
|id|String|EIP唯一标识最大长度：**36**|
|public_ip_address|String|IPv4时是申请到的EIP地址，IPv6时是IPv6地址对应的IPv4地址最大长度：**15**|
|status|String|功能说明：EIP的状态- 取值范围：冻结FREEZED，绑定失败BIND_ERROR，绑定中BINDING，释放中PENDING_DELETE， 创建中PENDING_CREATE，创建中NOTIFYING，释放中NOTIFY_DELETE，更新中PENDING_UPDATE， 未绑定DOWN ，绑定ACTIVE，绑定ELB，绑定VPN，失败ERROR。枚举值：**FREEZED****BIND_ERROR****BINDING****PENDING_DELETE****PENDING_CREATE****NOTIFYING****NOTIFY_DELETE****PENDING_UPDATE****DOWN****ACTIVE****ELB****ERROR****VPN**|
|tenant_id|String|项目ID最大长度：**36**|
|type|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最大长度：**36**|
|public_ipv6_address|String|IPv4时无此字段，IPv6时为申请到的EIP地址最大长度：**39**|
|ip_version|Integer|IP版本信息，取值范围是4和6枚举值：**4****6**|
|enterprise_project_id|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建弹性公网IP时，给弹性公网IP绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。最大长度：**36**|
|alias|String|功能说明：弹性公网IP名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最大长度：**64**|


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

-   创建包周期独占带宽和EIP，大小1Mb，周期1个月。不自动续费，不自动扣费。

    ```
    {
      "publicip" : {
        "type" : "5_bgp"
      },
      "bandwidth" : {
        "name" : "bw_666",
        "size" : 1,
        "share_type" : "PER",
        "charge_mode" : "bandwidth"
      },
      "extendParam" : {
        "charge_mode" : "prePaid",
        "period_type" : "month",
        "period_num" : 1,
        "is_auto_renew" : false,
        "is_auto_pay" : true
      }
    }
    ```

-   创建按需的IP、带宽；extendParam扩展字段，不填即可。

    ```
    {
      "publicip" : {
        "type" : "5_bgp"
      },
      "bandwidth" : {
        "name" : "bw_666",
        "size" : 1,
        "share_type" : "PER",
        "charge_mode" : "bandwidth"
      }
    }
    ```


## 响应示例

**状态码： 200**

POST操作正常返回

```
{
  "application/json-1" : {
    "publicip_id" : "f588ccfa-8750-4d7c-bf5d-2ede24414706",
    "order_id" : "CS1802081410IMDRN"
  },
  "application/json-2" : {
    "publicip" : {
      "tenant_id" : "8b7e35ad379141fc9df3e178bd64f55c",
      "bandwidth_size" : 0,
      "public_ip_address" : "161.17.101.7",
      "create_time" : "2015-07-16 04:10:52",
      "ip_version" : 4,
      "id" : "f588ccfa-8750-4d7c-bf5d-2ede24414706",
      "type" : "5_bgp",
      "status" : "PENDING_CREATE",
      "enterprise_project_id" : "0"
    }
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

