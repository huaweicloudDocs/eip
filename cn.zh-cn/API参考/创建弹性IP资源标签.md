# 创建弹性IP资源标签<a name="eip_apitag_0001"></a>

## 功能介绍<a name="zh-cn_topic_0201534118_section2090011408236"></a>

给指定弹性IP资源实例增加标签信息。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”、“华南-广州”区域开放。

## URI<a name="zh-cn_topic_0201534118_section1690074011233"></a>

POST /v2.0/\{project\_id\}/publicips/\{publicip\_id\}/tags

参数说明请参见[表1](#zh-cn_topic_0201534118_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534118_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534118_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534118_p47174532"><a name="zh-cn_topic_0201534118_p47174532"></a><a name="zh-cn_topic_0201534118_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534118_p63040734"><a name="zh-cn_topic_0201534118_p63040734"></a><a name="zh-cn_topic_0201534118_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534118_p6025849"><a name="zh-cn_topic_0201534118_p6025849"></a><a name="zh-cn_topic_0201534118_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534118_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534118_p8478608"><a name="zh-cn_topic_0201534118_p8478608"></a><a name="zh-cn_topic_0201534118_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534118_p15678685"><a name="zh-cn_topic_0201534118_p15678685"></a><a name="zh-cn_topic_0201534118_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534118_p10487112"><a name="zh-cn_topic_0201534118_p10487112"></a><a name="zh-cn_topic_0201534118_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534118_row21254748"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534118_p43913021"><a name="zh-cn_topic_0201534118_p43913021"></a><a name="zh-cn_topic_0201534118_p43913021"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534118_p184914"><a name="zh-cn_topic_0201534118_p184914"></a><a name="zh-cn_topic_0201534118_p184914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534118_p14978051"><a name="zh-cn_topic_0201534118_p14978051"></a><a name="zh-cn_topic_0201534118_p14978051"></a>EIP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534118_section1990974032314"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534118_table9909164018236"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534118_row6974154010238"><th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534118_p89741140152312"><a name="zh-cn_topic_0201534118_p89741140152312"></a><a name="zh-cn_topic_0201534118_p89741140152312"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534118_p2974164013235"><a name="zh-cn_topic_0201534118_p2974164013235"></a><a name="zh-cn_topic_0201534118_p2974164013235"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.62%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534118_p997410409235"><a name="zh-cn_topic_0201534118_p997410409235"></a><a name="zh-cn_topic_0201534118_p997410409235"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.379999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534118_p13974144018230"><a name="zh-cn_topic_0201534118_p13974144018230"></a><a name="zh-cn_topic_0201534118_p13974144018230"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534118_row11974194022315"><td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534118_p16974134022320"><a name="zh-cn_topic_0201534118_p16974134022320"></a><a name="zh-cn_topic_0201534118_p16974134022320"></a>tag</p>
    </td>
    <td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534118_p49755402238"><a name="zh-cn_topic_0201534118_p49755402238"></a><a name="zh-cn_topic_0201534118_p49755402238"></a><a href="#zh-cn_topic_0201534118_table13242848193719">tag</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.62%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534118_p497516406238"><a name="zh-cn_topic_0201534118_p497516406238"></a><a name="zh-cn_topic_0201534118_p497516406238"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.379999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534118_p69751040202314"><a name="zh-cn_topic_0201534118_p69751040202314"></a><a name="zh-cn_topic_0201534118_p69751040202314"></a>tag对象， 请参见<a href="#zh-cn_topic_0201534118_table13242848193719">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tag对象

    <a name="zh-cn_topic_0201534118_table13242848193719"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534118_row13343144812379"><th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534118_p15343174853715"><a name="zh-cn_topic_0201534118_p15343174853715"></a><a name="zh-cn_topic_0201534118_p15343174853715"></a>属性</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.060000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534118_p13431648163716"><a name="zh-cn_topic_0201534118_p13431648163716"></a><a name="zh-cn_topic_0201534118_p13431648163716"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="12.24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534118_p169809965412"><a name="zh-cn_topic_0201534118_p169809965412"></a><a name="zh-cn_topic_0201534118_p169809965412"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.699999999999996%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534118_p11344748183719"><a name="zh-cn_topic_0201534118_p11344748183719"></a><a name="zh-cn_topic_0201534118_p11344748183719"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534118_row103449487379"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534118_p183469482373"><a name="zh-cn_topic_0201534118_p183469482373"></a><a name="zh-cn_topic_0201534118_p183469482373"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534118_p1434684863710"><a name="zh-cn_topic_0201534118_p1434684863710"></a><a name="zh-cn_topic_0201534118_p1434684863710"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534118_p298018911544"><a name="zh-cn_topic_0201534118_p298018911544"></a><a name="zh-cn_topic_0201534118_p298018911544"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><a name="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"></a><ul id="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul2321196023222"><li>标签名称</li><li>不能为空。</li><li>长度不超过36个字符。</li><li>由英文字母、数字、下划线、中划线、中文字符组成。</li><li>同一资源的key值不能重复。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534118_row2346548163714"><td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534118_p1134624816377"><a name="zh-cn_topic_0201534118_p1134624816377"></a><a name="zh-cn_topic_0201534118_p1134624816377"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.060000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534118_p234619483371"><a name="zh-cn_topic_0201534118_p234619483371"></a><a name="zh-cn_topic_0201534118_p234619483371"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="12.24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534118_p209805915417"><a name="zh-cn_topic_0201534118_p209805915417"></a><a name="zh-cn_topic_0201534118_p209805915417"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.699999999999996%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><a name="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"></a><ul id="zh-cn_topic_0201534118_zh-cn_topic_0013935842_zh-cn_topic_0067805752_zh-cn_topic_0013859511_ul6706750105539"><li>标签值</li><li>长度不超过43个字符。</li><li>由英文字母、数字、下划线、点、中划线、中文字符组成。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips/{publicip_id}/tags
    
    {
        "tag": {
            "key": "key1",
            "value": "value1"
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534118_section691614409232"></a>

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


## 状态码<a name="zh-cn_topic_0201534118_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534118_section85821649202813"></a>

请参考[错误码](错误码.md)。

