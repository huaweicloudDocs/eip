# 共享带宽插入弹性公网IP<a name="eip_apisharedbandwidth_0004"></a>

## 功能介绍<a name="zh-cn_topic_0201534131_section16581154"></a>

共享带宽插入弹性公网IP。

## URI<a name="zh-cn_topic_0201534131_section15012662"></a>

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/insert

参数说明请参见[表1](#zh-cn_topic_0201534131_table25281875)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534131_table25281875"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534131_row26712487"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534131_p16227847"><a name="zh-cn_topic_0201534131_p16227847"></a><a name="zh-cn_topic_0201534131_p16227847"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534131_p39387211"><a name="zh-cn_topic_0201534131_p39387211"></a><a name="zh-cn_topic_0201534131_p39387211"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534131_p36247516"><a name="zh-cn_topic_0201534131_p36247516"></a><a name="zh-cn_topic_0201534131_p36247516"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534131_row50367649"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p53247746"><a name="zh-cn_topic_0201534131_p53247746"></a><a name="zh-cn_topic_0201534131_p53247746"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p18100201"><a name="zh-cn_topic_0201534131_p18100201"></a><a name="zh-cn_topic_0201534131_p18100201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p10487112"><a name="zh-cn_topic_0201534131_p10487112"></a><a name="zh-cn_topic_0201534131_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534131_row41709209"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p23002745"><a name="zh-cn_topic_0201534131_p23002745"></a><a name="zh-cn_topic_0201534131_p23002745"></a>bandwidth_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p51283066"><a name="zh-cn_topic_0201534131_p51283066"></a><a name="zh-cn_topic_0201534131_p51283066"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p60287683"><a name="zh-cn_topic_0201534131_p60287683"></a><a name="zh-cn_topic_0201534131_p60287683"></a>带宽唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534131_section896237"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534131_table3057854815556"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row6286666315556"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534131_p5903494715556"><a name="zh-cn_topic_0201534131_p5903494715556"></a><a name="zh-cn_topic_0201534131_p5903494715556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534131_p1710139915556"><a name="zh-cn_topic_0201534131_p1710139915556"></a><a name="zh-cn_topic_0201534131_p1710139915556"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534131_p4303610815556"><a name="zh-cn_topic_0201534131_p4303610815556"></a><a name="zh-cn_topic_0201534131_p4303610815556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534131_p6337274615556"><a name="zh-cn_topic_0201534131_p6337274615556"></a><a name="zh-cn_topic_0201534131_p6337274615556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row3291877615556"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534131_p4917516615556"><a name="zh-cn_topic_0201534131_p4917516615556"></a><a name="zh-cn_topic_0201534131_p4917516615556"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534131_p2376550915556"><a name="zh-cn_topic_0201534131_p2376550915556"></a><a name="zh-cn_topic_0201534131_p2376550915556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534131_p4595806815556"><a name="zh-cn_topic_0201534131_p4595806815556"></a><a name="zh-cn_topic_0201534131_p4595806815556"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534131_p1610901815556"><a name="zh-cn_topic_0201534131_p1610901815556"></a><a name="zh-cn_topic_0201534131_p1610901815556"></a>带宽对象，请参见<a href="#zh-cn_topic_0201534131_table31854691">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  bandwidth字段说明

    <a name="zh-cn_topic_0201534131_table31854691"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row6882862"><th class="cellrowborder" valign="top" width="13.350000000000001%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534131_p20640979"><a name="zh-cn_topic_0201534131_p20640979"></a><a name="zh-cn_topic_0201534131_p20640979"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534131_p61306625"><a name="zh-cn_topic_0201534131_p61306625"></a><a name="zh-cn_topic_0201534131_p61306625"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534131_p5200653172316"><a name="zh-cn_topic_0201534131_p5200653172316"></a><a name="zh-cn_topic_0201534131_p5200653172316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.830000000000005%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534131_p66889567"><a name="zh-cn_topic_0201534131_p66889567"></a><a name="zh-cn_topic_0201534131_p66889567"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row49345813"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534131_p37587916"><a name="zh-cn_topic_0201534131_p37587916"></a><a name="zh-cn_topic_0201534131_p37587916"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534131_p24722347"><a name="zh-cn_topic_0201534131_p24722347"></a><a name="zh-cn_topic_0201534131_p24722347"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534131_p18599757172316"><a name="zh-cn_topic_0201534131_p18599757172316"></a><a name="zh-cn_topic_0201534131_p18599757172316"></a>Array of <a href="#zh-cn_topic_0201534131_table30936422">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534131_ul1057071610312"></a><a name="zh-cn_topic_0201534131_ul1057071610312"></a><ul id="zh-cn_topic_0201534131_ul1057071610312"><li>功能说明：要插入共享带宽的<span id="zh-cn_topic_0201534131_text18486162013414"><a name="zh-cn_topic_0201534131_text18486162013414"></a><a name="zh-cn_topic_0201534131_text18486162013414"></a></span><span id="zh-cn_topic_0201534131_text10486162017418"><a name="zh-cn_topic_0201534131_text10486162017418"></a><a name="zh-cn_topic_0201534131_text10486162017418"></a>弹性公网IP</span>信息，请参见<a href="#zh-cn_topic_0201534131_table30936422">表4</a>。</li><li>约束：WHOLE类型的带宽支持多个<span id="zh-cn_topic_0201534131_text171130245418"><a name="zh-cn_topic_0201534131_text171130245418"></a><a name="zh-cn_topic_0201534131_text171130245418"></a></span><span id="zh-cn_topic_0201534131_text1113102416418"><a name="zh-cn_topic_0201534131_text1113102416418"></a><a name="zh-cn_topic_0201534131_text1113102416418"></a>弹性公网IP</span>，跟租户的配额相关，默认一个共享带宽的配额为20。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  publicip\_info对象

    <a name="zh-cn_topic_0201534131_table30936422"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row17161430"><th class="cellrowborder" valign="top" width="14.29%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534131_p47898561"><a name="zh-cn_topic_0201534131_p47898561"></a><a name="zh-cn_topic_0201534131_p47898561"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.03%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534131_p169718416504"><a name="zh-cn_topic_0201534131_p169718416504"></a><a name="zh-cn_topic_0201534131_p169718416504"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.96%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534131_p2828296517154"><a name="zh-cn_topic_0201534131_p2828296517154"></a><a name="zh-cn_topic_0201534131_p2828296517154"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.72%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534131_p58761073"><a name="zh-cn_topic_0201534131_p58761073"></a><a name="zh-cn_topic_0201534131_p58761073"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row62026502"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534131_p58090788"><a name="zh-cn_topic_0201534131_p58090788"></a><a name="zh-cn_topic_0201534131_p58090788"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534131_p79716416504"><a name="zh-cn_topic_0201534131_p79716416504"></a><a name="zh-cn_topic_0201534131_p79716416504"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534131_p921881117154"><a name="zh-cn_topic_0201534131_p921881117154"></a><a name="zh-cn_topic_0201534131_p921881117154"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534131_p476380"><a name="zh-cn_topic_0201534131_p476380"></a><a name="zh-cn_topic_0201534131_p476380"></a>带宽对应的<span id="zh-cn_topic_0201534131_text164255151912"><a name="zh-cn_topic_0201534131_text164255151912"></a><a name="zh-cn_topic_0201534131_text164255151912"></a></span><span id="zh-cn_topic_0201534131_text134257151798"><a name="zh-cn_topic_0201534131_text134257151798"></a><a name="zh-cn_topic_0201534131_text134257151798"></a>弹性公网IP</span>的唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row144151444141"><td class="cellrowborder" valign="top" width="14.29%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534131_p490210492147"><a name="zh-cn_topic_0201534131_p490210492147"></a><a name="zh-cn_topic_0201534131_p490210492147"></a>publicip_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534131_p4902154913141"><a name="zh-cn_topic_0201534131_p4902154913141"></a><a name="zh-cn_topic_0201534131_p4902154913141"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534131_p9902149171411"><a name="zh-cn_topic_0201534131_p9902149171411"></a><a name="zh-cn_topic_0201534131_p9902149171411"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534131_ul14903154919144"></a><a name="zh-cn_topic_0201534131_ul14903154919144"></a><ul id="zh-cn_topic_0201534131_ul14903154919144"><li>功能说明：<span id="zh-cn_topic_0201534131_text137487231492"><a name="zh-cn_topic_0201534131_text137487231492"></a><a name="zh-cn_topic_0201534131_text137487231492"></a></span><span id="zh-cn_topic_0201534131_text7748162318915"><a name="zh-cn_topic_0201534131_text7748162318915"></a><a name="zh-cn_topic_0201534131_text7748162318915"></a>弹性公网IP</span>的类型</li><li>取值范围：<em id="zh-cn_topic_0201534131_i16850184017499"><a name="zh-cn_topic_0201534131_i16850184017499"></a><a name="zh-cn_topic_0201534131_i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534131_ul585004064911"></a><a name="zh-cn_topic_0201534131_ul585004064911"></a><ul id="zh-cn_topic_0201534131_ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp、5_dualStack</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534131_ul9738153015499"></a><a name="zh-cn_topic_0201534131_ul9738153015499"></a><ul id="zh-cn_topic_0201534131_ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li><li>若publicip_id为弹性公网IP的id，则该字段可自动忽略。若publicip_id为IPv6端口PORT的id，则该字段必填，为5_dualStack（本条约束适用于“华北-北京四”）</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{Endpoint}/v2.0/{project_id}/bandwidths/{bandwidth_id}/insert
    
    {
      "bandwidth": {
        "publicip_info": [
          {
            "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f",
            "publicip_type": "5_bgp"
          }
        ]
      }
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534131_section8066134"></a>

-   响应参数

    **表 5**  响应参数

    <a name="zh-cn_topic_0201534131_table58151089155516"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row25417629155516"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534131_p45562050155516"><a name="zh-cn_topic_0201534131_p45562050155516"></a><a name="zh-cn_topic_0201534131_p45562050155516"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534131_p29734214155516"><a name="zh-cn_topic_0201534131_p29734214155516"></a><a name="zh-cn_topic_0201534131_p29734214155516"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534131_p59661173155516"><a name="zh-cn_topic_0201534131_p59661173155516"></a><a name="zh-cn_topic_0201534131_p59661173155516"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row716877155516"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p58067061155516"><a name="zh-cn_topic_0201534131_p58067061155516"></a><a name="zh-cn_topic_0201534131_p58067061155516"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p967638155516"><a name="zh-cn_topic_0201534131_p967638155516"></a><a name="zh-cn_topic_0201534131_p967638155516"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p34319839155516"><a name="zh-cn_topic_0201534131_p34319839155516"></a><a name="zh-cn_topic_0201534131_p34319839155516"></a>带宽对象，请参见<a href="#zh-cn_topic_0201534131_table138718569112">表6</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  bandwidth字段说明

    <a name="zh-cn_topic_0201534131_table138718569112"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row128705614111"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534131_p787856121118"><a name="zh-cn_topic_0201534131_p787856121118"></a><a name="zh-cn_topic_0201534131_p787856121118"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534131_p2088556181119"><a name="zh-cn_topic_0201534131_p2088556181119"></a><a name="zh-cn_topic_0201534131_p2088556181119"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534131_p1888115661112"><a name="zh-cn_topic_0201534131_p1888115661112"></a><a name="zh-cn_topic_0201534131_p1888115661112"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row1688115611112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p78865651114"><a name="zh-cn_topic_0201534131_p78865651114"></a><a name="zh-cn_topic_0201534131_p78865651114"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p1588256131115"><a name="zh-cn_topic_0201534131_p1588256131115"></a><a name="zh-cn_topic_0201534131_p1588256131115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul181211824134816"></a><a name="zh-cn_topic_0201534131_ul181211824134816"></a><ul id="zh-cn_topic_0201534131_ul181211824134816"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row17881356171113"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p20882056151111"><a name="zh-cn_topic_0201534131_p20882056151111"></a><a name="zh-cn_topic_0201534131_p20882056151111"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p208855641111"><a name="zh-cn_topic_0201534131_p208855641111"></a><a name="zh-cn_topic_0201534131_p208855641111"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul19451840174816"></a><a name="zh-cn_topic_0201534131_ul19451840174816"></a><ul id="zh-cn_topic_0201534131_ul19451840174816"><li>功能说明：带宽大小。</li><li>取值范围：默认5Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row488105641111"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p10881056191119"><a name="zh-cn_topic_0201534131_p10881056191119"></a><a name="zh-cn_topic_0201534131_p10881056191119"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p88816566118"><a name="zh-cn_topic_0201534131_p88816566118"></a><a name="zh-cn_topic_0201534131_p88816566118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p48813561118"><a name="zh-cn_topic_0201534131_p48813561118"></a><a name="zh-cn_topic_0201534131_p48813561118"></a>带宽唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row158855661120"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p17881856151120"><a name="zh-cn_topic_0201534131_p17881856151120"></a><a name="zh-cn_topic_0201534131_p17881856151120"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p18887564112"><a name="zh-cn_topic_0201534131_p18887564112"></a><a name="zh-cn_topic_0201534131_p18887564112"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul4262181884915"></a><a name="zh-cn_topic_0201534131_ul4262181884915"></a><ul id="zh-cn_topic_0201534131_ul4262181884915"><li>功能说明：带宽类型，标识是否是共享带宽</li><li>取值范围：WHOLE，PER<a name="zh-cn_topic_0201534131_ul313253512484"></a><a name="zh-cn_topic_0201534131_ul313253512484"></a><ul id="zh-cn_topic_0201534131_ul313253512484"><li>WHOLE表示共享带宽</li><li>PER表示独享带宽</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row1089195616112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p88910565118"><a name="zh-cn_topic_0201534131_p88910565118"></a><a name="zh-cn_topic_0201534131_p88910565118"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p289456141114"><a name="zh-cn_topic_0201534131_p289456141114"></a><a name="zh-cn_topic_0201534131_p289456141114"></a>Array of <a href="#zh-cn_topic_0201534131_table51281965">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul14114132894913"></a><a name="zh-cn_topic_0201534131_ul14114132894913"></a><ul id="zh-cn_topic_0201534131_ul14114132894913"><li>功能说明：带宽对应的<span id="zh-cn_topic_0201534131_text887935017917"><a name="zh-cn_topic_0201534131_text887935017917"></a><a name="zh-cn_topic_0201534131_text887935017917"></a></span><span id="zh-cn_topic_0201534131_text15879165018910"><a name="zh-cn_topic_0201534131_text15879165018910"></a><a name="zh-cn_topic_0201534131_text15879165018910"></a>弹性公网IP</span>信息，请参见<a href="#zh-cn_topic_0201534131_table51281965">表7</a>。</li><li>约束：WHOLE类型的带宽支持多个<span id="zh-cn_topic_0201534131_text32328541996"><a name="zh-cn_topic_0201534131_text32328541996"></a><a name="zh-cn_topic_0201534131_text32328541996"></a></span><span id="zh-cn_topic_0201534131_text192322545913"><a name="zh-cn_topic_0201534131_text192322545913"></a><a name="zh-cn_topic_0201534131_text192322545913"></a>弹性公网IP</span>，PER类型的带宽只能对应一个<span id="zh-cn_topic_0201534131_text16769165812914"><a name="zh-cn_topic_0201534131_text16769165812914"></a><a name="zh-cn_topic_0201534131_text16769165812914"></a></span><span id="zh-cn_topic_0201534131_text77698581994"><a name="zh-cn_topic_0201534131_text77698581994"></a><a name="zh-cn_topic_0201534131_text77698581994"></a>弹性公网IP</span></li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row1489156171117"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p489456141120"><a name="zh-cn_topic_0201534131_p489456141120"></a><a name="zh-cn_topic_0201534131_p489456141120"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p19891756141115"><a name="zh-cn_topic_0201534131_p19891756141115"></a><a name="zh-cn_topic_0201534131_p19891756141115"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p19517617121017"><a name="zh-cn_topic_0201534131_p19517617121017"></a><a name="zh-cn_topic_0201534131_p19517617121017"></a>项目ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row1089056121112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p1989105620112"><a name="zh-cn_topic_0201534131_p1989105620112"></a><a name="zh-cn_topic_0201534131_p1989105620112"></a>bandwidth_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p158995611110"><a name="zh-cn_topic_0201534131_p158995611110"></a><a name="zh-cn_topic_0201534131_p158995611110"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul5731955125012"></a><a name="zh-cn_topic_0201534131_ul5731955125012"></a><ul id="zh-cn_topic_0201534131_ul5731955125012"><li>功能说明：带宽类型，共享带宽默认为share。</li><li>取值范围：share，bgp，telcom，sbgp等<a name="zh-cn_topic_0201534131_ul1933102125013"></a><a name="zh-cn_topic_0201534131_ul1933102125013"></a><ul id="zh-cn_topic_0201534131_ul1933102125013"><li>share：共享带宽</li><li>bgp：动态bgp</li><li>telcom ：联通</li><li>sbgp：静态bgp</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row198331314193917"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p3181725102112"><a name="zh-cn_topic_0201534131_p3181725102112"></a><a name="zh-cn_topic_0201534131_p3181725102112"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p418192514212"><a name="zh-cn_topic_0201534131_p418192514212"></a><a name="zh-cn_topic_0201534131_p418192514212"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul101811251216"></a><a name="zh-cn_topic_0201534131_ul101811251216"></a><ul id="zh-cn_topic_0201534131_ul101811251216"><li>功能说明：按流量计费，按带宽计费还是按增强型95计费</li><li>取值范围：bandwidth（按带宽计费），traffic（按流量计费），95peak_plus（按增强型95计费），不返回或者为空时表示是bandwidth</li><li>约束：只有共享带宽支持95peak_plus（按增强型95计费），按增强型95计费时需要指定保底百分比，默认是20%</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row590556151112"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p99015567111"><a name="zh-cn_topic_0201534131_p99015567111"></a><a name="zh-cn_topic_0201534131_p99015567111"></a>billing_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p1890115614111"><a name="zh-cn_topic_0201534131_p1890115614111"></a><a name="zh-cn_topic_0201534131_p1890115614111"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p1190145612112"><a name="zh-cn_topic_0201534131_p1190145612112"></a><a name="zh-cn_topic_0201534131_p1190145612112"></a>账单信息。</p>
    <p id="zh-cn_topic_0201534131_p414131417317"><a name="zh-cn_topic_0201534131_p414131417317"></a><a name="zh-cn_topic_0201534131_p414131417317"></a>如果billing_info不为空，说明是包周期的带宽。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row457893134810"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p36136296490"><a name="zh-cn_topic_0201534131_p36136296490"></a><a name="zh-cn_topic_0201534131_p36136296490"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p561632984912"><a name="zh-cn_topic_0201534131_p561632984912"></a><a name="zh-cn_topic_0201534131_p561632984912"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul137091434125111"></a><a name="zh-cn_topic_0201534131_ul137091434125111"></a><ul id="zh-cn_topic_0201534131_ul137091434125111"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。创建共享带宽时，给共享带宽绑定企业项目ID。</li></ul>
    <div class="note" id="zh-cn_topic_0201534131_note13203107131712"><a name="zh-cn_topic_0201534131_note13203107131712"></a><a name="zh-cn_topic_0201534131_note13203107131712"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201534131_p1915862704914"><a name="zh-cn_topic_0201534131_p1915862704914"></a><a name="zh-cn_topic_0201534131_p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row9477203041814"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p16479330181816"><a name="zh-cn_topic_0201534131_p16479330181816"></a><a name="zh-cn_topic_0201534131_p16479330181816"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p5479163011185"><a name="zh-cn_topic_0201534131_p5479163011185"></a><a name="zh-cn_topic_0201534131_p5479163011185"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul114381249113115"></a><a name="zh-cn_topic_0201534131_ul114381249113115"></a><ul id="zh-cn_topic_0201534131_ul114381249113115"><li>功能说明：带宽的状态</li><li>取值范围：<a name="zh-cn_topic_0201534131_ul1943874963116"></a><a name="zh-cn_topic_0201534131_ul1943874963116"></a><ul id="zh-cn_topic_0201534131_ul1943874963116"><li>FREEZED：冻结</li><li>NORMAL：正常</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 7**  publicip\_info对象

    <a name="zh-cn_topic_0201534131_table51281965"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534131_row26928941"><th class="cellrowborder" valign="top" width="26.71%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534131_p33760584"><a name="zh-cn_topic_0201534131_p33760584"></a><a name="zh-cn_topic_0201534131_p33760584"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.6%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534131_p37114580172552"><a name="zh-cn_topic_0201534131_p37114580172552"></a><a name="zh-cn_topic_0201534131_p37114580172552"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.69%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534131_p43944024"><a name="zh-cn_topic_0201534131_p43944024"></a><a name="zh-cn_topic_0201534131_p43944024"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534131_row2696221"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p17067371"><a name="zh-cn_topic_0201534131_p17067371"></a><a name="zh-cn_topic_0201534131_p17067371"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p53490986172552"><a name="zh-cn_topic_0201534131_p53490986172552"></a><a name="zh-cn_topic_0201534131_p53490986172552"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p3792141220526"><a name="zh-cn_topic_0201534131_p3792141220526"></a><a name="zh-cn_topic_0201534131_p3792141220526"></a>功能说明：带宽对应的<span id="zh-cn_topic_0201534131_text13342844101013"><a name="zh-cn_topic_0201534131_text13342844101013"></a><a name="zh-cn_topic_0201534131_text13342844101013"></a></span><span id="zh-cn_topic_0201534131_text334254410106"><a name="zh-cn_topic_0201534131_text334254410106"></a><a name="zh-cn_topic_0201534131_text334254410106"></a>弹性公网IP</span>的唯一标识或IPv6端口的唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row963478"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p621304517467"><a name="zh-cn_topic_0201534131_p621304517467"></a><a name="zh-cn_topic_0201534131_p621304517467"></a>publicip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p1021574544615"><a name="zh-cn_topic_0201534131_p1021574544615"></a><a name="zh-cn_topic_0201534131_p1021574544615"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p198309316175"><a name="zh-cn_topic_0201534131_p198309316175"></a><a name="zh-cn_topic_0201534131_p198309316175"></a>功能说明：IPv4时是申请到的<span id="zh-cn_topic_0201534131_text9101248121015"><a name="zh-cn_topic_0201534131_text9101248121015"></a><a name="zh-cn_topic_0201534131_text9101248121015"></a></span><span id="zh-cn_topic_0201534131_text1110134811107"><a name="zh-cn_topic_0201534131_text1110134811107"></a><a name="zh-cn_topic_0201534131_text1110134811107"></a>弹性公网IP</span>地址，IPv6时为IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row049765515547"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p1270211337315"><a name="zh-cn_topic_0201534131_p1270211337315"></a><a name="zh-cn_topic_0201534131_p1270211337315"></a>publicipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p570212339313"><a name="zh-cn_topic_0201534131_p570212339313"></a><a name="zh-cn_topic_0201534131_p570212339313"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534131_p383015318171"><a name="zh-cn_topic_0201534131_p383015318171"></a><a name="zh-cn_topic_0201534131_p383015318171"></a>功能说明：IPv4时无此字段，IPv6时为申请到的<span id="zh-cn_topic_0201534131_text3783205121018"><a name="zh-cn_topic_0201534131_text3783205121018"></a><a name="zh-cn_topic_0201534131_text3783205121018"></a></span><span id="zh-cn_topic_0201534131_text97838519103"><a name="zh-cn_topic_0201534131_text97838519103"></a><a name="zh-cn_topic_0201534131_text97838519103"></a>弹性公网IP</span>地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row11195191125518"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p197308575327"><a name="zh-cn_topic_0201534131_p197308575327"></a><a name="zh-cn_topic_0201534131_p197308575327"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p11730115718326"><a name="zh-cn_topic_0201534131_p11730115718326"></a><a name="zh-cn_topic_0201534131_p11730115718326"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul4257145935817"></a><a name="zh-cn_topic_0201534131_ul4257145935817"></a><ul id="zh-cn_topic_0201534131_ul4257145935817"><li>功能说明：IP版本信息</li><li>取值范围：<a name="zh-cn_topic_0201534131_ul208241936115914"></a><a name="zh-cn_topic_0201534131_ul208241936115914"></a><ul id="zh-cn_topic_0201534131_ul208241936115914"><li>4：IPv4</li><li>6：IPv6</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534131_row32534423"><td class="cellrowborder" valign="top" width="26.71%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534131_p18042568"><a name="zh-cn_topic_0201534131_p18042568"></a><a name="zh-cn_topic_0201534131_p18042568"></a>publicip_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534131_p42115453172552"><a name="zh-cn_topic_0201534131_p42115453172552"></a><a name="zh-cn_topic_0201534131_p42115453172552"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.69%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534131_ul13831731151713"></a><a name="zh-cn_topic_0201534131_ul13831731151713"></a><ul id="zh-cn_topic_0201534131_ul13831731151713"><li>功能说明：<span id="zh-cn_topic_0201534131_text1658195610102"><a name="zh-cn_topic_0201534131_text1658195610102"></a><a name="zh-cn_topic_0201534131_text1658195610102"></a></span><span id="zh-cn_topic_0201534131_text1358135661016"><a name="zh-cn_topic_0201534131_text1358135661016"></a><a name="zh-cn_topic_0201534131_text1358135661016"></a>弹性公网IP</span>的类型</li><li>取值范围：5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）<a name="zh-cn_topic_0201534131_ul161028178419"></a><a name="zh-cn_topic_0201534131_ul161028178419"></a><ul id="zh-cn_topic_0201534131_ul161028178419"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：必须是系统具体支持的类型</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "bandwidth": {
            "id": "3fa5b383-5a73-4dcb-a314-c6128546d855",
            "name": "bandwidth123",
            "size": 10,
            "share_type": "WHOLE",
            "publicip_info": [
                {
                     "publicip_id": "d91b0028-6f6b-4478-808a-297b75b6812a", 
                     "publicip_address": "::ffff:192.168.89.9", 
                     "publicip_type": "5_dualStack",
                     "ip_version": 6
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f",
                    "publicip_address": "99.xx.xx.82",
                    "publicip_type": "5_bgp",
                    "ip_version": 4
                }
            ],
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "charge_mode": "traffic",
            "bandwidth_type": "share",
            "billing_info": "CS1712121146TSQOJ:0616e2a5dc9f4985ba52ea8c0c7e273c:southchina:35f2b308f5d64441a6fa7999fbcd4321"
        }
    }
    ```


## 状态码<a name="zh-cn_topic_0201534131_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534131_section85821649202813"></a>

请参考[错误码](错误码.md)。

