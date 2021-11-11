# 查询弹性公网IP<a name="eip_api_0002"></a>

## 功能介绍<a name="zh-cn_topic_0201534285_section40040492"></a>

查询指定弹性公网IP。

## 调试<a name="zh-cn_topic_0201534285_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&version=v2&api=ShowPublicip)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0201534285_section24820109"></a>

GET /v1/\{project\_id\}/publicips/\{publicip\_id\}

参数说明请参见[表1](#zh-cn_topic_0201534285_table57982344)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534285_table57982344"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534285_row19130757"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534285_p6087504"><a name="zh-cn_topic_0201534285_p6087504"></a><a name="zh-cn_topic_0201534285_p6087504"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534285_p23325828"><a name="zh-cn_topic_0201534285_p23325828"></a><a name="zh-cn_topic_0201534285_p23325828"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534285_p10343879"><a name="zh-cn_topic_0201534285_p10343879"></a><a name="zh-cn_topic_0201534285_p10343879"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534285_row32547908"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p19134881"><a name="zh-cn_topic_0201534285_p19134881"></a><a name="zh-cn_topic_0201534285_p19134881"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p6421510"><a name="zh-cn_topic_0201534285_p6421510"></a><a name="zh-cn_topic_0201534285_p6421510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p10487112"><a name="zh-cn_topic_0201534285_p10487112"></a><a name="zh-cn_topic_0201534285_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534285_row50769665"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p18702178"><a name="zh-cn_topic_0201534285_p18702178"></a><a name="zh-cn_topic_0201534285_p18702178"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p38481481"><a name="zh-cn_topic_0201534285_p38481481"></a><a name="zh-cn_topic_0201534285_p38481481"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p29992219"><a name="zh-cn_topic_0201534285_p29992219"></a><a name="zh-cn_topic_0201534285_p29992219"></a><span id="zh-cn_topic_0201534285_text38025321986"><a name="zh-cn_topic_0201534285_text38025321986"></a><a name="zh-cn_topic_0201534285_text38025321986"></a></span><span id="zh-cn_topic_0201534285_text18021328811"><a name="zh-cn_topic_0201534285_text18021328811"></a><a name="zh-cn_topic_0201534285_text18021328811"></a>弹性公网IP</span>唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534285_section22054394"></a>

-   请求参数

    无

-   请求样例

    ```
    Get https://{Endpoint}/v1/{project_id}/publicips/{publicip_id}
    ```


## 响应消息<a name="zh-cn_topic_0201534285_section64271818"></a>

-   响应参数

    **表 2**  响应参数

    <a name="zh-cn_topic_0201534285_table64961662152123"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534285_row7248731152123"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534285_p50276345152123"><a name="zh-cn_topic_0201534285_p50276345152123"></a><a name="zh-cn_topic_0201534285_p50276345152123"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534285_p23039456152123"><a name="zh-cn_topic_0201534285_p23039456152123"></a><a name="zh-cn_topic_0201534285_p23039456152123"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534285_p54256632152123"><a name="zh-cn_topic_0201534285_p54256632152123"></a><a name="zh-cn_topic_0201534285_p54256632152123"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534285_row32711048152123"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p32349241152123"><a name="zh-cn_topic_0201534285_p32349241152123"></a><a name="zh-cn_topic_0201534285_p32349241152123"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p45145628152123"><a name="zh-cn_topic_0201534285_p45145628152123"></a><a name="zh-cn_topic_0201534285_p45145628152123"></a><a href="#zh-cn_topic_0201534285_table3035698">publicip</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p27820057152123"><a name="zh-cn_topic_0201534285_p27820057152123"></a><a name="zh-cn_topic_0201534285_p27820057152123"></a><span id="zh-cn_topic_0201534285_text14694153301117"><a name="zh-cn_topic_0201534285_text14694153301117"></a><a name="zh-cn_topic_0201534285_text14694153301117"></a></span><span id="zh-cn_topic_0201534285_text1269403311115"><a name="zh-cn_topic_0201534285_text1269403311115"></a><a name="zh-cn_topic_0201534285_text1269403311115"></a>弹性公网IP</span>对象，请参见<a href="#zh-cn_topic_0201534285_table3035698">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="zh-cn_topic_0201534285_table3035698"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534285_row64466590"><th class="cellrowborder" valign="top" width="18.208179182081793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534285_p54411269"><a name="zh-cn_topic_0201534285_p54411269"></a><a name="zh-cn_topic_0201534285_p54411269"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.907409259074093%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534285_p3124580518523"><a name="zh-cn_topic_0201534285_p3124580518523"></a><a name="zh-cn_topic_0201534285_p3124580518523"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.884411558844114%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534285_p40293226"><a name="zh-cn_topic_0201534285_p40293226"></a><a name="zh-cn_topic_0201534285_p40293226"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534285_row42525879"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p22044193"><a name="zh-cn_topic_0201534285_p22044193"></a><a name="zh-cn_topic_0201534285_p22044193"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p4788225318523"><a name="zh-cn_topic_0201534285_p4788225318523"></a><a name="zh-cn_topic_0201534285_p4788225318523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p44048571"><a name="zh-cn_topic_0201534285_p44048571"></a><a name="zh-cn_topic_0201534285_p44048571"></a><span id="zh-cn_topic_0201534285_text45641388116"><a name="zh-cn_topic_0201534285_text45641388116"></a><a name="zh-cn_topic_0201534285_text45641388116"></a></span><span id="zh-cn_topic_0201534285_text15564338201117"><a name="zh-cn_topic_0201534285_text15564338201117"></a><a name="zh-cn_topic_0201534285_text15564338201117"></a>弹性公网IP</span>唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row60892825"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p33371781"><a name="zh-cn_topic_0201534285_p33371781"></a><a name="zh-cn_topic_0201534285_p33371781"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p5325729418523"><a name="zh-cn_topic_0201534285_p5325729418523"></a><a name="zh-cn_topic_0201534285_p5325729418523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul1945793192"></a><a name="zh-cn_topic_0201534285_ul1945793192"></a><ul id="zh-cn_topic_0201534285_ul1945793192"><li>功能说明：<span id="zh-cn_topic_0201534285_text5579184151110"><a name="zh-cn_topic_0201534285_text5579184151110"></a><a name="zh-cn_topic_0201534285_text5579184151110"></a></span><span id="zh-cn_topic_0201534285_text15579194112118"><a name="zh-cn_topic_0201534285_text15579194112118"></a><a name="zh-cn_topic_0201534285_text15579194112118"></a>弹性公网IP</span>的状态</li><li>取值范围：<a name="zh-cn_topic_0201534285_ul4678228115815"></a><a name="zh-cn_topic_0201534285_ul4678228115815"></a><ul id="zh-cn_topic_0201534285_ul4678228115815"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row17803202152320"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p09743162419"><a name="zh-cn_topic_0201534285_p09743162419"></a><a name="zh-cn_topic_0201534285_p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p12971231132410"><a name="zh-cn_topic_0201534285_p12971231132410"></a><a name="zh-cn_topic_0201534285_p12971231132410"></a><a href="#zh-cn_topic_0201534285_table66651219193417">profile</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p169773114242"><a name="zh-cn_topic_0201534285_p169773114242"></a><a name="zh-cn_topic_0201534285_p169773114242"></a>功能说明：额外参数，包括订单id、产品id等信息，详情请参见<a href="#zh-cn_topic_0201534285_table66651219193417">表4</a>。</p>
    <p id="zh-cn_topic_0201534285_p156320510335"><a name="zh-cn_topic_0201534285_p156320510335"></a><a name="zh-cn_topic_0201534285_p156320510335"></a>约束：如果profile不为空，说明是包周期的<span id="zh-cn_topic_0201534285_text13895448101120"><a name="zh-cn_topic_0201534285_text13895448101120"></a><a name="zh-cn_topic_0201534285_text13895448101120"></a></span><span id="zh-cn_topic_0201534285_text9895174820119"><a name="zh-cn_topic_0201534285_text9895174820119"></a><a name="zh-cn_topic_0201534285_text9895174820119"></a>弹性公网IP</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row1722212174296"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p15848707"><a name="zh-cn_topic_0201534285_p15848707"></a><a name="zh-cn_topic_0201534285_p15848707"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p3408038918330"><a name="zh-cn_topic_0201534285_p3408038918330"></a><a name="zh-cn_topic_0201534285_p3408038918330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul7176216121014"></a><a name="zh-cn_topic_0201534285_ul7176216121014"></a><ul id="zh-cn_topic_0201534285_ul7176216121014"><li>功能说明：<span id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text941224173012"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text941224173012"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text941224173012"></a></span><span id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4412641113015"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4412641113015"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4412641113015"></a>弹性公网IP</span>的类型</li><li>取值范围：<em id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i16850184017499"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i16850184017499"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul585004064911"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul585004064911"></a><ul id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：<em id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i541911467911"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i541911467911"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_i541911467911"></a>5_bgp</em>、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li><span id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4018327273"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4018327273"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_text4018327273"></a>中国-香港</span>：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul9738153015499"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul9738153015499"></a><ul id="zh-cn_topic_0201534285_zh-cn_topic_0201534274_ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row16458145723915"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p175119718406"><a name="zh-cn_topic_0201534285_p175119718406"></a><a name="zh-cn_topic_0201534285_p175119718406"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p6512979403"><a name="zh-cn_topic_0201534285_p6512979403"></a><a name="zh-cn_topic_0201534285_p6512979403"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p115126714020"><a name="zh-cn_topic_0201534285_p115126714020"></a><a name="zh-cn_topic_0201534285_p115126714020"></a>IPv4时无此字段，IPv6时为申请到的<span id="zh-cn_topic_0201534285_text13320110122"><a name="zh-cn_topic_0201534285_text13320110122"></a><a name="zh-cn_topic_0201534285_text13320110122"></a></span><span id="zh-cn_topic_0201534285_text1232131121217"><a name="zh-cn_topic_0201534285_text1232131121217"></a><a name="zh-cn_topic_0201534285_text1232131121217"></a>弹性公网IP</span>地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row19379155218596"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p59653533594"><a name="zh-cn_topic_0201534285_p59653533594"></a><a name="zh-cn_topic_0201534285_p59653533594"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p139651253165911"><a name="zh-cn_topic_0201534285_p139651253165911"></a><a name="zh-cn_topic_0201534285_p139651253165911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p1696514537598"><a name="zh-cn_topic_0201534285_p1696514537598"></a><a name="zh-cn_topic_0201534285_p1696514537598"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row180110932914"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p171101456172118"><a name="zh-cn_topic_0201534285_p171101456172118"></a><a name="zh-cn_topic_0201534285_p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p1811012569218"><a name="zh-cn_topic_0201534285_p1811012569218"></a><a name="zh-cn_topic_0201534285_p1811012569218"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><div class="p" id="zh-cn_topic_0201534285_p1211011564217"><a name="zh-cn_topic_0201534285_p1211011564217"></a><a name="zh-cn_topic_0201534285_p1211011564217"></a>IP版本信息，取值范围是4和6<a name="zh-cn_topic_0201534285_ul13987110227"></a><a name="zh-cn_topic_0201534285_ul13987110227"></a><ul id="zh-cn_topic_0201534285_ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row66070243"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p50089467"><a name="zh-cn_topic_0201534285_p50089467"></a><a name="zh-cn_topic_0201534285_p50089467"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p1357258018523"><a name="zh-cn_topic_0201534285_p1357258018523"></a><a name="zh-cn_topic_0201534285_p1357258018523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul1693412582014"></a><a name="zh-cn_topic_0201534285_ul1693412582014"></a><ul id="zh-cn_topic_0201534285_ul1693412582014"><li>功能说明：绑定<span id="zh-cn_topic_0201534285_text1095561417127"><a name="zh-cn_topic_0201534285_text1095561417127"></a><a name="zh-cn_topic_0201534285_text1095561417127"></a></span><span id="zh-cn_topic_0201534285_text49554143127"><a name="zh-cn_topic_0201534285_text49554143127"></a><a name="zh-cn_topic_0201534285_text49554143127"></a>弹性公网IP</span>的私有IP地址</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534285_text1764617187121"><a name="zh-cn_topic_0201534285_text1764617187121"></a><a name="zh-cn_topic_0201534285_text1764617187121"></a></span><span id="zh-cn_topic_0201534285_text1646191819126"><a name="zh-cn_topic_0201534285_text1646191819126"></a><a name="zh-cn_topic_0201534285_text1646191819126"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row12246230153229"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p11971849153234"><a name="zh-cn_topic_0201534285_p11971849153234"></a><a name="zh-cn_topic_0201534285_p11971849153234"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p2563717518523"><a name="zh-cn_topic_0201534285_p2563717518523"></a><a name="zh-cn_topic_0201534285_p2563717518523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul420471472010"></a><a name="zh-cn_topic_0201534285_ul420471472010"></a><ul id="zh-cn_topic_0201534285_ul420471472010"><li>功能说明：端口id。</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534285_text1260872119127"><a name="zh-cn_topic_0201534285_text1260872119127"></a><a name="zh-cn_topic_0201534285_text1260872119127"></a></span><span id="zh-cn_topic_0201534285_text1660872117123"><a name="zh-cn_topic_0201534285_text1660872117123"></a><a name="zh-cn_topic_0201534285_text1660872117123"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row7204713"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p46710863"><a name="zh-cn_topic_0201534285_p46710863"></a><a name="zh-cn_topic_0201534285_p46710863"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p6334526618523"><a name="zh-cn_topic_0201534285_p6334526618523"></a><a name="zh-cn_topic_0201534285_p6334526618523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p25354291121"><a name="zh-cn_topic_0201534285_p25354291121"></a><a name="zh-cn_topic_0201534285_p25354291121"></a>项目ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row55494360"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p65858198"><a name="zh-cn_topic_0201534285_p65858198"></a><a name="zh-cn_topic_0201534285_p65858198"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p3069292618523"><a name="zh-cn_topic_0201534285_p3069292618523"></a><a name="zh-cn_topic_0201534285_p3069292618523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p36292894"><a name="zh-cn_topic_0201534285_p36292894"></a><a name="zh-cn_topic_0201534285_p36292894"></a><span id="zh-cn_topic_0201534285_text766216268127"><a name="zh-cn_topic_0201534285_text766216268127"></a><a name="zh-cn_topic_0201534285_text766216268127"></a></span><span id="zh-cn_topic_0201534285_text206621326111214"><a name="zh-cn_topic_0201534285_text206621326111214"></a><a name="zh-cn_topic_0201534285_text206621326111214"></a>弹性公网IP</span>申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row58200593"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p16627584"><a name="zh-cn_topic_0201534285_p16627584"></a><a name="zh-cn_topic_0201534285_p16627584"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p309907418523"><a name="zh-cn_topic_0201534285_p309907418523"></a><a name="zh-cn_topic_0201534285_p309907418523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p3934181618641"><a name="zh-cn_topic_0201534285_p3934181618641"></a><a name="zh-cn_topic_0201534285_p3934181618641"></a><span id="zh-cn_topic_0201534285_text13132112961213"><a name="zh-cn_topic_0201534285_text13132112961213"></a><a name="zh-cn_topic_0201534285_text13132112961213"></a></span><span id="zh-cn_topic_0201534285_text15132152911212"><a name="zh-cn_topic_0201534285_text15132152911212"></a><a name="zh-cn_topic_0201534285_text15132152911212"></a>弹性公网IP</span>对应带宽ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row51415138"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p3876622"><a name="zh-cn_topic_0201534285_p3876622"></a><a name="zh-cn_topic_0201534285_p3876622"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p4969847118523"><a name="zh-cn_topic_0201534285_p4969847118523"></a><a name="zh-cn_topic_0201534285_p4969847118523"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p2365466"><a name="zh-cn_topic_0201534285_p2365466"></a><a name="zh-cn_topic_0201534285_p2365466"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row21289199"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p46703582"><a name="zh-cn_topic_0201534285_p46703582"></a><a name="zh-cn_topic_0201534285_p46703582"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p6615323718523"><a name="zh-cn_topic_0201534285_p6615323718523"></a><a name="zh-cn_topic_0201534285_p6615323718523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul2255712095"></a><a name="zh-cn_topic_0201534285_ul2255712095"></a><ul id="zh-cn_topic_0201534285_ul2255712095"><li>功能说明：<span id="zh-cn_topic_0201534285_text17754163111125"><a name="zh-cn_topic_0201534285_text17754163111125"></a><a name="zh-cn_topic_0201534285_text17754163111125"></a></span><span id="zh-cn_topic_0201534285_text17754203112121"><a name="zh-cn_topic_0201534285_text17754203112121"></a><a name="zh-cn_topic_0201534285_text17754203112121"></a>弹性公网IP</span>的带宽类型</li><li>取值范围：PER，WHOLE。<a name="zh-cn_topic_0201534285_ul729412507220"></a><a name="zh-cn_topic_0201534285_ul729412507220"></a><ul id="zh-cn_topic_0201534285_ul729412507220"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    <a name="zh-cn_topic_0201534285_ul1369035014203"></a><a name="zh-cn_topic_0201534285_ul1369035014203"></a><ul id="zh-cn_topic_0201534285_ul1369035014203"><li>约束：其中IPv6暂不支持WHOLE类型带宽。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row5951536918414"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p6587627918414"><a name="zh-cn_topic_0201534285_p6587627918414"></a><a name="zh-cn_topic_0201534285_p6587627918414"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p3318647218414"><a name="zh-cn_topic_0201534285_p3318647218414"></a><a name="zh-cn_topic_0201534285_p3318647218414"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p374970718414"><a name="zh-cn_topic_0201534285_p374970718414"></a><a name="zh-cn_topic_0201534285_p374970718414"></a>带宽名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row7438151912404"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p979842771215"><a name="zh-cn_topic_0201534285_p979842771215"></a><a name="zh-cn_topic_0201534285_p979842771215"></a>alias</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p137987278128"><a name="zh-cn_topic_0201534285_p137987278128"></a><a name="zh-cn_topic_0201534285_p137987278128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p175531744191218"><a name="zh-cn_topic_0201534285_p175531744191218"></a><a name="zh-cn_topic_0201534285_p175531744191218"></a>弹性公网IP名称</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row1066119511342"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p19564181313543"><a name="zh-cn_topic_0201534285_p19564181313543"></a><a name="zh-cn_topic_0201534285_p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p13564413185412"><a name="zh-cn_topic_0201534285_p13564413185412"></a><a name="zh-cn_topic_0201534285_p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul184004104214"></a><a name="zh-cn_topic_0201534285_ul184004104214"></a><ul id="zh-cn_topic_0201534285_ul184004104214"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li><li>不指定该参数时，默认值是 0，0表示默认企业项目。</li></ul>
    <div class="note" id="zh-cn_topic_0201534285_note19041412125118"><a name="zh-cn_topic_0201534285_note19041412125118"></a><a name="zh-cn_topic_0201534285_note19041412125118"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201534285_zh-cn_topic_0201534275_p1915862704914"><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534275_p1915862704914"></a><a name="zh-cn_topic_0201534285_zh-cn_topic_0201534275_p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row0494191811246"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p1388313292268"><a name="zh-cn_topic_0201534285_p1388313292268"></a><a name="zh-cn_topic_0201534285_p1388313292268"></a>public_border_group</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p118831329122611"><a name="zh-cn_topic_0201534285_p118831329122611"></a><a name="zh-cn_topic_0201534285_p118831329122611"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p29889336324"><a name="zh-cn_topic_0201534285_p29889336324"></a><a name="zh-cn_topic_0201534285_p29889336324"></a>功能说明：表示中心站点资源或者边缘站点资源，对接了边缘站点的区域才会返回此字段</p>
    <p id="zh-cn_topic_0201534285_p20127195053611"><a name="zh-cn_topic_0201534285_p20127195053611"></a><a name="zh-cn_topic_0201534285_p20127195053611"></a>取值范围：</p>
    <a name="zh-cn_topic_0201534285_ul1660185933618"></a><a name="zh-cn_topic_0201534285_ul1660185933618"></a><ul id="zh-cn_topic_0201534285_ul1660185933618"><li>center</li><li>边缘站点名称</li></ul>
    <p id="zh-cn_topic_0201534285_p65761507386"><a name="zh-cn_topic_0201534285_p65761507386"></a><a name="zh-cn_topic_0201534285_p65761507386"></a>约束限制：只能绑定与该字段相同的publicip资源</p>
    <a name="zh-cn_topic_0201534285_ul16116154317382"></a><a name="zh-cn_topic_0201534285_ul16116154317382"></a>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row1623670161"><td class="cellrowborder" valign="top" width="18.208179182081793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p17216171341115"><a name="zh-cn_topic_0201534285_p17216171341115"></a><a name="zh-cn_topic_0201534285_p17216171341115"></a>allow_share_bandwidth_types</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.907409259074093%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p13216141361114"><a name="zh-cn_topic_0201534285_p13216141361114"></a><a name="zh-cn_topic_0201534285_p13216141361114"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.884411558844114%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534285_ul1756619360147"></a><a name="zh-cn_topic_0201534285_ul1756619360147"></a><ul id="zh-cn_topic_0201534285_ul1756619360147"><li>功能说明：表示此publicip可以加入的共享带宽类型列表。</li><li>如果列表为空，表示该publicip不能加入任何共享带宽。</li><li>约束：publicip只能加入到有该带宽类型的共享带宽中。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  profile字段说明

    <a name="zh-cn_topic_0201534285_table66651219193417"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534285_row167319197349"><th class="cellrowborder" valign="top" width="18.27%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534285_p206761195347"><a name="zh-cn_topic_0201534285_p206761195347"></a><a name="zh-cn_topic_0201534285_p206761195347"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.919999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534285_p156812193344"><a name="zh-cn_topic_0201534285_p156812193344"></a><a name="zh-cn_topic_0201534285_p156812193344"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.81%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534285_p17684101933410"><a name="zh-cn_topic_0201534285_p17684101933410"></a><a name="zh-cn_topic_0201534285_p17684101933410"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534285_row962259102216"><td class="cellrowborder" valign="top" width="18.27%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p962309182220"><a name="zh-cn_topic_0201534285_p962309182220"></a><a name="zh-cn_topic_0201534285_p962309182220"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.919999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p136231597223"><a name="zh-cn_topic_0201534285_p136231597223"></a><a name="zh-cn_topic_0201534285_p136231597223"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.81%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p26235912225"><a name="zh-cn_topic_0201534285_p26235912225"></a><a name="zh-cn_topic_0201534285_p26235912225"></a>订单的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row18686141920341"><td class="cellrowborder" valign="top" width="18.27%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p11688201923418"><a name="zh-cn_topic_0201534285_p11688201923418"></a><a name="zh-cn_topic_0201534285_p11688201923418"></a>product_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.919999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p169318196347"><a name="zh-cn_topic_0201534285_p169318196347"></a><a name="zh-cn_topic_0201534285_p169318196347"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.81%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p149921832153419"><a name="zh-cn_topic_0201534285_p149921832153419"></a><a name="zh-cn_topic_0201534285_p149921832153419"></a>产品的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row167161319173418"><td class="cellrowborder" valign="top" width="18.27%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p5718101903412"><a name="zh-cn_topic_0201534285_p5718101903412"></a><a name="zh-cn_topic_0201534285_p5718101903412"></a>region_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.919999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p47241019143417"><a name="zh-cn_topic_0201534285_p47241019143417"></a><a name="zh-cn_topic_0201534285_p47241019143417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.81%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p09201951174716"><a name="zh-cn_topic_0201534285_p09201951174716"></a><a name="zh-cn_topic_0201534285_p09201951174716"></a>region的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534285_row1472971912347"><td class="cellrowborder" valign="top" width="18.27%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534285_p187311719103415"><a name="zh-cn_topic_0201534285_p187311719103415"></a><a name="zh-cn_topic_0201534285_p187311719103415"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.919999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534285_p9735141923418"><a name="zh-cn_topic_0201534285_p9735141923418"></a><a name="zh-cn_topic_0201534285_p9735141923418"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.81%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534285_p09931918183013"><a name="zh-cn_topic_0201534285_p09931918183013"></a><a name="zh-cn_topic_0201534285_p09931918183013"></a>用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "publicip": {
            "id": "2ec9b78d-9368-46f3-8f29-d1a95622a568",
            "status": "DOWN",
            "profile": {
              "user_id": "35f2b308f5d64441a6fa7999fbcd4321",
              "product_id": "00301-48027-0--0",
              "region_id": "xxx",
              "order_id": "xxxxxxxxx"
            },
            "type": "5_bgp",
            "public_ip_address": "161.xx.xx.12",
            "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
            "private_ip_address": "192.168.10.5",
            "create_time": "2015-07-16 04:32:50",
            "bandwidth_id": "49c8825b-bed9-46ff-9416-704b96d876a2",
            "bandwidth_share_type": "PER",
            "bandwidth_size": 10,    //EIP的带宽大小为10Mbit/s
            "bandwidth_name": "bandwidth-test",
            "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439",
            "ip_version": 4
        }
    }
    ```


## 状态码<a name="zh-cn_topic_0201534285_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534285_section85821649202813"></a>

请参考[错误码](错误码.md)。

