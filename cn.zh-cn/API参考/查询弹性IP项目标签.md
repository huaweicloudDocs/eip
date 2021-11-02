# 查询弹性IP项目标签<a name="eip_apitag_0006"></a>

## 功能介绍<a name="zh-cn_topic_0201534134_section5413192818251"></a>

查询租户在指定区域和实例类型的所有标签集合。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”、“华南-广州”区域开放。

## URI<a name="zh-cn_topic_0201534134_section1414182816254"></a>

GET /v2.0/\{project\_id\}/publicips/tags

参数说明请参见[表1](#zh-cn_topic_0201534134_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534134_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534134_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534134_p47174532"><a name="zh-cn_topic_0201534134_p47174532"></a><a name="zh-cn_topic_0201534134_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534134_p63040734"><a name="zh-cn_topic_0201534134_p63040734"></a><a name="zh-cn_topic_0201534134_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534134_p6025849"><a name="zh-cn_topic_0201534134_p6025849"></a><a name="zh-cn_topic_0201534134_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534134_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534134_p8478608"><a name="zh-cn_topic_0201534134_p8478608"></a><a name="zh-cn_topic_0201534134_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534134_p15678685"><a name="zh-cn_topic_0201534134_p15678685"></a><a name="zh-cn_topic_0201534134_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534134_p10487112"><a name="zh-cn_topic_0201534134_p10487112"></a><a name="zh-cn_topic_0201534134_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534134_section1342142882511"></a>

-   请求参数

    无

-   请求样例

    ```
    GET /v2.0/{project_id}/publicips/tags
    ```


## 响应消息<a name="zh-cn_topic_0201534134_section242122862514"></a>

-   响应参数

    **表 2**  响应参数

    <a name="zh-cn_topic_0201534134_table242418284253"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534134_row155362282252"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534134_p65362028192517"><a name="zh-cn_topic_0201534134_p65362028192517"></a><a name="zh-cn_topic_0201534134_p65362028192517"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.48%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534134_p155361728192510"><a name="zh-cn_topic_0201534134_p155361728192510"></a><a name="zh-cn_topic_0201534134_p155361728192510"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="65.16999999999999%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534134_p1253616288258"><a name="zh-cn_topic_0201534134_p1253616288258"></a><a name="zh-cn_topic_0201534134_p1253616288258"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534134_row65365287254"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534134_p553612832513"><a name="zh-cn_topic_0201534134_p553612832513"></a><a name="zh-cn_topic_0201534134_p553612832513"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.48%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534134_p1453619282257"><a name="zh-cn_topic_0201534134_p1453619282257"></a><a name="zh-cn_topic_0201534134_p1453619282257"></a>Array of <a href="#zh-cn_topic_0201534134_table043062842515">tag</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="65.16999999999999%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534134_p155364285253"><a name="zh-cn_topic_0201534134_p155364285253"></a><a name="zh-cn_topic_0201534134_p155364285253"></a>tag对象列表，请参见<a href="#zh-cn_topic_0201534134_table043062842515">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag字段数据结构说明

    <a name="zh-cn_topic_0201534134_table043062842515"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_row16625112015"><th class="cellrowborder" valign="top" width="25.332533253325334%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p156216117208"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p156216117208"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p156216117208"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.332533253325334%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p8622172014"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p8622172014"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p8622172014"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.33493349334934%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p1262101182018"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p1262101182018"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p1262101182018"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_row166216192017"><td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p562013203"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p562013203"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p562013203"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p4621132014"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p4621132014"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p4621132014"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.33493349334934%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p3622162019"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p3622162019"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p3622162019"></a>键。</p>
    <a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_row862171152012"><td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p2062312201"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p2062312201"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p2062312201"></a>values</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.332533253325334%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p7282112319144"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p7282112319144"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p7282112319144"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.33493349334934%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p166210162014"><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p166210162014"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_p166210162014"></a>值列表。</p>
    <a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0201534134_zh-cn_topic_0201534104_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
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
                "values": [
                    "value1",
                    "value2"
                ]
            },
            {
                "key": "key2",
                "values": [
                    "value1",
                    "value2"
                ]
            }
        ]
    }
    ```


## 状态码<a name="zh-cn_topic_0201534134_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534134_section85821649202813"></a>

请参考[错误码](错误码.md)。

