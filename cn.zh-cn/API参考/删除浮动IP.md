# 删除浮动IP<a name="eip_openstackapi_0010"></a>

## 功能介绍

删除浮动IP。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=NeutronDeleteFloatingIp)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

DELETE /v2.0/floatingips/\{floatingip\_id\}

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|floatingip_id|是|String|floatingip的ID|


## 请求参数

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


## 响应参数

**状态码： 400**

**表 3**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 4**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 401**

**表 5**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|NeutronError|NeutronError object|Neutron服务异常|


**表 6**  NeutronError

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|type|String|服务异常错误类型最小长度：**0**最大长度：**64**|
|detail|String|服务异常错误详情最小长度：**0**最大长度：**256**|


**状态码： 403**

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


**状态码： 404**

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


**状态码： 405**

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


**状态码： 406**

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


**状态码： 407**

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


**状态码： 408**

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


**状态码： 409**

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


**状态码： 500**

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


**状态码： 501**

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


**状态码： 502**

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


**状态码： 503**

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


**状态码： 504**

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


## 请求示例

```
DELETE https://{Endpoint}/v2.0/floatingips/a95ec431-8473-463b-aede-34fb048ee3a7
```

## 响应示例

无

## 状态码

|状态码|描述|
|--|--|
|204|DELETE操作正常返回|
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

