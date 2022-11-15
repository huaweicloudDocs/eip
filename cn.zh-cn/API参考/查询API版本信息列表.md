# 查询API版本信息列表<a name="eip_openstackapi_0002"></a>

## 功能介绍<a name="zh-cn_topic_0201534229_section47928120"></a>

返回当前API所有可用的版本（仅针对OpenStack原生接口）。

## 调试<a name="zh-cn_topic_0201534229_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=VPC&version=v2&api=ListApiVersion)中调试该接口。

## URI<a name="zh-cn_topic_0201534229_section28699899"></a>

GET /

## 请求消息<a name="zh-cn_topic_0201534229_section42990474"></a>

请求参数

无

请求样例

```
GET https://{Endpoint}/
```

## 响应消息<a name="zh-cn_topic_0201534229_section51369953"></a>

响应参数

**表 1**  响应参数

|参数名称|类型|说明|
|--|--|--|
|versions|Array of version objects|API版本列表，请参见表2。|


**表 2**  version对象

|参数名称|类型|说明|
|--|--|--|
|status|String|API版本的状态：CURRENT（当前版本）STABLE（稳定版本）DEPRECATED（废弃版本）|
|id|String|API版本|
|links|Array of link objects|链接列表，请参见表3。|


**表 3**  link对象

|参数名称|类型|说明|
|--|--|--|
|href|String|API链接|
|rel|String|API链接与该API版本的关系|


响应样例

```
{
    "versions": [
        {
            "status": "CURRENT", 
            "id": "v2.0", 
            "links": [
                {
                    "href": "https://None/v2.0", 
                    "rel": "self"
                }
            ]
        }
    ]
}
```

## 状态码<a name="zh-cn_topic_0201534229_section10470352390"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534229_section85821649202813"></a>

请参见[错误码](错误码.md)。

