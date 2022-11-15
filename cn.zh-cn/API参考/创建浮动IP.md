# 创建浮动IP<a name="eip_openstackapi_0008"></a>

## 功能介绍

创建浮动IP的外部网络UUID，请使用GET /v2.0/networks?router:external=True或neutron net-external-list方式获取。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=NeutronCreateFloatingIp)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

POST /v2.0/floatingips

## 请求参数

**表 1**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


**表 2**  请求Body参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|floatingip|是|CreateFloatingIpOption object|创建floatingip对象|


**表 3**  CreateFloatingIpOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|floating_ip_address|否|String|浮动IP地址。最大长度：**64**|
|floating_network_id|是|String|外部网络的id。只能使用固定的外网，外部网络的信息请通过GET /v2.0/networks?router:external=True或GET /v2.0/networks?name={floating_network}或neutron net-external-list方式查询。|
|port_id|否|String|端口id最大长度：**36**|
|fixed_ip_address|否|String|关联端口的私有IP地址。最大长度：**64**|


## 响应参数

**状态码： 201**

**表 4**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|floatingip|PostAndPutFloatingIpResp object|floatingip对象|


**表 5**  PostAndPutFloatingIpResp

|参数|参数类型|描述|
|--|--|--|
|fixed_ip_address|String|关联端口的私有IP地址。最小长度：**0**最大长度：**64**|
|floating_ip_address|String|浮动IP地址。最小长度：**0**最大长度：**64**|
|floating_network_id|String|外部网络的id。最小长度：**0**最大长度：**36**|
|id|String|浮动IP地址的id。最小长度：**0**最大长度：**36**|
|port_id|String|端口id。最小长度：**0**最大长度：**36**|
|router_id|String|所属路由器id。最小长度：**0**最大长度：**36**|
|status|String|网络状态，可以为ACTIVE， DOWN或ERROR。DOWN：未绑定ACTIVE：绑定ERROR：异常枚举值：**ACTIVE****DOWN****ERROR**|
|tenant_id|String|项目id。最小长度：**0**最大长度：**36**|
|dns_name|String|DNS名称 该参数当前仅在“华南-广州”开放最小长度：**0**最大长度：**255**|
|dns_domain|String|DNS域地址 该参数当前仅在“华南-广州”开放最小长度：**0**最大长度：**255**|


**状态码： 400**

**表 6**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 7**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 401**

**表 8**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 9**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 403**

**表 10**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 11**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 404**

**表 12**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 13**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 405**

**表 14**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 15**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 406**

**表 16**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 17**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 407**

**表 18**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 19**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 408**

**表 20**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 21**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 409**

**表 22**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 23**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 500**

**表 24**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 25**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 501**

**表 26**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 27**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 502**

**表 28**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 29**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 503**

**表 30**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 31**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 504**

**表 32**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 33**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


## 请求示例

```
POST https://{Endpoint}/v2.0/floatingips {"floatingip": {"floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975"}}
```

## 响应示例

**状态码： 201**

POST操作正常返回

```
{
  "floatingip" : {
    "id" : "1a3a2818-d9b4-4a9c-8a19-5252c499d1cd",
    "status" : "DOWN",
    "router_id" : null,
    "tenant_id" : "bbfe8c41dd034a07bebd592bf03b4b0c",
    "floating_network_id" : "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
    "fixed_ip_address" : null,
    "floating_ip_address" : "88.88.215.205",
    "port_id" : null,
    "dns_name" : "ecs-88-99-103-61",
    "dns_domain" : "compute.hwclouds-dns.com."
  }
}
```

## 状态码

|状态码|描述|
|--|--|
|201|POST操作正常返回|
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

