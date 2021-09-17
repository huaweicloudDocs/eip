# 批量创建和删除弹性IP资源标签<a name="eip_apitag_0004"></a>

## 功能介绍<a name="zh-cn_topic_0201534168_section16984350162413"></a>

为指定的弹性IP资源实例批量添加或删除标签。

此接口为幂等接口：

创建时如果请求体中存在重复key则报错。

创建时，不允许设置重复key数据，如果数据库已存在该key，就覆盖value的值。

删除时，如果删除的标签不存在，默认处理成功，删除时不对标签字符集范围做校验。删除时tags结构体不能缺失，key不能为空，或者空字符串。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”区域开放。

## URI<a name="zh-cn_topic_0201534168_section49844500244"></a>

POST /v2.0/\{project\_id\}/publicips/\{publicip\_id\}/tags/action

参数说明请参见[表1](#zh-cn_topic_0201534168_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534168_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534168_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534168_p47174532"><a name="zh-cn_topic_0201534168_p47174532"></a><a name="zh-cn_topic_0201534168_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534168_p63040734"><a name="zh-cn_topic_0201534168_p63040734"></a><a name="zh-cn_topic_0201534168_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534168_p6025849"><a name="zh-cn_topic_0201534168_p6025849"></a><a name="zh-cn_topic_0201534168_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534168_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534168_p8478608"><a name="zh-cn_topic_0201534168_p8478608"></a><a name="zh-cn_topic_0201534168_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534168_p15678685"><a name="zh-cn_topic_0201534168_p15678685"></a><a name="zh-cn_topic_0201534168_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534168_p10487112"><a name="zh-cn_topic_0201534168_p10487112"></a><a name="zh-cn_topic_0201534168_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534168_row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534168_p43913021"><a name="zh-cn_topic_0201534168_p43913021"></a><a name="zh-cn_topic_0201534168_p43913021"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534168_p184914"><a name="zh-cn_topic_0201534168_p184914"></a><a name="zh-cn_topic_0201534168_p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534168_p14978051"><a name="zh-cn_topic_0201534168_p14978051"></a><a name="zh-cn_topic_0201534168_p14978051"></a>EIP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534168_section1799117501243"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534168_table8992250172415"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534168_row3711351132413"><th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534168_p471145111242"><a name="zh-cn_topic_0201534168_p471145111242"></a><a name="zh-cn_topic_0201534168_p471145111242"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534168_p47115515247"><a name="zh-cn_topic_0201534168_p47115515247"></a><a name="zh-cn_topic_0201534168_p47115515247"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.509999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534168_p10711051202417"><a name="zh-cn_topic_0201534168_p10711051202417"></a><a name="zh-cn_topic_0201534168_p10711051202417"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.49%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534168_p117218511241"><a name="zh-cn_topic_0201534168_p117218511241"></a><a name="zh-cn_topic_0201534168_p117218511241"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534168_row572951152420"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534168_p17721851132411"><a name="zh-cn_topic_0201534168_p17721851132411"></a><a name="zh-cn_topic_0201534168_p17721851132411"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534168_p072551172414"><a name="zh-cn_topic_0201534168_p072551172414"></a><a name="zh-cn_topic_0201534168_p072551172414"></a>Array of <a href="#zh-cn_topic_0201534168_table13242848193719">tag</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534168_p7721851162410"><a name="zh-cn_topic_0201534168_p7721851162410"></a><a name="zh-cn_topic_0201534168_p7721851162410"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.49%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534168_p67265110244"><a name="zh-cn_topic_0201534168_p67265110244"></a><a name="zh-cn_topic_0201534168_p67265110244"></a>tag对象列表，请参见<a href="#zh-cn_topic_0201534168_table13242848193719">表3</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534168_row57295120245"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534168_p572115152417"><a name="zh-cn_topic_0201534168_p572115152417"></a><a name="zh-cn_topic_0201534168_p572115152417"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534168_p12724511244"><a name="zh-cn_topic_0201534168_p12724511244"></a><a name="zh-cn_topic_0201534168_p12724511244"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534168_p3721951162417"><a name="zh-cn_topic_0201534168_p3721951162417"></a><a name="zh-cn_topic_0201534168_p3721951162417"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.49%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534168_p1562014114112"><a name="zh-cn_topic_0201534168_p1562014114112"></a><a name="zh-cn_topic_0201534168_p1562014114112"></a>操作标识：</p>
    <a name="zh-cn_topic_0201534168_ul2205152413110"></a><a name="zh-cn_topic_0201534168_ul2205152413110"></a><ul id="zh-cn_topic_0201534168_ul2205152413110"><li>create：创建</li><li>delete：删除</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag对象

    <a name="zh-cn_topic_0201534168_table13242848193719"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534168_row13343144812379"><th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534168_p15343174853715"><a name="zh-cn_topic_0201534168_p15343174853715"></a><a name="zh-cn_topic_0201534168_p15343174853715"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534168_p13431648163716"><a name="zh-cn_topic_0201534168_p13431648163716"></a><a name="zh-cn_topic_0201534168_p13431648163716"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534168_p169809965412"><a name="zh-cn_topic_0201534168_p169809965412"></a><a name="zh-cn_topic_0201534168_p169809965412"></a>必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.699999999999996%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534168_p11344748183719"><a name="zh-cn_topic_0201534168_p11344748183719"></a><a name="zh-cn_topic_0201534168_p11344748183719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534168_row103449487379"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534168_p183469482373"><a name="zh-cn_topic_0201534168_p183469482373"></a><a name="zh-cn_topic_0201534168_p183469482373"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534168_p1434684863710"><a name="zh-cn_topic_0201534168_p1434684863710"></a><a name="zh-cn_topic_0201534168_p1434684863710"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534168_p298018911544"><a name="zh-cn_topic_0201534168_p298018911544"></a><a name="zh-cn_topic_0201534168_p298018911544"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534168_row2346548163714"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534168_p1134624816377"><a name="zh-cn_topic_0201534168_p1134624816377"></a><a name="zh-cn_topic_0201534168_p1134624816377"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534168_p234619483371"><a name="zh-cn_topic_0201534168_p234619483371"></a><a name="zh-cn_topic_0201534168_p234619483371"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534168_p209805915417"><a name="zh-cn_topic_0201534168_p209805915417"></a><a name="zh-cn_topic_0201534168_p209805915417"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0201534168_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例1：批量创建标签

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags/action
    
    {
        "action": "create",
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


-   请求样例2：批量删除标签

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags/action
    
    {
        "action": "delete",
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


## 响应消息<a name="zh-cn_topic_0201534168_section173510241"></a>

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


## 状态码<a name="zh-cn_topic_0201534168_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534168_section85821649202813"></a>

请参考[错误码](错误码.md)。

