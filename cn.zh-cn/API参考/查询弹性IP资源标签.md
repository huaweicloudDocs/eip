# 查询弹性IP资源标签<a name="eip_apitag_0002"></a>

## 功能介绍<a name="zh-cn_topic_0201534160_section131671842412"></a>

查询指定弹性IP实例的标签信息。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”、“华南-广州”区域开放。

## URI<a name="zh-cn_topic_0201534160_section731781892418"></a>

GET /v2.0/\{project\_id\}/publicips/\{publicip\_id\}/tags

参数说明请参见[表1](#zh-cn_topic_0201534160_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534160_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534160_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534160_p47174532"><a name="zh-cn_topic_0201534160_p47174532"></a><a name="zh-cn_topic_0201534160_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534160_p63040734"><a name="zh-cn_topic_0201534160_p63040734"></a><a name="zh-cn_topic_0201534160_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534160_p6025849"><a name="zh-cn_topic_0201534160_p6025849"></a><a name="zh-cn_topic_0201534160_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534160_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534160_p8478608"><a name="zh-cn_topic_0201534160_p8478608"></a><a name="zh-cn_topic_0201534160_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534160_p15678685"><a name="zh-cn_topic_0201534160_p15678685"></a><a name="zh-cn_topic_0201534160_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534160_p10487112"><a name="zh-cn_topic_0201534160_p10487112"></a><a name="zh-cn_topic_0201534160_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534160_row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534160_p725824594416"><a name="zh-cn_topic_0201534160_p725824594416"></a><a name="zh-cn_topic_0201534160_p725824594416"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534160_p184914"><a name="zh-cn_topic_0201534160_p184914"></a><a name="zh-cn_topic_0201534160_p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534160_p14978051"><a name="zh-cn_topic_0201534160_p14978051"></a><a name="zh-cn_topic_0201534160_p14978051"></a>EIP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534160_section12330418152420"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags
    ```


## 响应消息<a name="zh-cn_topic_0201534160_section83301318102415"></a>

-   响应参数

    **表 2**  响应参数

    <a name="zh-cn_topic_0201534160_table2033011815242"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534160_row4392171813241"><th class="cellrowborder" valign="top" width="13.33%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534160_p10392181872410"><a name="zh-cn_topic_0201534160_p10392181872410"></a><a name="zh-cn_topic_0201534160_p10392181872410"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.11%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534160_p939231813249"><a name="zh-cn_topic_0201534160_p939231813249"></a><a name="zh-cn_topic_0201534160_p939231813249"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="65.56%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534160_p93927180241"><a name="zh-cn_topic_0201534160_p93927180241"></a><a name="zh-cn_topic_0201534160_p93927180241"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534160_row163921181243"><td class="cellrowborder" valign="top" width="13.33%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534160_p1739281812410"><a name="zh-cn_topic_0201534160_p1739281812410"></a><a name="zh-cn_topic_0201534160_p1739281812410"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.11%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534160_p1239241812243"><a name="zh-cn_topic_0201534160_p1239241812243"></a><a name="zh-cn_topic_0201534160_p1239241812243"></a>Array of <a href="#zh-cn_topic_0201534160_table13242848193719">tag</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.56%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534160_p143926189247"><a name="zh-cn_topic_0201534160_p143926189247"></a><a name="zh-cn_topic_0201534160_p143926189247"></a>tag对象列表，请参见<a href="#zh-cn_topic_0201534160_table13242848193719">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag对象

    <a name="zh-cn_topic_0201534160_table13242848193719"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534160_row13343144812379"><th class="cellrowborder" valign="top" width="14.78%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534160_p15343174853715"><a name="zh-cn_topic_0201534160_p15343174853715"></a><a name="zh-cn_topic_0201534160_p15343174853715"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.67%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534160_p13431648163716"><a name="zh-cn_topic_0201534160_p13431648163716"></a><a name="zh-cn_topic_0201534160_p13431648163716"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="65.55%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534160_p11344748183719"><a name="zh-cn_topic_0201534160_p11344748183719"></a><a name="zh-cn_topic_0201534160_p11344748183719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534160_row103449487379"><td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534160_p183469482373"><a name="zh-cn_topic_0201534160_p183469482373"></a><a name="zh-cn_topic_0201534160_p183469482373"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534160_p1434684863710"><a name="zh-cn_topic_0201534160_p1434684863710"></a><a name="zh-cn_topic_0201534160_p1434684863710"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.55%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534160_row2346548163714"><td class="cellrowborder" valign="top" width="14.78%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534160_p1134624816377"><a name="zh-cn_topic_0201534160_p1134624816377"></a><a name="zh-cn_topic_0201534160_p1134624816377"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.67%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534160_p234619483371"><a name="zh-cn_topic_0201534160_p234619483371"></a><a name="zh-cn_topic_0201534160_p234619483371"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.55%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0201534160_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "tags": [
            {
                "key": "key1",
                "value": "value1"
            },
            {
                "key": "key2",
                "value": "value3"
            }
        ]
    }
    ```


## 状态码<a name="zh-cn_topic_0201534160_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534160_section85821649202813"></a>

请参考[错误码](错误码.md)。

