# 更新浮动IP<a name="eip_openstackapi_0009"></a>

## 功能介绍

更新浮动IP。 更新时需在URL中给出浮动IP地址的ID。 port\_id 为空，则表示浮动IP从端口解绑。

该接口有以下使用约束：

-   绑定浮动IP过程中，如果浮动IP处于“error”状态，请先尝试执行浮动IP解绑定动作。

-   不支持直接把已经绑定浮动IP的端口重新绑定到另外一个浮动IP上，必须先解绑再绑定。


## 接口约束

绑定浮动IP过程中，如果浮动IP处于“error”状态，请先尝试执行浮动IP解绑定动作。不支持直接把已经绑定端口的浮动ip重新绑定到另外一个端口上，必须先解绑定再绑定。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=NeutronUpdateFloatingIp)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

PUT /v2.0/floatingips/\{floatingip\_id\}

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|floatingip_id|是|String|浮动IP地址的id。 【使用说明】创建浮动IP时不选，查询，更新，删除时是必选。最小长度：**0**最大长度：**36**|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）最小长度：**0**最大长度：**4096**|


**表 3**  请求Body参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|floatingip|是|UpdateFloatingIpOption object|更新floatingip对象|


**表 4**  UpdateFloatingIpOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|port_id|否|String|端口id。最小长度：**0**最大长度：**36**|


## 响应参数

**状态码： 200**

**表 5**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|floatingip|PostAndPutFloatingIpResp object|floatingip对象|


**表 6**  PostAndPutFloatingIpResp

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

**表 7**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 8**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 401**

**表 9**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 10**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 403**

**表 11**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 12**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 404**

**表 13**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 14**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 405**

**表 15**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 16**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 406**

**表 17**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 18**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 407**

**表 19**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 20**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 408**

**表 21**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 22**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 409**

**表 23**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 24**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 500**

**表 25**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 26**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 501**

**表 27**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 28**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 502**

**表 29**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 30**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 503**

**表 31**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 32**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 504**

**表 33**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 34**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


## 请求示例

-   ```
{
  "floatingip" : {
    "port_id" : null
  }
}
```

-   ```
{
  "floatingip" : {
    "port_id" : "f91f5763-c5a2-4458-979d-61e48b3c3fac"
  }
}
```


## 响应示例

**状态码： 200**

GET和PUT操作正常返回

```
{
  "application/json-1" : {
    "floatingip" : {
      "id" : "b997e0d4-3359-4c74-8f88-bc0af81cd5a2",
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
  },
  "application/json-2" : {
    "floatingip" : {
      "id" : "b997e0d4-3359-4c74-8f88-bc0af81cd5a2",
      "status" : "DOWN",
      "router_id" : null,
      "tenant_id" : "bbfe8c41dd034a07bebd592bf03b4b0c",
      "project_id" : "bbfe8c41dd034a07bebd592bf03b4b0c",
      "floating_network_id" : "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
      "fixed_ip_address" : "192.168.10.3",
      "floating_ip_address" : "88.88.215.205",
      "port_id" : "00587256-27e3-489b-96bf-ea80c1da4aeb",
      "created_at" : "2018-09-20T02:10:02",
      "updated_at" : "2018-09-20T02:10:07"
    }
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

