# 删除弹性公网IP<a name="eip_api_0005"></a>

## 功能介绍<a name="zh-cn_topic_0201534180_section21768161"></a>

删除弹性公网IP。

## URI<a name="zh-cn_topic_0201534180_section61695723"></a>

DELETE /v1/\{project\_id\}/publicips/\{publicip\_id\}

参数说明请参见[表1](#zh-cn_topic_0201534180_table45251091)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534180_table45251091"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534180_row25040094"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534180_p14981763"><a name="zh-cn_topic_0201534180_p14981763"></a><a name="zh-cn_topic_0201534180_p14981763"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534180_p5563313"><a name="zh-cn_topic_0201534180_p5563313"></a><a name="zh-cn_topic_0201534180_p5563313"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534180_p47975183"><a name="zh-cn_topic_0201534180_p47975183"></a><a name="zh-cn_topic_0201534180_p47975183"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534180_row60784581"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534180_p24604028"><a name="zh-cn_topic_0201534180_p24604028"></a><a name="zh-cn_topic_0201534180_p24604028"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534180_p46769243"><a name="zh-cn_topic_0201534180_p46769243"></a><a name="zh-cn_topic_0201534180_p46769243"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534180_p10487112"><a name="zh-cn_topic_0201534180_p10487112"></a><a name="zh-cn_topic_0201534180_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534180_row3475817"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534180_p13105749"><a name="zh-cn_topic_0201534180_p13105749"></a><a name="zh-cn_topic_0201534180_p13105749"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534180_p54932709"><a name="zh-cn_topic_0201534180_p54932709"></a><a name="zh-cn_topic_0201534180_p54932709"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534180_p20364417"><a name="zh-cn_topic_0201534180_p20364417"></a><a name="zh-cn_topic_0201534180_p20364417"></a><span id="zh-cn_topic_0201534180_text106083413176"><a name="zh-cn_topic_0201534180_text106083413176"></a><a name="zh-cn_topic_0201534180_text106083413176"></a></span><span id="zh-cn_topic_0201534180_text16081412170"><a name="zh-cn_topic_0201534180_text16081412170"></a><a name="zh-cn_topic_0201534180_text16081412170"></a>弹性公网IP</span>唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534180_section18390601"></a>

-   请求参数

    无

-   请求样例

    ```
    DELETE https://{Endpoint}/v1/{project_id}/publicips
    ```


## 响应消息<a name="zh-cn_topic_0201534180_section31297682"></a>

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


## 状态码<a name="zh-cn_topic_0201534180_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534180_section85821649202813"></a>

请参考[错误码](错误码.md)。

