# 删除弹性IP资源标签<a name="eip_apitag_0003"></a>

## 功能介绍<a name="zh-cn_topic_0201534220_section13639163252413"></a>

删除指定弹性IP资源实例的标签信息。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”区域开放。

## URI<a name="zh-cn_topic_0201534220_section264093272413"></a>

DELETE /v2.0/\{project\_id\}/publicips/\{publicip\_id\}/tags/\{key\}

参数说明请参见[表1](#zh-cn_topic_0201534220_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534220_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534220_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534220_p47174532"><a name="zh-cn_topic_0201534220_p47174532"></a><a name="zh-cn_topic_0201534220_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534220_p63040734"><a name="zh-cn_topic_0201534220_p63040734"></a><a name="zh-cn_topic_0201534220_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534220_p6025849"><a name="zh-cn_topic_0201534220_p6025849"></a><a name="zh-cn_topic_0201534220_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534220_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534220_p8478608"><a name="zh-cn_topic_0201534220_p8478608"></a><a name="zh-cn_topic_0201534220_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534220_p15678685"><a name="zh-cn_topic_0201534220_p15678685"></a><a name="zh-cn_topic_0201534220_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534220_p10487112"><a name="zh-cn_topic_0201534220_p10487112"></a><a name="zh-cn_topic_0201534220_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534220_row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534220_p43913021"><a name="zh-cn_topic_0201534220_p43913021"></a><a name="zh-cn_topic_0201534220_p43913021"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534220_p184914"><a name="zh-cn_topic_0201534220_p184914"></a><a name="zh-cn_topic_0201534220_p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534220_p14978051"><a name="zh-cn_topic_0201534220_p14978051"></a><a name="zh-cn_topic_0201534220_p14978051"></a>EIP唯一标识</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534220_row172919431459"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534220_p8234174425110"><a name="zh-cn_topic_0201534220_p8234174425110"></a><a name="zh-cn_topic_0201534220_p8234174425110"></a>key</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534220_p11234114455116"><a name="zh-cn_topic_0201534220_p11234114455116"></a><a name="zh-cn_topic_0201534220_p11234114455116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534220_p3234194414511"><a name="zh-cn_topic_0201534220_p3234194414511"></a><a name="zh-cn_topic_0201534220_p3234194414511"></a>标签的键值</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534220_section6649132102410"></a>

-   请求参数

    无

-   请求样例

    ```
    DELETE https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags/{key}
    ```


## 响应消息<a name="zh-cn_topic_0201534220_section76491632142420"></a>

-   响应参数

    无

-   响应样例

    无

    或

    ```
    {
           "code":"xxx",
           "message":"xxxxx"
    }
    ```


## 状态码<a name="zh-cn_topic_0201534220_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534220_section85821649202813"></a>

请参考[错误码](错误码.md)。

