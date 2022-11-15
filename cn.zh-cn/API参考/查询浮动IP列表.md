# 查询浮动IP列表<a name="eip_openstackapi_0006"></a>

## 功能介绍

查询提交请求的租户有权限操作的所有浮动IP地址。单次查询最多返回2000条数据，超过2000后会返回分页标记。

## 接口约束

单次查询最多返回2000条数据，超过2000后会返回分页标记。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=NeutronListFloatingIps)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

GET /v2.0/floatingips

**表 1**  Query参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|limit|否|Integer|分页查询每页返回的记录个数，取值范围为0~intmax。 limit需要和marker配合使用，详细规则请见marker的参数说明最小值：**0**最大值：**2000**|
|marker|否|String|分页查询的起始资源ID，表示从指定资源的下一条记录开始查询。 marker需要和limit配合使用：若不传入marker和limit参数，查询结果返回全部资源记录。若不传入marker参数，limit为10，查询结果返回第1~10条资源记录。若marker为第10条记录的资源ID，limit为10，查询结果返回第11~20条资源记录。若marker为第10条记录的资源ID，不传入limit参数，查询结果返回第11条及之后的所有资源记录。最小长度：**0**最大长度：**36**|
|page_reverse|否|Boolean|False/True，是否设置分页的顺序。|
|id|否|String|浮动IP的id。最小长度：**0**最大长度：**36**|
|floating_ip_address|否|String|浮动IP地址（IPv4格式）。最小长度：**0**最大长度：**64**|
|router_id|否|String|所属路由器id。最小长度：**0**最大长度：**36**|
|port_id|否|String|端口id。最小长度：**0**最大长度：**36**|
|fixed_ip_address|否|String|关联端口的私有IP地址。最小长度：**0**最大长度：**64**|
|tenant_id|否|String|项目ID。最小长度：**0**最大长度：**36**|
|floating_network_id|否|String|外部网络的id。只能使用固定的外网，外部网络的信息请通过GET /v2.0/networks?router:external=True或GET /v2.0/networks?name={floating_network}或neutron net-external-list方式查询最小长度：**0**最大长度：**36**|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）最小长度：**0**最大长度：**4096**|


## 响应参数

**状态码： 200**

**表 3**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|floatingips|Array of FloatingIpResp objects|floatingip对象列表|
|floatingips_links|Array of Pager objects|floatingips_link对象列表|


**表 4**  FloatingIpResp

|参数|参数类型|描述|
|--|--|--|
|fixed_ip_address|String|关联端口的私有IP地址。最小长度：**0**最大长度：**64**|
|floating_ip_address|String|浮动IP地址。最小长度：**0**最大长度：**64**|
|floating_network_id|String|外部网络id最小长度：**0**最大长度：**36**|
|id|String|浮动IP地址的id。最小长度：**0**最大长度：**36**|
|port_id|String|端口id最小长度：**0**最大长度：**36**|
|router_id|String|所属路由器id。最小长度：**0**最大长度：**36**|
|status|String|网络状态，可以为ACTIVE， DOWN或ERROR。DOWN：未绑定ACTIVE：绑定ERROR：异常枚举值：**ACTIVE****DOWN****ERROR**|
|tenant_id|String|项目id。最小长度：**0**最大长度：**36**|
|project_id|String|项目id。最小长度：**0**最大长度：**36**|
|dns_name|String|DNS名称 该参数当前仅在“华南-广州”开放最小长度：**0**最大长度：**255**|
|dns_domain|String|DNS域地址 该参数当前仅在“华南-广州”开放最小长度：**0**最大长度：**255**|
|created_at|String|资源创建时间 采用UTC时间 格式：YYYY-MM-DDTHH:MM:SS|
|updated_at|String|资源更新时间 采用UTC时间 格式：YYYY-MM-DDTHH:MM:SS|


**表 5**  Pager

|参数|参数类型|描述|
|--|--|--|
|href|String|页码url最小长度：**0**最大长度：**256**|
|rel|String|next:下一页 previous:前一页枚举值：**next****previous**|


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

-   ```
GET https://{Endpoint}/v2.0/floatingips?limit=1
```

-   ```
GET https://{Endpoint}/v2.0/floatingips?id={fip_id}&router_id={router_id}&floating_network_id={net_id}&floating_ip_address={floating_ip}&port_id={port_id}&fixed_ip_address={fixed_ip}&tenant_id={tenant_id}
```


## 响应示例

**状态码： 200**

GET操作正常返回

```
{
  "floatingips" : [ {
    "id" : "1a3a2818-d9b4-4a9c-8a19-5252c499d1cd",
    "status" : "DOWN",
    "router_id" : null,
    "tenant_id" : "bbfe8c41dd034a07bebd592bf03b4b0c",
    "project_id" : "bbfe8c41dd034a07bebd592bf03b4b0c",
    "floating_network_id" : "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
    "fixed_ip_address" : null,
    "floating_ip_address" : "99.99.99.84",
    "port_id" : null,
    "dns_name" : "ecs-88-99-103-61",
    "dns_domain" : "compute.hwclouds-dns.com.",
    "created_at" : "2017-10-19T12:21:28",
    "updated_at" : "2018-07-30T12:52:13"
  } ],
  "floatingips_links" : [ {
    "href" : "https://network.region.cn-southwest-2.hwclouds.com/v2.0/floatingips.json?limit=2000&marker=000a6144-5010-46f2-bf06-6a1c94477ea3&page_reverse=true",
    "rel" : "previous"
  }, {
    "href" : "https://network.region.cn-southwest-2.hwclouds.com/v2.0/floatingips.json?limit=2000&marker=d445e537-bc81-4039-9c7b-f9c1f5c73c78",
    "rel" : "next"
  } ]
}
```

## 状态码

|状态码|描述|
|--|--|
|200|GET操作正常返回|
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

