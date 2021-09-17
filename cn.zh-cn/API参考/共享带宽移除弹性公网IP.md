# 共享带宽移除弹性公网IP<a name="eip_apisharedbandwidth_0005"></a>

## 功能介绍<a name="zh-cn_topic_0201534216_section16581154"></a>

共享带宽移除弹性公网IP。

## 调试<a name="zh-cn_topic_0201534216_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&version=v2&api=RemovePublicipsFromSharedBandwidth)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0201534216_section15012662"></a>

POST /v2.0/\{project\_id\}/bandwidths/\{bandwidth\_id\}/remove

参数说明请参见[表1](#zh-cn_topic_0201534216_table25281875)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534216_table25281875"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534216_row26712487"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534216_p16227847"><a name="zh-cn_topic_0201534216_p16227847"></a><a name="zh-cn_topic_0201534216_p16227847"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534216_p39387211"><a name="zh-cn_topic_0201534216_p39387211"></a><a name="zh-cn_topic_0201534216_p39387211"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534216_p36247516"><a name="zh-cn_topic_0201534216_p36247516"></a><a name="zh-cn_topic_0201534216_p36247516"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534216_row50367649"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534216_p53247746"><a name="zh-cn_topic_0201534216_p53247746"></a><a name="zh-cn_topic_0201534216_p53247746"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534216_p18100201"><a name="zh-cn_topic_0201534216_p18100201"></a><a name="zh-cn_topic_0201534216_p18100201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534216_p10487112"><a name="zh-cn_topic_0201534216_p10487112"></a><a name="zh-cn_topic_0201534216_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534216_row41709209"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534216_p23002745"><a name="zh-cn_topic_0201534216_p23002745"></a><a name="zh-cn_topic_0201534216_p23002745"></a>bandwidth_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534216_p51283066"><a name="zh-cn_topic_0201534216_p51283066"></a><a name="zh-cn_topic_0201534216_p51283066"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534216_p60287683"><a name="zh-cn_topic_0201534216_p60287683"></a><a name="zh-cn_topic_0201534216_p60287683"></a>带宽唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534216_section896237"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534216_table3057854815556"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534216_row6286666315556"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534216_p5903494715556"><a name="zh-cn_topic_0201534216_p5903494715556"></a><a name="zh-cn_topic_0201534216_p5903494715556"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534216_p1710139915556"><a name="zh-cn_topic_0201534216_p1710139915556"></a><a name="zh-cn_topic_0201534216_p1710139915556"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534216_p4303610815556"><a name="zh-cn_topic_0201534216_p4303610815556"></a><a name="zh-cn_topic_0201534216_p4303610815556"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534216_p6337274615556"><a name="zh-cn_topic_0201534216_p6337274615556"></a><a name="zh-cn_topic_0201534216_p6337274615556"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534216_row3291877615556"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p4917516615556"><a name="zh-cn_topic_0201534216_p4917516615556"></a><a name="zh-cn_topic_0201534216_p4917516615556"></a>bandwidth</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p2376550915556"><a name="zh-cn_topic_0201534216_p2376550915556"></a><a name="zh-cn_topic_0201534216_p2376550915556"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p4595806815556"><a name="zh-cn_topic_0201534216_p4595806815556"></a><a name="zh-cn_topic_0201534216_p4595806815556"></a><a href="#zh-cn_topic_0201534216_table31854691">bandwidth</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534216_p1610901815556"><a name="zh-cn_topic_0201534216_p1610901815556"></a><a name="zh-cn_topic_0201534216_p1610901815556"></a>带宽对象，请参见<a href="#zh-cn_topic_0201534216_table31854691">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  bandwidth字段说明

    <a name="zh-cn_topic_0201534216_table31854691"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534216_row6882862"><th class="cellrowborder" valign="top" width="13.350000000000001%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534216_p20640979"><a name="zh-cn_topic_0201534216_p20640979"></a><a name="zh-cn_topic_0201534216_p20640979"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534216_p61306625"><a name="zh-cn_topic_0201534216_p61306625"></a><a name="zh-cn_topic_0201534216_p61306625"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="13.91%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534216_p5200653172316"><a name="zh-cn_topic_0201534216_p5200653172316"></a><a name="zh-cn_topic_0201534216_p5200653172316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.830000000000005%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534216_p66889567"><a name="zh-cn_topic_0201534216_p66889567"></a><a name="zh-cn_topic_0201534216_p66889567"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534216_row49345813"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p37587916"><a name="zh-cn_topic_0201534216_p37587916"></a><a name="zh-cn_topic_0201534216_p37587916"></a>publicip_info</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p24722347"><a name="zh-cn_topic_0201534216_p24722347"></a><a name="zh-cn_topic_0201534216_p24722347"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p18599757172316"><a name="zh-cn_topic_0201534216_p18599757172316"></a><a name="zh-cn_topic_0201534216_p18599757172316"></a>Array of <a href="#zh-cn_topic_0201534216_table30936422">publicip_info</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534216_ul290995117818"></a><a name="zh-cn_topic_0201534216_ul290995117818"></a><ul id="zh-cn_topic_0201534216_ul290995117818"><li>功能说明：要从共享带宽中移除的<span id="zh-cn_topic_0201534216_text16874929201119"><a name="zh-cn_topic_0201534216_text16874929201119"></a><a name="zh-cn_topic_0201534216_text16874929201119"></a></span><span id="zh-cn_topic_0201534216_text19874112931112"><a name="zh-cn_topic_0201534216_text19874112931112"></a><a name="zh-cn_topic_0201534216_text19874112931112"></a>弹性公网IP</span>信息，请参见<a href="#zh-cn_topic_0201534216_table30936422">表4</a>。</li><li>约束：WHOLE类型的带宽支持多个<span id="zh-cn_topic_0201534216_text0160114517113"><a name="zh-cn_topic_0201534216_text0160114517113"></a><a name="zh-cn_topic_0201534216_text0160114517113"></a></span><span id="zh-cn_topic_0201534216_text5160134513116"><a name="zh-cn_topic_0201534216_text5160134513116"></a><a name="zh-cn_topic_0201534216_text5160134513116"></a>弹性公网IP</span>，跟租户的配额相关，默认一个共享带宽的配额为20。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534216_row193703372412"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p183711037154117"><a name="zh-cn_topic_0201534216_p183711037154117"></a><a name="zh-cn_topic_0201534216_p183711037154117"></a>charge_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p17371237114118"><a name="zh-cn_topic_0201534216_p17371237114118"></a><a name="zh-cn_topic_0201534216_p17371237114118"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p15371143714413"><a name="zh-cn_topic_0201534216_p15371143714413"></a><a name="zh-cn_topic_0201534216_p15371143714413"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534216_p877125719190"><a name="zh-cn_topic_0201534216_p877125719190"></a><a name="zh-cn_topic_0201534216_p877125719190"></a><span id="zh-cn_topic_0201534216_text157741850161119"><a name="zh-cn_topic_0201534216_text157741850161119"></a><a name="zh-cn_topic_0201534216_text157741850161119"></a></span><span id="zh-cn_topic_0201534216_text16774350101117"><a name="zh-cn_topic_0201534216_text16774350101117"></a><a name="zh-cn_topic_0201534216_text16774350101117"></a>弹性公网IP</span>从共享带宽移除后，会为此<span id="zh-cn_topic_0201534216_text111271558116"><a name="zh-cn_topic_0201534216_text111271558116"></a><a name="zh-cn_topic_0201534216_text111271558116"></a></span><span id="zh-cn_topic_0201534216_text19127185551113"><a name="zh-cn_topic_0201534216_text19127185551113"></a><a name="zh-cn_topic_0201534216_text19127185551113"></a>弹性公网IP</span>创建独占带宽进行计费。</p>
    <p id="zh-cn_topic_0201534216_p29217211425"><a name="zh-cn_topic_0201534216_p29217211425"></a><a name="zh-cn_topic_0201534216_p29217211425"></a>此参数表示<span id="zh-cn_topic_0201534216_text8806205914113"><a name="zh-cn_topic_0201534216_text8806205914113"></a><a name="zh-cn_topic_0201534216_text8806205914113"></a></span><span id="zh-cn_topic_0201534216_text188061359161114"><a name="zh-cn_topic_0201534216_text188061359161114"></a><a name="zh-cn_topic_0201534216_text188061359161114"></a>弹性公网IP</span>从共享带宽移除后，使用的独占带宽的计费类型。</p>
    <p id="zh-cn_topic_0201534216_p179232117423"><a name="zh-cn_topic_0201534216_p179232117423"></a><a name="zh-cn_topic_0201534216_p179232117423"></a>（bandwidth/traffic）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534216_row1125210414413"><td class="cellrowborder" valign="top" width="13.350000000000001%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p1425214412410"><a name="zh-cn_topic_0201534216_p1425214412410"></a><a name="zh-cn_topic_0201534216_p1425214412410"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p1525210418416"><a name="zh-cn_topic_0201534216_p1525210418416"></a><a name="zh-cn_topic_0201534216_p1525210418416"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="13.91%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p7252164114118"><a name="zh-cn_topic_0201534216_p7252164114118"></a><a name="zh-cn_topic_0201534216_p7252164114118"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.830000000000005%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534216_p42481825142019"><a name="zh-cn_topic_0201534216_p42481825142019"></a><a name="zh-cn_topic_0201534216_p42481825142019"></a><span id="zh-cn_topic_0201534216_text17497547122"><a name="zh-cn_topic_0201534216_text17497547122"></a><a name="zh-cn_topic_0201534216_text17497547122"></a></span><span id="zh-cn_topic_0201534216_text104979414126"><a name="zh-cn_topic_0201534216_text104979414126"></a><a name="zh-cn_topic_0201534216_text104979414126"></a>弹性公网IP</span>从共享带宽移除后，会为此<span id="zh-cn_topic_0201534216_text73282881219"><a name="zh-cn_topic_0201534216_text73282881219"></a><a name="zh-cn_topic_0201534216_text73282881219"></a></span><span id="zh-cn_topic_0201534216_text1132898201215"><a name="zh-cn_topic_0201534216_text1132898201215"></a><a name="zh-cn_topic_0201534216_text1132898201215"></a>弹性公网IP</span>创建独占带宽进行计费。</p>
    <p id="zh-cn_topic_0201534216_p16249725152011"><a name="zh-cn_topic_0201534216_p16249725152011"></a><a name="zh-cn_topic_0201534216_p16249725152011"></a>此参数表示<span id="zh-cn_topic_0201534216_text154171912181212"><a name="zh-cn_topic_0201534216_text154171912181212"></a><a name="zh-cn_topic_0201534216_text154171912181212"></a></span><span id="zh-cn_topic_0201534216_text4417191221212"><a name="zh-cn_topic_0201534216_text4417191221212"></a><a name="zh-cn_topic_0201534216_text4417191221212"></a>弹性公网IP</span>从共享带宽移除后，使用的独占带宽的带宽大小。（M）</p>
    <p id="zh-cn_topic_0201534216_p721494415220"><a name="zh-cn_topic_0201534216_p721494415220"></a><a name="zh-cn_topic_0201534216_p721494415220"></a>取值范围：默认为1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  publicip\_info对象

    <a name="zh-cn_topic_0201534216_table30936422"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534216_row17161430"><th class="cellrowborder" valign="top" width="13.3%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534216_p47898561"><a name="zh-cn_topic_0201534216_p47898561"></a><a name="zh-cn_topic_0201534216_p47898561"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.02%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534216_p157089251981"><a name="zh-cn_topic_0201534216_p157089251981"></a><a name="zh-cn_topic_0201534216_p157089251981"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.96%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534216_p2828296517154"><a name="zh-cn_topic_0201534216_p2828296517154"></a><a name="zh-cn_topic_0201534216_p2828296517154"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.72%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534216_p58761073"><a name="zh-cn_topic_0201534216_p58761073"></a><a name="zh-cn_topic_0201534216_p58761073"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534216_row62026502"><td class="cellrowborder" valign="top" width="13.3%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p58090788"><a name="zh-cn_topic_0201534216_p58090788"></a><a name="zh-cn_topic_0201534216_p58090788"></a>publicip_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p10708102514810"><a name="zh-cn_topic_0201534216_p10708102514810"></a><a name="zh-cn_topic_0201534216_p10708102514810"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p921881117154"><a name="zh-cn_topic_0201534216_p921881117154"></a><a name="zh-cn_topic_0201534216_p921881117154"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534216_p476380"><a name="zh-cn_topic_0201534216_p476380"></a><a name="zh-cn_topic_0201534216_p476380"></a>带宽对应的<span id="zh-cn_topic_0201534216_text4370119121210"><a name="zh-cn_topic_0201534216_text4370119121210"></a><a name="zh-cn_topic_0201534216_text4370119121210"></a></span><span id="zh-cn_topic_0201534216_text1537041961214"><a name="zh-cn_topic_0201534216_text1537041961214"></a><a name="zh-cn_topic_0201534216_text1537041961214"></a>弹性公网IP</span>的唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534216_row472114161816"><td class="cellrowborder" valign="top" width="13.3%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534216_p652012122440"><a name="zh-cn_topic_0201534216_p652012122440"></a><a name="zh-cn_topic_0201534216_p652012122440"></a>publicip_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534216_p10708142510820"><a name="zh-cn_topic_0201534216_p10708142510820"></a><a name="zh-cn_topic_0201534216_p10708142510820"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534216_p727719492445"><a name="zh-cn_topic_0201534216_p727719492445"></a><a name="zh-cn_topic_0201534216_p727719492445"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.72%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534216_p1752019125446"><a name="zh-cn_topic_0201534216_p1752019125446"></a><a name="zh-cn_topic_0201534216_p1752019125446"></a>若publicip_id为<span id="zh-cn_topic_0201534216_text7427152210128"><a name="zh-cn_topic_0201534216_text7427152210128"></a><a name="zh-cn_topic_0201534216_text7427152210128"></a></span><span id="zh-cn_topic_0201534216_text542716229123"><a name="zh-cn_topic_0201534216_text542716229123"></a><a name="zh-cn_topic_0201534216_text542716229123"></a>弹性公网IP</span>的id，则该字段会自动忽略。若publicip_id为IPv6端口的id，则该字段必填5_dualStack（目前仅华北-北京四支持）。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    POST https://{Endpoint}/v2.0/{project_id}/bandwidths/{bandwidth_id}/remove
    
    {
        "bandwidth": {
            "publicip_info": [
                {
                    "publicip_id": "d91b0028-6f6b-4478-808a-297b75b6812a"
     
                },
                {
                    "publicip_id": "1d184b2c-4ec9-49b5-a3f9-27600a76ba3f"
                }
            ],
            "charge_mode": "traffic",
            "size": 22
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534216_section8066134"></a>

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


## 状态码<a name="zh-cn_topic_0201534216_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534216_section85821649202813"></a>

请参考[错误码](错误码.md)。

