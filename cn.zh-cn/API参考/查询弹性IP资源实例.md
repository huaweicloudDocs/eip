# 查询弹性IP资源实例<a name="eip_apitag_0005"></a>

## 功能介绍<a name="zh-cn_topic_0201534190_section1962411310253"></a>

使用标签过滤实例。

该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”、“华南-广州”区域开放。

## URI<a name="zh-cn_topic_0201534190_section11624171382513"></a>

POST /v2.0/\{project\_id\}/publicips/resource\_instances/action

参数说明请参见[表1](#zh-cn_topic_0201534190_table27380479)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534190_table27380479"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534190_row28751554"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534190_p47174532"><a name="zh-cn_topic_0201534190_p47174532"></a><a name="zh-cn_topic_0201534190_p47174532"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534190_p63040734"><a name="zh-cn_topic_0201534190_p63040734"></a><a name="zh-cn_topic_0201534190_p63040734"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534190_p6025849"><a name="zh-cn_topic_0201534190_p6025849"></a><a name="zh-cn_topic_0201534190_p6025849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534190_row18331773"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p8478608"><a name="zh-cn_topic_0201534190_p8478608"></a><a name="zh-cn_topic_0201534190_p8478608"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p15678685"><a name="zh-cn_topic_0201534190_p15678685"></a><a name="zh-cn_topic_0201534190_p15678685"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p10487112"><a name="zh-cn_topic_0201534190_p10487112"></a><a name="zh-cn_topic_0201534190_p10487112"></a>项目ID，请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534190_section9629111372520"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534190_table6653101362518"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row10890201372517"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534190_p178901213172513"><a name="zh-cn_topic_0201534190_p178901213172513"></a><a name="zh-cn_topic_0201534190_p178901213172513"></a>参数名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534190_p38902139259"><a name="zh-cn_topic_0201534190_p38902139259"></a><a name="zh-cn_topic_0201534190_p38902139259"></a>类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534190_p5890151372511"><a name="zh-cn_topic_0201534190_p5890151372511"></a><a name="zh-cn_topic_0201534190_p5890151372511"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.42574257425742%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534190_p3890181342518"><a name="zh-cn_topic_0201534190_p3890181342518"></a><a name="zh-cn_topic_0201534190_p3890181342518"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row11890161322518"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p10890111318251"><a name="zh-cn_topic_0201534190_p10890111318251"></a><a name="zh-cn_topic_0201534190_p10890111318251"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p1239241812243"><a name="zh-cn_topic_0201534190_p1239241812243"></a><a name="zh-cn_topic_0201534190_p1239241812243"></a>Array of <a href="#zh-cn_topic_0201534190_table16632111318253">tags</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p1889041312253"><a name="zh-cn_topic_0201534190_p1889041312253"></a><a name="zh-cn_topic_0201534190_p1889041312253"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p48900130251"><a name="zh-cn_topic_0201534190_p48900130251"></a><a name="zh-cn_topic_0201534190_p48900130251"></a>包含标签，最多包含10个key，每个key下面的value最多10个，结构体不能缺失，key不能为空或者空字符串。Key不能重复，同一个key中values不能重复。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row1389091382511"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p389021352513"><a name="zh-cn_topic_0201534190_p389021352513"></a><a name="zh-cn_topic_0201534190_p389021352513"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p168901813172511"><a name="zh-cn_topic_0201534190_p168901813172511"></a><a name="zh-cn_topic_0201534190_p168901813172511"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p168906139251"><a name="zh-cn_topic_0201534190_p168906139251"></a><a name="zh-cn_topic_0201534190_p168906139251"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p1589091312258"><a name="zh-cn_topic_0201534190_p1589091312258"></a><a name="zh-cn_topic_0201534190_p1589091312258"></a>查询记录数（action为count时无此参数）如果action为filter默认为1000，limit最多为1000，不能为负数，最小值为1</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row5890313172513"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p138901013132519"><a name="zh-cn_topic_0201534190_p138901013132519"></a><a name="zh-cn_topic_0201534190_p138901013132519"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p1889020133259"><a name="zh-cn_topic_0201534190_p1889020133259"></a><a name="zh-cn_topic_0201534190_p1889020133259"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p12890131372510"><a name="zh-cn_topic_0201534190_p12890131372510"></a><a name="zh-cn_topic_0201534190_p12890131372510"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p18901613132519"><a name="zh-cn_topic_0201534190_p18901613132519"></a><a name="zh-cn_topic_0201534190_p18901613132519"></a>（索引位置）， 从offset指定的下一条数据开始查询。 查询第一页数据时，不需要传入此参数，查询后续页码数据时，将查询前一页数据时响应体中的值带入此参数（action为count时无此参数）如果action为filter默认为0，必须为数字，不能为负数</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row19890191382520"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p2891161314258"><a name="zh-cn_topic_0201534190_p2891161314258"></a><a name="zh-cn_topic_0201534190_p2891161314258"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p14891161312512"><a name="zh-cn_topic_0201534190_p14891161312512"></a><a name="zh-cn_topic_0201534190_p14891161312512"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p1389115138251"><a name="zh-cn_topic_0201534190_p1389115138251"></a><a name="zh-cn_topic_0201534190_p1389115138251"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p10891413192514"><a name="zh-cn_topic_0201534190_p10891413192514"></a><a name="zh-cn_topic_0201534190_p10891413192514"></a>操作标识（仅限于filter，count）：filter（过滤），count(查询总条数)</p>
    <p id="zh-cn_topic_0201534190_p1889191322516"><a name="zh-cn_topic_0201534190_p1889191322516"></a><a name="zh-cn_topic_0201534190_p1889191322516"></a>如果是filter就是分页查询，如果是count只需按照条件将总条数返回即可。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row118911113102515"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p208913138258"><a name="zh-cn_topic_0201534190_p208913138258"></a><a name="zh-cn_topic_0201534190_p208913138258"></a>matches</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p163372262315"><a name="zh-cn_topic_0201534190_p163372262315"></a><a name="zh-cn_topic_0201534190_p163372262315"></a>Array of <a href="#zh-cn_topic_0201534190_table18642101315254">match</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p6891111312256"><a name="zh-cn_topic_0201534190_p6891111312256"></a><a name="zh-cn_topic_0201534190_p6891111312256"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42574257425742%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p18891613102512"><a name="zh-cn_topic_0201534190_p18891613102512"></a><a name="zh-cn_topic_0201534190_p18891613102512"></a>搜索字段，key为要匹配的字段，当前仅支持resource_name。value为匹配的值。此字段为固定字典值。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  tags字段数据结构说明

    <a name="zh-cn_topic_0201534190_table16632111318253"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row1789113139250"><th class="cellrowborder" valign="top" width="31.626837316268368%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534190_p78915138256"><a name="zh-cn_topic_0201534190_p78915138256"></a><a name="zh-cn_topic_0201534190_p78915138256"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534190_p158911913112510"><a name="zh-cn_topic_0201534190_p158911913112510"></a><a name="zh-cn_topic_0201534190_p158911913112510"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534190_p0891613152515"><a name="zh-cn_topic_0201534190_p0891613152515"></a><a name="zh-cn_topic_0201534190_p0891613152515"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.7960203979602%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534190_p1489151317257"><a name="zh-cn_topic_0201534190_p1489151317257"></a><a name="zh-cn_topic_0201534190_p1489151317257"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row17891131332517"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p0891151372514"><a name="zh-cn_topic_0201534190_p0891151372514"></a><a name="zh-cn_topic_0201534190_p0891151372514"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p6891181362517"><a name="zh-cn_topic_0201534190_p6891181362517"></a><a name="zh-cn_topic_0201534190_p6891181362517"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p11891121320254"><a name="zh-cn_topic_0201534190_p11891121320254"></a><a name="zh-cn_topic_0201534190_p11891121320254"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p2891131311252"><a name="zh-cn_topic_0201534190_p2891131311252"></a><a name="zh-cn_topic_0201534190_p2891131311252"></a>键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row08913131253"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p9891171316250"><a name="zh-cn_topic_0201534190_p9891171316250"></a><a name="zh-cn_topic_0201534190_p9891171316250"></a>values</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p2891191311251"><a name="zh-cn_topic_0201534190_p2891191311251"></a><a name="zh-cn_topic_0201534190_p2891191311251"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p1289191392518"><a name="zh-cn_topic_0201534190_p1289191392518"></a><a name="zh-cn_topic_0201534190_p1289191392518"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p108915133258"><a name="zh-cn_topic_0201534190_p108915133258"></a><a name="zh-cn_topic_0201534190_p108915133258"></a>值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  match字段数据结构说明

    <a name="zh-cn_topic_0201534190_table18642101315254"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row7891101302515"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534190_p689117135251"><a name="zh-cn_topic_0201534190_p689117135251"></a><a name="zh-cn_topic_0201534190_p689117135251"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.13131313131313%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534190_p188911413192519"><a name="zh-cn_topic_0201534190_p188911413192519"></a><a name="zh-cn_topic_0201534190_p188911413192519"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.14141414141414%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534190_p5891121362511"><a name="zh-cn_topic_0201534190_p5891121362511"></a><a name="zh-cn_topic_0201534190_p5891121362511"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534190_p1089371313256"><a name="zh-cn_topic_0201534190_p1089371313256"></a><a name="zh-cn_topic_0201534190_p1089371313256"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row58931413202516"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p989314135254"><a name="zh-cn_topic_0201534190_p989314135254"></a><a name="zh-cn_topic_0201534190_p989314135254"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.13131313131313%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p1789319133253"><a name="zh-cn_topic_0201534190_p1789319133253"></a><a name="zh-cn_topic_0201534190_p1789319133253"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p1889320134251"><a name="zh-cn_topic_0201534190_p1889320134251"></a><a name="zh-cn_topic_0201534190_p1889320134251"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p188931913182514"><a name="zh-cn_topic_0201534190_p188931913182514"></a><a name="zh-cn_topic_0201534190_p188931913182514"></a>键。当前仅限定为resource_name</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row108933135254"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p7893201310254"><a name="zh-cn_topic_0201534190_p7893201310254"></a><a name="zh-cn_topic_0201534190_p7893201310254"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.13131313131313%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p15893113102518"><a name="zh-cn_topic_0201534190_p15893113102518"></a><a name="zh-cn_topic_0201534190_p15893113102518"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.14141414141414%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p15893161332520"><a name="zh-cn_topic_0201534190_p15893161332520"></a><a name="zh-cn_topic_0201534190_p15893161332520"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p3893181332515"><a name="zh-cn_topic_0201534190_p3893181332515"></a><a name="zh-cn_topic_0201534190_p3893181332515"></a>值。每个值最大长度255个unicode字符。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例1：action为filter

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips/resource_instances/action
    
    {
        "offset": "0",
        "limit": "100",
        "action": "filter",
        "matches": [
            {
                "key": "resource_name",
                "value": "resource1"
            }
        ],
        "tags": [
            {
                "key": "key1",
                "values": [
                    "*value1",
                    "value2"
                ]
            }
        ]
    }
    ```

-   请求样例2：action为count

    ```
    {
        "action": "count",
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
        ],
        "matches": [
            {
                "key": "resource_name",
                "value": "resource1"
            }
        ]
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534190_section3676613112519"></a>

-   响应参数

    **表 5**  响应参数

    <a name="zh-cn_topic_0201534190_table669961372515"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row689311382512"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534190_p11893151312516"><a name="zh-cn_topic_0201534190_p11893151312516"></a><a name="zh-cn_topic_0201534190_p11893151312516"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.330000000000005%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534190_p1789361319251"><a name="zh-cn_topic_0201534190_p1789361319251"></a><a name="zh-cn_topic_0201534190_p1789361319251"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="34.67%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534190_p19893131310258"><a name="zh-cn_topic_0201534190_p19893131310258"></a><a name="zh-cn_topic_0201534190_p19893131310258"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row7893201315255"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p889311310255"><a name="zh-cn_topic_0201534190_p889311310255"></a><a name="zh-cn_topic_0201534190_p889311310255"></a>resources</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p658617115246"><a name="zh-cn_topic_0201534190_p658617115246"></a><a name="zh-cn_topic_0201534190_p658617115246"></a>Array of <a href="#zh-cn_topic_0201534190_table15678313132518">resource</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p1893111313258"><a name="zh-cn_topic_0201534190_p1893111313258"></a><a name="zh-cn_topic_0201534190_p1893111313258"></a>resource对象列表，请参见<a href="#zh-cn_topic_0201534190_table15678313132518">表6</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row1989331314259"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p158931313152513"><a name="zh-cn_topic_0201534190_p158931313152513"></a><a name="zh-cn_topic_0201534190_p158931313152513"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p58931113112511"><a name="zh-cn_topic_0201534190_p58931113112511"></a><a name="zh-cn_topic_0201534190_p58931113112511"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p10893121312258"><a name="zh-cn_topic_0201534190_p10893121312258"></a><a name="zh-cn_topic_0201534190_p10893121312258"></a>总记录数</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  resource对象

    <a name="zh-cn_topic_0201534190_table15678313132518"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row14893181314253"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534190_p1889361320250"><a name="zh-cn_topic_0201534190_p1889361320250"></a><a name="zh-cn_topic_0201534190_p1889361320250"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="37.330000000000005%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534190_p8893161342512"><a name="zh-cn_topic_0201534190_p8893161342512"></a><a name="zh-cn_topic_0201534190_p8893161342512"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="34.67%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534190_p3894151362514"><a name="zh-cn_topic_0201534190_p3894151362514"></a><a name="zh-cn_topic_0201534190_p3894151362514"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row389421332512"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p1289461362516"><a name="zh-cn_topic_0201534190_p1289461362516"></a><a name="zh-cn_topic_0201534190_p1289461362516"></a>resource_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p13894111322519"><a name="zh-cn_topic_0201534190_p13894111322519"></a><a name="zh-cn_topic_0201534190_p13894111322519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p589451313259"><a name="zh-cn_topic_0201534190_p589451313259"></a><a name="zh-cn_topic_0201534190_p589451313259"></a>资源ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row12894213172511"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p11894181312514"><a name="zh-cn_topic_0201534190_p11894181312514"></a><a name="zh-cn_topic_0201534190_p11894181312514"></a>resouce_detail</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p6894121314259"><a name="zh-cn_topic_0201534190_p6894121314259"></a><a name="zh-cn_topic_0201534190_p6894121314259"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p14894181315254"><a name="zh-cn_topic_0201534190_p14894181315254"></a><a name="zh-cn_topic_0201534190_p14894181315254"></a>资源详情。 资源对象，用于扩展。默认为空</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row1189431342514"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p58945135256"><a name="zh-cn_topic_0201534190_p58945135256"></a><a name="zh-cn_topic_0201534190_p58945135256"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p752144512478"><a name="zh-cn_topic_0201534190_p752144512478"></a><a name="zh-cn_topic_0201534190_p752144512478"></a>Array of <a href="#zh-cn_topic_0201534190_table1548032316199">tags</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p188941913122519"><a name="zh-cn_topic_0201534190_p188941913122519"></a><a name="zh-cn_topic_0201534190_p188941913122519"></a>标签列表，没有标签默认为空数组，参见<a href="#zh-cn_topic_0201534190_table1548032316199">表7</a></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row889451315256"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534190_p188943136256"><a name="zh-cn_topic_0201534190_p188943136256"></a><a name="zh-cn_topic_0201534190_p188943136256"></a>resource_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.330000000000005%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534190_p2894191372516"><a name="zh-cn_topic_0201534190_p2894191372516"></a><a name="zh-cn_topic_0201534190_p2894191372516"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="34.67%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534190_p3894141342514"><a name="zh-cn_topic_0201534190_p3894141342514"></a><a name="zh-cn_topic_0201534190_p3894141342514"></a>资源名称，没有默认为空字符串</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 7**  tags字段数据结构说明

    <a name="zh-cn_topic_0201534190_table1548032316199"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534190_row1785310237196"><th class="cellrowborder" valign="top" width="31.626837316268368%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534190_p185312312192"><a name="zh-cn_topic_0201534190_p185312312192"></a><a name="zh-cn_topic_0201534190_p185312312192"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534190_p208531923101913"><a name="zh-cn_topic_0201534190_p208531923101913"></a><a name="zh-cn_topic_0201534190_p208531923101913"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534190_p685312311196"><a name="zh-cn_topic_0201534190_p685312311196"></a><a name="zh-cn_topic_0201534190_p685312311196"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="39.7960203979602%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534190_p4853122311199"><a name="zh-cn_topic_0201534190_p4853122311199"></a><a name="zh-cn_topic_0201534190_p4853122311199"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534190_row08532238197"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p16854122312191"><a name="zh-cn_topic_0201534190_p16854122312191"></a><a name="zh-cn_topic_0201534190_p16854122312191"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p10854102317195"><a name="zh-cn_topic_0201534190_p10854102317195"></a><a name="zh-cn_topic_0201534190_p10854102317195"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p5854122371919"><a name="zh-cn_topic_0201534190_p5854122371919"></a><a name="zh-cn_topic_0201534190_p5854122371919"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p085432316193"><a name="zh-cn_topic_0201534190_p085432316193"></a><a name="zh-cn_topic_0201534190_p085432316193"></a>键。最大长度127个unicode字符。 key不能为空。(搜索时不对此参数做校验)</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534190_row15854623141911"><td class="cellrowborder" valign="top" width="31.626837316268368%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534190_p68541223141919"><a name="zh-cn_topic_0201534190_p68541223141919"></a><a name="zh-cn_topic_0201534190_p68541223141919"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534190_p17854223161918"><a name="zh-cn_topic_0201534190_p17854223161918"></a><a name="zh-cn_topic_0201534190_p17854223161918"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534190_p188541423181914"><a name="zh-cn_topic_0201534190_p188541423181914"></a><a name="zh-cn_topic_0201534190_p188541423181914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="39.7960203979602%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534190_p198541623121914"><a name="zh-cn_topic_0201534190_p198541623121914"></a><a name="zh-cn_topic_0201534190_p198541623121914"></a>值列表。每个值最大长度255个unicode字符，如果values为空列表，则表示any_value。value之间为或的关系。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例1：action为filte

    ```
    { 
          "resources": [
             {
                "resource_detail": null, 
                "resource_id": "cdfs_cefs_wesas_12_dsad", 
                "resource_name": "resouece1", 
                "tags": [
                    {
                       "key": "key1"，
                       "value": "value1"
                    },
                    {
                       "key": "key2"，
                       "value": "value1"
                    }
                 ]
             }
           ], 
          "total_count": 1000
    }
    ```

-   响应样例2：action为count

    ```
    {
           "total_count": 1000
    }
    ```


## 状态码<a name="zh-cn_topic_0201534190_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534190_section85821649202813"></a>

请参考[错误码](错误码.md)。

