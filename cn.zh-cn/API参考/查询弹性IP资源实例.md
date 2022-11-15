# 查询弹性IP资源实例<a name="eip_apitag_0005"></a>

## 功能介绍

使用标签过滤实例。

## 调试<a name="atuogenerate_1"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=ListPublicipsByTags)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI

POST /v2.0/\{project\_id\}/publicips/resource\_instances/action

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
|tags|否|Array of TagReq objects|包含标签，最多包含10个key。 每个key下面的value最多10个，结构体不能缺失，key不能为空或者空字符串。 Key不能重复，同一个key中values不能重复。|
|limit|否|Integer|查询记录数（action为count时无此参数）如果action为filter默认为1000，limit最多为1000，不能为负数，最小值为1最小值：**1**最大值：**1000**|
|offset|否|Integer|索引位置， 从offset指定的下一条数据开始查询。 查询第一页数据时，不需要传入此参数，查询后续页码数据时，将查询前一页数据时响应体中的值带入此参数（action为count时无此参数）如果action为filter默认为0，必须为数字，不能为负数最小值：**0**|
|action|是|String|操作标识（仅限于filter，count）：filter（过滤），count(查询总条数) 如果是filter就是分页查询，如果是count只需按照条件将总条数返回即可。枚举值：**filter****count**|
|matches|否|Array of MatchReq objects|搜索字段，key为要匹配的字段，当前仅支持resource_name。value为匹配的值。此字段为固定字典值。|


**表 4**  TagReq

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|key|是|String|键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)最大长度：**127**|
|values|是|Array of strings|值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。最大长度：**255**|


**表 5**  MatchReq

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|key|是|String|键。当前仅限定为resource_name枚举值：**resource_name**|
|value|是|String|值。每个值最大长度255个unicode字符。最大长度：**255**|


## 响应参数

**状态码： 200**

**表 6**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|resources|Array of ListResourceResp objects|resource对象列表|
|total_count|Integer|总记录数|


**表 7**  ListResourceResp

|参数|参数类型|描述|
|--|--|--|
|resouce_detail|Object|资源详情。 资源对象，用于扩展。默认为空|
|resource_id|String|资源ID最小长度：**0**最大长度：**36**|
|resource_name|String|资源名称，没有默认为空字符串最小长度：**0**最大长度：**256**|
|tags|Array of ListResourceTagResp objects|标签列表，没有标签默认为空数组|


**表 8**  ListResourceTagResp

|参数|参数类型|描述|
|--|--|--|
|key|String|键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)最小长度：**0**最大长度：**36**|
|value|String|值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。最小长度：**0**最大长度：**43**|


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

-   action为filter时请求体

    ```
    {
      "offset" : 0,
      "limit" : 100,
      "action" : "filter",
      "matches" : [ {
        "key" : "resource_name",
        "value" : "resource1"
      } ],
      "tags" : [ {
        "key" : "key1",
        "values" : [ "value1", "value2" ]
      } ]
    }
    ```

-   action为count时请求体

    ```
    {
      "action" : "count",
      "tags" : [ {
        "key" : "key1",
        "values" : [ "value1", "value2" ]
      }, {
        "key" : "key2",
        "values" : [ "value1", "value2" ]
      } ],
      "matches" : [ {
        "key" : "resource_name",
        "value" : "resource1"
      } ]
    }
    ```


## 响应示例

**状态码： 200**

GET操作正常返回

```
{
  "application/json-1" : {
    "total_count" : 1000,
    "resources" : [ {
      "resource_detail" : null,
      "resource_id" : "cdfs_cefs_wesas_12_dsad",
      "resource_name" : "resouece1",
      "tags" : [ {
        "value" : "value1",
        "key" : "key1"
      }, {
        "value" : "value1",
        "key" : "key2"
      } ]
    } ]
  },
  "application/json-2" : {
    "total_count" : 1000
  }
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

