# 申请包周期弹性公网IP<a name="eip_api_0006"></a>

## 功能介绍<a name="zh-cn_topic_0201534185_section95417125714"></a>

申请包年包月的弹性公网IP。

在成功调用本接口申请包年包月的弹性公网IP后：

-   如果您需要支付订单，请参考“[支付包周期产品订单](https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746561.html)”进行支付。若想使用优惠券，请将请求中的is\_auto\_pay字段设置为false，参考“[查询订单可用优惠券](https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0092953630.html)”进行支付，或者在华为云官网页面使用优惠券进行支付。
-   如果您需要查询订单的资源开通详情，请参考“[查询订单的资源开通详情](https://support.huaweicloud.com/api-oce/api_order_00001.html)”。
-   如果您需要退订该包周期资源，请参考“[退订包周期资源](https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html)”。

## URI<a name="zh-cn_topic_0201534185_section135831105716"></a>

POST /v2.0/\{project\_id\}/publicips

参数说明请参见[表1](#zh-cn_topic_0201534185_table56312185710)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534185_table56312185710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534185_row1965641135717"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534185_p665618113574"><a name="zh-cn_topic_0201534185_p665618113574"></a><a name="zh-cn_topic_0201534185_p665618113574"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534185_p166564116579"><a name="zh-cn_topic_0201534185_p166564116579"></a><a name="zh-cn_topic_0201534185_p166564116579"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534185_p3657101185710"><a name="zh-cn_topic_0201534185_p3657101185710"></a><a name="zh-cn_topic_0201534185_p3657101185710"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534185_row166578119574"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p1865719114578"><a name="zh-cn_topic_0201534185_p1865719114578"></a><a name="zh-cn_topic_0201534185_p1865719114578"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p18657181175718"><a name="zh-cn_topic_0201534185_p18657181175718"></a><a name="zh-cn_topic_0201534185_p18657181175718"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p10487112"><a name="zh-cn_topic_0201534185_p10487112"></a><a name="zh-cn_topic_0201534185_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="zh-cn_topic_0201534185_section14762185713"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534185_table15872015575"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row126571614572"><th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534185_p1465751175719"><a name="zh-cn_topic_0201534185_p1465751175719"></a><a name="zh-cn_topic_0201534185_p1465751175719"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534185_p56571318579"><a name="zh-cn_topic_0201534185_p56571318579"></a><a name="zh-cn_topic_0201534185_p56571318579"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.42785721427857%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534185_p1657161135717"><a name="zh-cn_topic_0201534185_p1657161135717"></a><a name="zh-cn_topic_0201534185_p1657161135717"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.95520447955205%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534185_p965717135716"><a name="zh-cn_topic_0201534185_p965717135716"></a><a name="zh-cn_topic_0201534185_p965717135716"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row166579118574"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p565741155713"><a name="zh-cn_topic_0201534185_p565741155713"></a><a name="zh-cn_topic_0201534185_p565741155713"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p5657161175715"><a name="zh-cn_topic_0201534185_p5657161175715"></a><a name="zh-cn_topic_0201534185_p5657161175715"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p865721165716"><a name="zh-cn_topic_0201534185_p865721165716"></a><a name="zh-cn_topic_0201534185_p865721165716"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534185_p465781125718"><a name="zh-cn_topic_0201534185_p465781125718"></a><a name="zh-cn_topic_0201534185_p465781125718"></a>弹性公网IP对象，请参见<a href="#zh-cn_topic_0201534185_table91041517574">表3</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row1465781175717"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p15657131175716"><a name="zh-cn_topic_0201534185_p15657131175716"></a><a name="zh-cn_topic_0201534185_p15657131175716"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p765771205716"><a name="zh-cn_topic_0201534185_p765771205716"></a><a name="zh-cn_topic_0201534185_p765771205716"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p16657181155715"><a name="zh-cn_topic_0201534185_p16657181155715"></a><a name="zh-cn_topic_0201534185_p16657181155715"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534185_p965771145711"><a name="zh-cn_topic_0201534185_p965771145711"></a><a name="zh-cn_topic_0201534185_p965771145711"></a>带宽对象，请参见<a href="#zh-cn_topic_0201534185_table15129191175710">表4</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row36589119571"><td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p1265815112573"><a name="zh-cn_topic_0201534185_p1265815112573"></a><a name="zh-cn_topic_0201534185_p1265815112573"></a>extendParam</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p186581217571"><a name="zh-cn_topic_0201534185_p186581217571"></a><a name="zh-cn_topic_0201534185_p186581217571"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.42785721427857%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p965861175711"><a name="zh-cn_topic_0201534185_p965861175711"></a><a name="zh-cn_topic_0201534185_p965861175711"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.95520447955205%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534185_p14658615577"><a name="zh-cn_topic_0201534185_p14658615577"></a><a name="zh-cn_topic_0201534185_p14658615577"></a>扩展参数，用于包周期资源申请。请参见<a href="#zh-cn_topic_0201534185_table1616617135712">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="zh-cn_topic_0201534185_table91041517574"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row2065811135712"><th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534185_p12658181125714"><a name="zh-cn_topic_0201534185_p12658181125714"></a><a name="zh-cn_topic_0201534185_p12658181125714"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534185_p166581415574"><a name="zh-cn_topic_0201534185_p166581415574"></a><a name="zh-cn_topic_0201534185_p166581415574"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534185_p1965801105715"><a name="zh-cn_topic_0201534185_p1965801105715"></a><a name="zh-cn_topic_0201534185_p1965801105715"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534185_p56582105713"><a name="zh-cn_topic_0201534185_p56582105713"></a><a name="zh-cn_topic_0201534185_p56582105713"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row1065821115717"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p30749271"><a name="zh-cn_topic_0201534185_p30749271"></a><a name="zh-cn_topic_0201534185_p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p7663035"><a name="zh-cn_topic_0201534185_p7663035"></a><a name="zh-cn_topic_0201534185_p7663035"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p70444218129"><a name="zh-cn_topic_0201534185_p70444218129"></a><a name="zh-cn_topic_0201534185_p70444218129"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul29589093174724"></a><a name="zh-cn_topic_0201534185_ul29589093174724"></a><ul id="zh-cn_topic_0201534185_ul29589093174724"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="zh-cn_topic_0201534185_i16850184017499"><a name="zh-cn_topic_0201534185_i16850184017499"></a><a name="zh-cn_topic_0201534185_i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534185_ul585004064911"></a><a name="zh-cn_topic_0201534185_ul585004064911"></a><ul id="zh-cn_topic_0201534185_ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534185_ul9738153015499"></a><a name="zh-cn_topic_0201534185_ul9738153015499"></a><ul id="zh-cn_topic_0201534185_ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row2935112184111"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p712415486592"><a name="zh-cn_topic_0201534185_p712415486592"></a><a name="zh-cn_topic_0201534185_p712415486592"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p1412434815914"><a name="zh-cn_topic_0201534185_p1412434815914"></a><a name="zh-cn_topic_0201534185_p1412434815914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p112413482593"><a name="zh-cn_topic_0201534185_p112413482593"></a><a name="zh-cn_topic_0201534185_p112413482593"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul1842191914615"></a><a name="zh-cn_topic_0201534185_ul1842191914615"></a><ul id="zh-cn_topic_0201534185_ul1842191914615"><li>功能说明：弹性公网IP的版本</li><li>取值范围：4、6，分别表示创建ipv4和ipv6</li><li>约束：<a name="zh-cn_topic_0201534185_ul1190139775"></a><a name="zh-cn_topic_0201534185_ul1190139775"></a><ul id="zh-cn_topic_0201534185_ul1190139775"><li>必须是系统具体支持的类型</li><li>不填或空字符串时，默认创建ipv4</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  bandwidth字段说明

    <a name="zh-cn_topic_0201534185_table15129191175710"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row1665918116579"><th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534185_p765971205718"><a name="zh-cn_topic_0201534185_p765971205718"></a><a name="zh-cn_topic_0201534185_p765971205718"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534185_p18659111125710"><a name="zh-cn_topic_0201534185_p18659111125710"></a><a name="zh-cn_topic_0201534185_p18659111125710"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534185_p965901145714"><a name="zh-cn_topic_0201534185_p965901145714"></a><a name="zh-cn_topic_0201534185_p965901145714"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534185_p26593115712"><a name="zh-cn_topic_0201534185_p26593115712"></a><a name="zh-cn_topic_0201534185_p26593115712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row96591313578"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p86597165720"><a name="zh-cn_topic_0201534185_p86597165720"></a><a name="zh-cn_topic_0201534185_p86597165720"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p1165971175715"><a name="zh-cn_topic_0201534185_p1165971175715"></a><a name="zh-cn_topic_0201534185_p1165971175715"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p165918117578"><a name="zh-cn_topic_0201534185_p165918117578"></a><a name="zh-cn_topic_0201534185_p165918117578"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul4651549103511"></a><a name="zh-cn_topic_0201534185_ul4651549103511"></a><ul id="zh-cn_topic_0201534185_ul4651549103511"><li>功能说明：带宽名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li><li>约束：<a name="zh-cn_topic_0201534185_ul56861953103518"></a><a name="zh-cn_topic_0201534185_ul56861953103518"></a><ul id="zh-cn_topic_0201534185_ul56861953103518"><li>如果share_type是PER，该字段是必选。</li><li>如果bandwidth对象的id有值，该字段被忽略。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row56591115718"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p8659101115716"><a name="zh-cn_topic_0201534185_p8659101115716"></a><a name="zh-cn_topic_0201534185_p8659101115716"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p26591318572"><a name="zh-cn_topic_0201534185_p26591318572"></a><a name="zh-cn_topic_0201534185_p26591318572"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p4659181175718"><a name="zh-cn_topic_0201534185_p4659181175718"></a><a name="zh-cn_topic_0201534185_p4659181175718"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul9790510185"></a><a name="zh-cn_topic_0201534185_ul9790510185"></a><ul id="zh-cn_topic_0201534185_ul9790510185"><li>功能说明：带宽大小</li><li>取值范围：默认1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</li><li>约束：share_type取值PER时，该字段必选。如果bandwidth对象的id有值，该字段被忽略。</li><li>注意：调整带宽时的最小单位会根据带宽范围不同存在差异。<a name="zh-cn_topic_0201534185_ul4773151615366"></a><a name="zh-cn_topic_0201534185_ul4773151615366"></a><ul id="zh-cn_topic_0201534185_ul4773151615366"><li>小于等于300Mbit/s：默认最小单位为1Mbit/s。</li><li>300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。</li><li>大于1000Mbit/s：默认最小单位为500Mbit/s。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row565991115718"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p196595175716"><a name="zh-cn_topic_0201534185_p196595175716"></a><a name="zh-cn_topic_0201534185_p196595175716"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p126597105713"><a name="zh-cn_topic_0201534185_p126597105713"></a><a name="zh-cn_topic_0201534185_p126597105713"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p196606165717"><a name="zh-cn_topic_0201534185_p196606165717"></a><a name="zh-cn_topic_0201534185_p196606165717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul940614814366"></a><a name="zh-cn_topic_0201534185_ul940614814366"></a><ul id="zh-cn_topic_0201534185_ul940614814366"><li>功能说明：使用已有的共享带宽创建IP</li><li>取值范围：共享带宽ID</li><li>约束：<a name="zh-cn_topic_0201534185_ul3277456133617"></a><a name="zh-cn_topic_0201534185_ul3277456133617"></a><ul id="zh-cn_topic_0201534185_ul3277456133617"><li>WHOLE类型的带宽ID；</li><li>在预付费的情况下，不填该值。该字段取空字符串时，会被忽略。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row196601419579"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p1166021105718"><a name="zh-cn_topic_0201534185_p1166021105718"></a><a name="zh-cn_topic_0201534185_p1166021105718"></a>share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p19660316577"><a name="zh-cn_topic_0201534185_p19660316577"></a><a name="zh-cn_topic_0201534185_p19660316577"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p5660919572"><a name="zh-cn_topic_0201534185_p5660919572"></a><a name="zh-cn_topic_0201534185_p5660919572"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul850110171372"></a><a name="zh-cn_topic_0201534185_ul850110171372"></a><ul id="zh-cn_topic_0201534185_ul850110171372"><li>功能说明：带宽类型</li><li>取值范围：<a name="zh-cn_topic_0201534185_ul9698817175619"></a><a name="zh-cn_topic_0201534185_ul9698817175619"></a><ul id="zh-cn_topic_0201534185_ul9698817175619"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li><li>使用已有带宽创建IP时，该字段的值，以带宽的共享类型为准。</li><li>约束：在预付费的情况下，只能使用PER类型</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row1660131135719"><td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p96604119574"><a name="zh-cn_topic_0201534185_p96604119574"></a><a name="zh-cn_topic_0201534185_p96604119574"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p066010175715"><a name="zh-cn_topic_0201534185_p066010175715"></a><a name="zh-cn_topic_0201534185_p066010175715"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p1166021195720"><a name="zh-cn_topic_0201534185_p1166021195720"></a><a name="zh-cn_topic_0201534185_p1166021195720"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul48781258153710"></a><a name="zh-cn_topic_0201534185_ul48781258153710"></a><ul id="zh-cn_topic_0201534185_ul48781258153710"><li>功能说明：计费模式，按流量计费或者按带宽计费。</li><li>取值范围：bandwidth，traffic，默认是bandwidth。取值为traffic，表示流量计费。</li><li>约束：包周期的弹性IP带宽计费模式只能按照带宽计费。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  extendParam字段说明

    <a name="zh-cn_topic_0201534185_table1616617135712"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row1666011115575"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534185_p19660131125711"><a name="zh-cn_topic_0201534185_p19660131125711"></a><a name="zh-cn_topic_0201534185_p19660131125711"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.252525252525254%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534185_p866014175712"><a name="zh-cn_topic_0201534185_p866014175712"></a><a name="zh-cn_topic_0201534185_p866014175712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.090909090909093%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534185_p12660111125715"><a name="zh-cn_topic_0201534185_p12660111125715"></a><a name="zh-cn_topic_0201534185_p12660111125715"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534185_p1866091105712"><a name="zh-cn_topic_0201534185_p1866091105712"></a><a name="zh-cn_topic_0201534185_p1866091105712"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row1066011118573"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p66604118574"><a name="zh-cn_topic_0201534185_p66604118574"></a><a name="zh-cn_topic_0201534185_p66604118574"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.252525252525254%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p2660111135718"><a name="zh-cn_topic_0201534185_p2660111135718"></a><a name="zh-cn_topic_0201534185_p2660111135718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.090909090909093%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p8660111115715"><a name="zh-cn_topic_0201534185_p8660111115715"></a><a name="zh-cn_topic_0201534185_p8660111115715"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul4848115153813"></a><a name="zh-cn_topic_0201534185_ul4848115153813"></a><ul id="zh-cn_topic_0201534185_ul4848115153813"><li>功能说明：付费方式（预付费、按需付费；预付费，即包周期付费）</li><li>取值范围：<a name="zh-cn_topic_0201534185_ul169751157183817"></a><a name="zh-cn_topic_0201534185_ul169751157183817"></a><ul id="zh-cn_topic_0201534185_ul169751157183817"><li>prePaid -预付费，即包年包月；</li><li>postPaid -后付费，即按需付费；</li><li>默认值是postPaid。</li></ul>
    </li><li>后付费的场景下，extendParam的其他字段都会被忽略。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row66611219574"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p1666120145712"><a name="zh-cn_topic_0201534185_p1666120145712"></a><a name="zh-cn_topic_0201534185_p1666120145712"></a>period_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.252525252525254%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p1666131105719"><a name="zh-cn_topic_0201534185_p1666131105719"></a><a name="zh-cn_topic_0201534185_p1666131105719"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.090909090909093%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p76616185712"><a name="zh-cn_topic_0201534185_p76616185712"></a><a name="zh-cn_topic_0201534185_p76616185712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul182664270396"></a><a name="zh-cn_topic_0201534185_ul182664270396"></a><ul id="zh-cn_topic_0201534185_ul182664270396"><li>功能说明：订购资源的周期类型（包年、包月等）。</li><li>取值范围：<a name="zh-cn_topic_0201534185_ul1188493318393"></a><a name="zh-cn_topic_0201534185_ul1188493318393"></a><ul id="zh-cn_topic_0201534185_ul1188493318393"><li>month-月</li><li>year-年</li></ul>
    </li><li>约束：<p id="zh-cn_topic_0201534185_p1027114324528"><a name="zh-cn_topic_0201534185_p1027114324528"></a><a name="zh-cn_topic_0201534185_p1027114324528"></a>如果用包周期共享带宽创建时（即携带共享带宽id创建弹性公网IP）此字段可不填。付费方式是预付费且不是使用共享带宽创建IP时，该字段必选；</p>
    </li></ul>
    <p id="zh-cn_topic_0201534185_p1979334215564"><a name="zh-cn_topic_0201534185_p1979334215564"></a><a name="zh-cn_topic_0201534185_p1979334215564"></a>使用共享带宽创建IP时，带宽资源到期时间与IP的到期时间相同。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row166111135717"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p12661318573"><a name="zh-cn_topic_0201534185_p12661318573"></a><a name="zh-cn_topic_0201534185_p12661318573"></a>period_num</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.252525252525254%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p36616113576"><a name="zh-cn_topic_0201534185_p36616113576"></a><a name="zh-cn_topic_0201534185_p36616113576"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.090909090909093%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p166611514573"><a name="zh-cn_topic_0201534185_p166611514573"></a><a name="zh-cn_topic_0201534185_p166611514573"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul4447175653915"></a><a name="zh-cn_topic_0201534185_ul4447175653915"></a><ul id="zh-cn_topic_0201534185_ul4447175653915"><li>功能说明：订购周期数</li><li>取值范围：(后续会随运营策略变化)<a name="zh-cn_topic_0201534185_ul52991518407"></a><a name="zh-cn_topic_0201534185_ul52991518407"></a><ul id="zh-cn_topic_0201534185_ul52991518407"><li>period_type为month时，为[1,9]，</li><li>period_type为year时，为[1,3]</li></ul>
    </li><li>约束：同period_type约束。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row1666191155718"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p176615185712"><a name="zh-cn_topic_0201534185_p176615185712"></a><a name="zh-cn_topic_0201534185_p176615185712"></a>is_auto_renew</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.252525252525254%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p1166112125711"><a name="zh-cn_topic_0201534185_p1166112125711"></a><a name="zh-cn_topic_0201534185_p1166112125711"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.090909090909093%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p966110165717"><a name="zh-cn_topic_0201534185_p966110165717"></a><a name="zh-cn_topic_0201534185_p966110165717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul1059612233404"></a><a name="zh-cn_topic_0201534185_ul1059612233404"></a><ul id="zh-cn_topic_0201534185_ul1059612233404"><li>功能说明：是否自动续订</li><li>取值范围：<p id="zh-cn_topic_0201534185_p437113598116"><a name="zh-cn_topic_0201534185_p437113598116"></a><a name="zh-cn_topic_0201534185_p437113598116"></a>false：不自动续订；true：自动续订；默认值：false</p>
    </li><li>约束：<p id="zh-cn_topic_0201534185_p797817497111"><a name="zh-cn_topic_0201534185_p797817497111"></a><a name="zh-cn_topic_0201534185_p797817497111"></a>到期后，默认自动续订1个月（自动续订时间后续可能会变化），详情可联系客服咨询。</p>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row566112118576"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534185_p166111105711"><a name="zh-cn_topic_0201534185_p166111105711"></a><a name="zh-cn_topic_0201534185_p166111105711"></a>is_auto_pay</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.252525252525254%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534185_p7661215578"><a name="zh-cn_topic_0201534185_p7661215578"></a><a name="zh-cn_topic_0201534185_p7661215578"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.090909090909093%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534185_p266218155720"><a name="zh-cn_topic_0201534185_p266218155720"></a><a name="zh-cn_topic_0201534185_p266218155720"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534185_ul781495117401"></a><a name="zh-cn_topic_0201534185_ul781495117401"></a><ul id="zh-cn_topic_0201534185_ul781495117401"><li>功能说明：下单订购后，是否自动从客户的账户中支付；默认是“不自动支付”</li><li>取值范围：<a name="zh-cn_topic_0201534185_ul1754865674019"></a><a name="zh-cn_topic_0201534185_ul1754865674019"></a><ul id="zh-cn_topic_0201534185_ul1754865674019"><li>true：是（自动支付，从账户余额自动扣费）</li><li>false：否（默认值，只提交订单不支付，需要客户手动去支付）</li></ul>
    </li><li>约束：<p id="zh-cn_topic_0201534185_p483505155946"><a name="zh-cn_topic_0201534185_p483505155946"></a><a name="zh-cn_topic_0201534185_p483505155946"></a>自动支付时，只能使用账户的现金支付；如果要使用代金券，请选择不自动支付，然后在用户费用中心，选择代金券支付。</p>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例1

    创建包周期独占带宽和弹性公网IP，大小1Mbit/s，周期1个月。不自动续费，不自动扣费。

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips
    
    {
        "publicip": {
            "type": "5_bgp"
        },
        "bandwidth": {
            "name": "bw_666",
            "size": 1,
            "share_type": "PER",
            "charge_mode": "bandwidth"
        },
        "extendParam": {
            "charge_mode": "prePaid",
            "period_type": "month",
            "period_num": 1,
            "is_auto_renew": "false",
            "is_auto_pay": "true"
        }
    }
    ```

-   请求样例2

    创建按需的IP、带宽；extendParam扩展字段，不填即可。

    ```
    POST https://{Endpoint}/v2.0/{project_id}/publicips
    
    {
        "publicip": {
            "type": "5_bgp"
        },
        "bandwidth": {
            "name": "bw_666",
            "size": 1,
            "share_type": "PER",
            "charge_mode": "bandwidth"
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534185_section4196111195719"></a>

-   响应参数

    <a name="zh-cn_topic_0201534185_table719831105710"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row206633110574"><th class="cellrowborder" valign="top" width="18.08%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0201534185_p116636185715"><a name="zh-cn_topic_0201534185_p116636185715"></a><a name="zh-cn_topic_0201534185_p116636185715"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.3%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0201534185_p1766313112570"><a name="zh-cn_topic_0201534185_p1766313112570"></a><a name="zh-cn_topic_0201534185_p1766313112570"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.620000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0201534185_p066391195720"><a name="zh-cn_topic_0201534185_p066391195720"></a><a name="zh-cn_topic_0201534185_p066391195720"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row7663161195710"><td class="cellrowborder" valign="top" width="18.08%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0201534185_p4663112575"><a name="zh-cn_topic_0201534185_p4663112575"></a><a name="zh-cn_topic_0201534185_p4663112575"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0201534185_p176632120574"><a name="zh-cn_topic_0201534185_p176632120574"></a><a name="zh-cn_topic_0201534185_p176632120574"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.620000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0201534185_p1266319110571"><a name="zh-cn_topic_0201534185_p1266319110571"></a><a name="zh-cn_topic_0201534185_p1266319110571"></a>弹性公网IP对象（后付费场景返回对象）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row196635135712"><td class="cellrowborder" valign="top" width="18.08%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0201534185_p1366441185715"><a name="zh-cn_topic_0201534185_p1366441185715"></a><a name="zh-cn_topic_0201534185_p1366441185715"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.3%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0201534185_p1966419105711"><a name="zh-cn_topic_0201534185_p1966419105711"></a><a name="zh-cn_topic_0201534185_p1966419105711"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.620000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0201534185_p566413115570"><a name="zh-cn_topic_0201534185_p566413115570"></a><a name="zh-cn_topic_0201534185_p566413115570"></a>订单号（预付费场景返回该字段）</p>
    <div class="note" id="zh-cn_topic_0201534185_note172685205318"><a name="zh-cn_topic_0201534185_note172685205318"></a><a name="zh-cn_topic_0201534185_note172685205318"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0201534185_ul619218461815"></a><a name="zh-cn_topic_0201534185_ul619218461815"></a><ul id="zh-cn_topic_0201534185_ul619218461815"><li>如果需要支付订单，请参考<a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">支付包周期产品订单</a>。</li></ul>
    <a name="zh-cn_topic_0201534185_ul530215481987"></a><a name="zh-cn_topic_0201534185_ul530215481987"></a><ul id="zh-cn_topic_0201534185_ul530215481987"><li>如果需要查询订单的资源开通详情，请参考“<a href="https://support.huaweicloud.com/api-oce/api_order_00001.html" target="_blank" rel="noopener noreferrer">查询订单的资源开通详情</a>”。</li><li>如果需要退订该包周期资源，请参考“<a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">退订包周期资源</a>”。</li></ul>
    <p id="zh-cn_topic_0201534185_p925914325818"><a name="zh-cn_topic_0201534185_p925914325818"></a><a name="zh-cn_topic_0201534185_p925914325818"></a></p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  publicip字段说明

    <a name="zh-cn_topic_0201534185_table12207101195717"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534185_row86647165710"><th class="cellrowborder" valign="top" width="18.781878187818783%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534185_p146642116578"><a name="zh-cn_topic_0201534185_p146642116578"></a><a name="zh-cn_topic_0201534185_p146642116578"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.802480248024803%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534185_p966461125710"><a name="zh-cn_topic_0201534185_p966461125710"></a><a name="zh-cn_topic_0201534185_p966461125710"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.41564156415642%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534185_p86642018575"><a name="zh-cn_topic_0201534185_p86642018575"></a><a name="zh-cn_topic_0201534185_p86642018575"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534185_row19664316570"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p166419135719"><a name="zh-cn_topic_0201534185_p166419135719"></a><a name="zh-cn_topic_0201534185_p166419135719"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p766410195716"><a name="zh-cn_topic_0201534185_p766410195716"></a><a name="zh-cn_topic_0201534185_p766410195716"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p36641516576"><a name="zh-cn_topic_0201534185_p36641516576"></a><a name="zh-cn_topic_0201534185_p36641516576"></a>弹性公网IP唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row1266412113577"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p196641195712"><a name="zh-cn_topic_0201534185_p196641195712"></a><a name="zh-cn_topic_0201534185_p196641195712"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p466416125717"><a name="zh-cn_topic_0201534185_p466416125717"></a><a name="zh-cn_topic_0201534185_p466416125717"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534185_ul19116513422"></a><a name="zh-cn_topic_0201534185_ul19116513422"></a><ul id="zh-cn_topic_0201534185_ul19116513422"><li>功能说明：弹性公网IP的状态</li><li>取值范围：<a name="zh-cn_topic_0201534185_ul15948194512578"></a><a name="zh-cn_topic_0201534185_ul15948194512578"></a><ul id="zh-cn_topic_0201534185_ul15948194512578"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row146646155711"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p13406917195317"><a name="zh-cn_topic_0201534185_p13406917195317"></a><a name="zh-cn_topic_0201534185_p13406917195317"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p1588502212317"><a name="zh-cn_topic_0201534185_p1588502212317"></a><a name="zh-cn_topic_0201534185_p1588502212317"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534185_ul28851022135"></a><a name="zh-cn_topic_0201534185_ul28851022135"></a><ul id="zh-cn_topic_0201534185_ul28851022135"><li>功能说明：弹性公网IP的类型</li><li>取值范围：<em id="zh-cn_topic_0201534185_i3737141110610"><a name="zh-cn_topic_0201534185_i3737141110610"></a><a name="zh-cn_topic_0201534185_i3737141110610"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534185_ul773751116619"></a><a name="zh-cn_topic_0201534185_ul773751116619"></a><ul id="zh-cn_topic_0201534185_ul773751116619"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：5_bgp、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li>亚太-香港：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534185_ul9737141112610"></a><a name="zh-cn_topic_0201534185_ul9737141112610"></a><ul id="zh-cn_topic_0201534185_ul9737141112610"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"publicip_type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row666491145710"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p36645114579"><a name="zh-cn_topic_0201534185_p36645114579"></a><a name="zh-cn_topic_0201534185_p36645114579"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p196641014573"><a name="zh-cn_topic_0201534185_p196641014573"></a><a name="zh-cn_topic_0201534185_p196641014573"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p19576252174619"><a name="zh-cn_topic_0201534185_p19576252174619"></a><a name="zh-cn_topic_0201534185_p19576252174619"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row88911219154214"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p174765913710"><a name="zh-cn_topic_0201534185_p174765913710"></a><a name="zh-cn_topic_0201534185_p174765913710"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p18476149163714"><a name="zh-cn_topic_0201534185_p18476149163714"></a><a name="zh-cn_topic_0201534185_p18476149163714"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p167581149102812"><a name="zh-cn_topic_0201534185_p167581149102812"></a><a name="zh-cn_topic_0201534185_p167581149102812"></a>IPv4时无此字段，IPv6时为申请到的弹性公网IP地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row933062812445"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p171101456172118"><a name="zh-cn_topic_0201534185_p171101456172118"></a><a name="zh-cn_topic_0201534185_p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p1811012569218"><a name="zh-cn_topic_0201534185_p1811012569218"></a><a name="zh-cn_topic_0201534185_p1811012569218"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p10645141832513"><a name="zh-cn_topic_0201534185_p10645141832513"></a><a name="zh-cn_topic_0201534185_p10645141832513"></a>IP版本信息，取值范围是4和6</p>
    <a name="zh-cn_topic_0201534185_ul13987110227"></a><a name="zh-cn_topic_0201534185_ul13987110227"></a><ul id="zh-cn_topic_0201534185_ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row366410119579"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p46646115713"><a name="zh-cn_topic_0201534185_p46646115713"></a><a name="zh-cn_topic_0201534185_p46646115713"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p66640115716"><a name="zh-cn_topic_0201534185_p66640115716"></a><a name="zh-cn_topic_0201534185_p66640115716"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p1484814291233"><a name="zh-cn_topic_0201534185_p1484814291233"></a><a name="zh-cn_topic_0201534185_p1484814291233"></a>项目ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row1966411195714"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p126656118578"><a name="zh-cn_topic_0201534185_p126656118578"></a><a name="zh-cn_topic_0201534185_p126656118578"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p666517111573"><a name="zh-cn_topic_0201534185_p666517111573"></a><a name="zh-cn_topic_0201534185_p666517111573"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p166519135713"><a name="zh-cn_topic_0201534185_p166519135713"></a><a name="zh-cn_topic_0201534185_p166519135713"></a>弹性公网IP申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row56651165710"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p46651711577"><a name="zh-cn_topic_0201534185_p46651711577"></a><a name="zh-cn_topic_0201534185_p46651711577"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p16665714575"><a name="zh-cn_topic_0201534185_p16665714575"></a><a name="zh-cn_topic_0201534185_p16665714575"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534185_p36659155710"><a name="zh-cn_topic_0201534185_p36659155710"></a><a name="zh-cn_topic_0201534185_p36659155710"></a>带宽大小</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534185_row163534111354"><td class="cellrowborder" valign="top" width="18.781878187818783%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534185_p415181314516"><a name="zh-cn_topic_0201534185_p415181314516"></a><a name="zh-cn_topic_0201534185_p415181314516"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.802480248024803%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534185_p171612139511"><a name="zh-cn_topic_0201534185_p171612139511"></a><a name="zh-cn_topic_0201534185_p171612139511"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.41564156415642%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534185_ul816191312517"></a><a name="zh-cn_topic_0201534185_ul816191312517"></a><ul id="zh-cn_topic_0201534185_ul816191312517"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例1

    包年包月场景

    ```
    {
        "order_id": "CS1802081410IMDRN"
    }
    ```


-   响应样例2

    按需场景

    ```
    {
      "publicip": {
        "id": "4eaf3b63-48ca-4410-ab85-bdfddf4b35fd",
        "status": "PENDING_CREATE",
        "type": "5_bgp",
        "public_ip_address": "10.xx.xx.238",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-03-27 13:11:58",
        "bandwidth_size": 0,
        "enterprise_project_id": "0",
        "ip_version": 4
      }
    }
    ```


## 状态码<a name="zh-cn_topic_0201534185_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534185_section85821649202813"></a>

请参考[错误码](错误码.md)。

