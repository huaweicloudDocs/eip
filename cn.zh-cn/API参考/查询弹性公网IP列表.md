# 查询弹性公网IP列表<a name="eip_api_0003"></a>

## 功能介绍<a name="zh-cn_topic_0201534309_section52618256"></a>

查询弹性公网IP列表。

## 调试<a name="zh-cn_topic_0201534309_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&version=v2&api=ListPublicips)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0201534309_section3802258"></a>

GET /v1/\{project\_id\}/publicips

参数说明请参见[表1](#zh-cn_topic_0201534309_table51200735)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534309_table51200735"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534309_row8909633"><th class="cellrowborder" valign="top" width="22.757724227577242%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534309_p50591634"><a name="zh-cn_topic_0201534309_p50591634"></a><a name="zh-cn_topic_0201534309_p50591634"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.598840115988402%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534309_p4281684"><a name="zh-cn_topic_0201534309_p4281684"></a><a name="zh-cn_topic_0201534309_p4281684"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.13848615138486%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534309_p2939873918724"><a name="zh-cn_topic_0201534309_p2939873918724"></a><a name="zh-cn_topic_0201534309_p2939873918724"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.50494950504949%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534309_p11272110"><a name="zh-cn_topic_0201534309_p11272110"></a><a name="zh-cn_topic_0201534309_p11272110"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534309_row40625737"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p2350413"><a name="zh-cn_topic_0201534309_p2350413"></a><a name="zh-cn_topic_0201534309_p2350413"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p56165728"><a name="zh-cn_topic_0201534309_p56165728"></a><a name="zh-cn_topic_0201534309_p56165728"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p3248766718724"><a name="zh-cn_topic_0201534309_p3248766718724"></a><a name="zh-cn_topic_0201534309_p3248766718724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p10487112"><a name="zh-cn_topic_0201534309_p10487112"></a><a name="zh-cn_topic_0201534309_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row8409368"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p10070188"><a name="zh-cn_topic_0201534309_p10070188"></a><a name="zh-cn_topic_0201534309_p10070188"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p10378893"><a name="zh-cn_topic_0201534309_p10378893"></a><a name="zh-cn_topic_0201534309_p10378893"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p1425535118724"><a name="zh-cn_topic_0201534309_p1425535118724"></a><a name="zh-cn_topic_0201534309_p1425535118724"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p28526205175853"><a name="zh-cn_topic_0201534309_p28526205175853"></a><a name="zh-cn_topic_0201534309_p28526205175853"></a>分页查询的起始资源ID，表示从指定资源的下一条记录开始查询。</p>
<p id="zh-cn_topic_0201534309_p538818488578"><a name="zh-cn_topic_0201534309_p538818488578"></a><a name="zh-cn_topic_0201534309_p538818488578"></a>marker需要和limit配合使用：</p>
<a name="zh-cn_topic_0201534309_ul12704811125810"></a><a name="zh-cn_topic_0201534309_ul12704811125810"></a><ul id="zh-cn_topic_0201534309_ul12704811125810"><li>若不传入marker和limit参数，查询结果返回全部资源记录。</li><li>若不传入marker参数，limit为10，查询结果返回第1~10条资源记录。</li><li>若marker为第10条记录的资源ID，limit为10，查询结果返回第11~20条资源记录。</li><li>若marker为第10条记录的资源ID，不传入limit参数，查询结果返回第11条及之后的所有资源记录。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row25110514"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p20685786"><a name="zh-cn_topic_0201534309_p20685786"></a><a name="zh-cn_topic_0201534309_p20685786"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p64935954"><a name="zh-cn_topic_0201534309_p64935954"></a><a name="zh-cn_topic_0201534309_p64935954"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p1383277618724"><a name="zh-cn_topic_0201534309_p1383277618724"></a><a name="zh-cn_topic_0201534309_p1383277618724"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p2017153116589"><a name="zh-cn_topic_0201534309_p2017153116589"></a><a name="zh-cn_topic_0201534309_p2017153116589"></a>分页查询每页返回的记录个数，取值范围为0~intmax。</p>
<p id="zh-cn_topic_0201534309_p125192338584"><a name="zh-cn_topic_0201534309_p125192338584"></a><a name="zh-cn_topic_0201534309_p125192338584"></a>limit需要和marker配合使用，详细规则请见marker的参数说明。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row1508191624314"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p388332415436"><a name="zh-cn_topic_0201534309_p388332415436"></a><a name="zh-cn_topic_0201534309_p388332415436"></a>ip_version</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p4883162416438"><a name="zh-cn_topic_0201534309_p4883162416438"></a><a name="zh-cn_topic_0201534309_p4883162416438"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p208831024134318"><a name="zh-cn_topic_0201534309_p208831024134318"></a><a name="zh-cn_topic_0201534309_p208831024134318"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p1388342494310"><a name="zh-cn_topic_0201534309_p1388342494310"></a><a name="zh-cn_topic_0201534309_p1388342494310"></a>IP地址版本信息</p>
<a name="zh-cn_topic_0201534309_ul451413191236"></a><a name="zh-cn_topic_0201534309_ul451413191236"></a><ul id="zh-cn_topic_0201534309_ul451413191236"><li>4：IPv4</li><li>6：IPv6</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row13633172111266"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p55289571029"><a name="zh-cn_topic_0201534309_p55289571029"></a><a name="zh-cn_topic_0201534309_p55289571029"></a>enterprise_project_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p15529457128"><a name="zh-cn_topic_0201534309_p15529457128"></a><a name="zh-cn_topic_0201534309_p15529457128"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p165291857925"><a name="zh-cn_topic_0201534309_p165291857925"></a><a name="zh-cn_topic_0201534309_p165291857925"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534309_ul152391731105011"></a><a name="zh-cn_topic_0201534309_ul152391731105011"></a><ul id="zh-cn_topic_0201534309_ul152391731105011"><li>功能说明：企业项目ID。可以使用该字段过滤某个企业项目下的<span id="zh-cn_topic_0201534309_text38025321986"><a name="zh-cn_topic_0201534309_text38025321986"></a><a name="zh-cn_topic_0201534309_text38025321986"></a></span><span id="zh-cn_topic_0201534309_text18021328811"><a name="zh-cn_topic_0201534309_text18021328811"></a><a name="zh-cn_topic_0201534309_text18021328811"></a>弹性公网IP</span>。</li><li>取值范围：最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。“0”表示默认企业项目。若需要查询当前用户所有企业项目绑定的弹性公网IP，请传参<strong id="zh-cn_topic_0201534309_b185061540163015"><a name="zh-cn_topic_0201534309_b185061540163015"></a><a name="zh-cn_topic_0201534309_b185061540163015"></a>all_granted_eps</strong>。</li></ul>
<div class="note" id="zh-cn_topic_0201534309_note19041412125118"><a name="zh-cn_topic_0201534309_note19041412125118"></a><a name="zh-cn_topic_0201534309_note19041412125118"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row18892171262518"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p1019931162613"><a name="zh-cn_topic_0201534309_p1019931162613"></a><a name="zh-cn_topic_0201534309_p1019931162613"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p18201231192618"><a name="zh-cn_topic_0201534309_p18201231192618"></a><a name="zh-cn_topic_0201534309_p18201231192618"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p172018317262"><a name="zh-cn_topic_0201534309_p172018317262"></a><a name="zh-cn_topic_0201534309_p172018317262"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p8203311261"><a name="zh-cn_topic_0201534309_p8203311261"></a><a name="zh-cn_topic_0201534309_p8203311261"></a>绑定弹性公网IP的端口id</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row83596161253"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p1120831122616"><a name="zh-cn_topic_0201534309_p1120831122616"></a><a name="zh-cn_topic_0201534309_p1120831122616"></a>public_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p2020131102613"><a name="zh-cn_topic_0201534309_p2020131102613"></a><a name="zh-cn_topic_0201534309_p2020131102613"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p22011312267"><a name="zh-cn_topic_0201534309_p22011312267"></a><a name="zh-cn_topic_0201534309_p22011312267"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p1201031162614"><a name="zh-cn_topic_0201534309_p1201031162614"></a><a name="zh-cn_topic_0201534309_p1201031162614"></a>IPv4时是申请到的弹性公网IP地址，IPv6时是IPv6地址对应的IPv4地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row537621910258"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p122083119267"><a name="zh-cn_topic_0201534309_p122083119267"></a><a name="zh-cn_topic_0201534309_p122083119267"></a>private_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p9201231112617"><a name="zh-cn_topic_0201534309_p9201231112617"></a><a name="zh-cn_topic_0201534309_p9201231112617"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p62013152613"><a name="zh-cn_topic_0201534309_p62013152613"></a><a name="zh-cn_topic_0201534309_p62013152613"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534309_ul72111312262"></a><a name="zh-cn_topic_0201534309_ul72111312262"></a><ul id="zh-cn_topic_0201534309_ul72111312262"><li>功能说明：绑定弹性公网IP的私有IP地址</li><li>约束：只有绑定了的弹性公网IP才会有该参数</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0201534309_row4466132218255"><td class="cellrowborder" valign="top" width="22.757724227577242%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534309_p1321133162612"><a name="zh-cn_topic_0201534309_p1321133162612"></a><a name="zh-cn_topic_0201534309_p1321133162612"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="11.598840115988402%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534309_p821133116269"><a name="zh-cn_topic_0201534309_p821133116269"></a><a name="zh-cn_topic_0201534309_p821133116269"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.13848615138486%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534309_p121331182614"><a name="zh-cn_topic_0201534309_p121331182614"></a><a name="zh-cn_topic_0201534309_p121331182614"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="50.50494950504949%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534309_p6211331102610"><a name="zh-cn_topic_0201534309_p6211331102610"></a><a name="zh-cn_topic_0201534309_p6211331102610"></a>弹性公网IP唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534309_section34220326"></a>

-   请求参数

    无

-   请求样例

    ```
    GET https://{Endpoint}/v1/{project_id}/publicips?limit={limit}&marker={marker}
    ```


## 响应消息<a name="zh-cn_topic_0201534309_section39547486"></a>

-   响应参数

    **表 2**  响应参数

    <a name="zh-cn_topic_0201534309_table22603002152149"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534309_row30843029152149"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534309_p15257431152149"><a name="zh-cn_topic_0201534309_p15257431152149"></a><a name="zh-cn_topic_0201534309_p15257431152149"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534309_p44693705152149"><a name="zh-cn_topic_0201534309_p44693705152149"></a><a name="zh-cn_topic_0201534309_p44693705152149"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534309_p63420361152149"><a name="zh-cn_topic_0201534309_p63420361152149"></a><a name="zh-cn_topic_0201534309_p63420361152149"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534309_row36775597152149"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p26033374152149"><a name="zh-cn_topic_0201534309_p26033374152149"></a><a name="zh-cn_topic_0201534309_p26033374152149"></a>publicips</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p746714339186"><a name="zh-cn_topic_0201534309_p746714339186"></a><a name="zh-cn_topic_0201534309_p746714339186"></a>Array of <a href="#zh-cn_topic_0201534309_table83964341880">publicips</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p14951203152149"><a name="zh-cn_topic_0201534309_p14951203152149"></a><a name="zh-cn_topic_0201534309_p14951203152149"></a><span id="zh-cn_topic_0201534309_text54783315327"><a name="zh-cn_topic_0201534309_text54783315327"></a><a name="zh-cn_topic_0201534309_text54783315327"></a></span><span id="zh-cn_topic_0201534309_text34793343219"><a name="zh-cn_topic_0201534309_text34793343219"></a><a name="zh-cn_topic_0201534309_text34793343219"></a>弹性公网IP</span>列表对象，请参见<a href="#zh-cn_topic_0201534309_table83964341880">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicips字段说明

    <a name="zh-cn_topic_0201534309_table83964341880"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534309_row608739661880"><th class="cellrowborder" valign="top" width="17.958204179582044%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534309_p318442431880"><a name="zh-cn_topic_0201534309_p318442431880"></a><a name="zh-cn_topic_0201534309_p318442431880"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.82741725827417%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534309_p201897271880"><a name="zh-cn_topic_0201534309_p201897271880"></a><a name="zh-cn_topic_0201534309_p201897271880"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.214378562143786%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534309_p247551571880"><a name="zh-cn_topic_0201534309_p247551571880"></a><a name="zh-cn_topic_0201534309_p247551571880"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534309_row590107001880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p151373871880"><a name="zh-cn_topic_0201534309_p151373871880"></a><a name="zh-cn_topic_0201534309_p151373871880"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p623914921880"><a name="zh-cn_topic_0201534309_p623914921880"></a><a name="zh-cn_topic_0201534309_p623914921880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p205460611880"><a name="zh-cn_topic_0201534309_p205460611880"></a><a name="zh-cn_topic_0201534309_p205460611880"></a><span id="zh-cn_topic_0201534309_text760720883219"><a name="zh-cn_topic_0201534309_text760720883219"></a><a name="zh-cn_topic_0201534309_text760720883219"></a></span><span id="zh-cn_topic_0201534309_text106072817328"><a name="zh-cn_topic_0201534309_text106072817328"></a><a name="zh-cn_topic_0201534309_text106072817328"></a>弹性公网IP</span>唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row506968211880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p128018091880"><a name="zh-cn_topic_0201534309_p128018091880"></a><a name="zh-cn_topic_0201534309_p128018091880"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p394853281880"><a name="zh-cn_topic_0201534309_p394853281880"></a><a name="zh-cn_topic_0201534309_p394853281880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul263945115243"></a><a name="zh-cn_topic_0201534309_ul263945115243"></a><ul id="zh-cn_topic_0201534309_ul263945115243"><li>功能说明：<span id="zh-cn_topic_0201534309_text11500313183219"><a name="zh-cn_topic_0201534309_text11500313183219"></a><a name="zh-cn_topic_0201534309_text11500313183219"></a></span><span id="zh-cn_topic_0201534309_text750041313321"><a name="zh-cn_topic_0201534309_text750041313321"></a><a name="zh-cn_topic_0201534309_text750041313321"></a>弹性公网IP</span>的状态</li><li>取值范围：<a name="zh-cn_topic_0201534309_ul7905205815810"></a><a name="zh-cn_topic_0201534309_ul7905205815810"></a><ul id="zh-cn_topic_0201534309_ul7905205815810"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row16130133562319"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p09743162419"><a name="zh-cn_topic_0201534309_p09743162419"></a><a name="zh-cn_topic_0201534309_p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p12971231132410"><a name="zh-cn_topic_0201534309_p12971231132410"></a><a name="zh-cn_topic_0201534309_p12971231132410"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p5644118182514"><a name="zh-cn_topic_0201534309_p5644118182514"></a><a name="zh-cn_topic_0201534309_p5644118182514"></a>功能说明：额外参数，包括订单id、产品id等信息，详情请参见<a href="#zh-cn_topic_0201534309_table66651219193417">表4</a>。</p>
    <p id="zh-cn_topic_0201534309_p16644118152519"><a name="zh-cn_topic_0201534309_p16644118152519"></a><a name="zh-cn_topic_0201534309_p16644118152519"></a>约束：如果profile不为空，说明是包周期的<span id="zh-cn_topic_0201534309_text1887940143217"><a name="zh-cn_topic_0201534309_text1887940143217"></a><a name="zh-cn_topic_0201534309_text1887940143217"></a></span><span id="zh-cn_topic_0201534309_text5887940103217"><a name="zh-cn_topic_0201534309_text5887940103217"></a><a name="zh-cn_topic_0201534309_text5887940103217"></a>弹性公网IP</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row230260811880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p30749271"><a name="zh-cn_topic_0201534309_p30749271"></a><a name="zh-cn_topic_0201534309_p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p379401841880"><a name="zh-cn_topic_0201534309_p379401841880"></a><a name="zh-cn_topic_0201534309_p379401841880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul7176216121014"></a><a name="zh-cn_topic_0201534309_ul7176216121014"></a><ul id="zh-cn_topic_0201534309_ul7176216121014"><li>功能说明：<span id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text941224173012"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text941224173012"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text941224173012"></a></span><span id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4412641113015"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4412641113015"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4412641113015"></a>弹性公网IP</span>的类型</li><li>取值范围：<em id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i16850184017499"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i16850184017499"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul585004064911"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul585004064911"></a><ul id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：<em id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i541911467911"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i541911467911"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_i541911467911"></a>5_bgp</em>、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li><span id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4018327273"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4018327273"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_text4018327273"></a>中国-香港</span>：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul9738153015499"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul9738153015499"></a><ul id="zh-cn_topic_0201534309_zh-cn_topic_0201534274_ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row389218135338"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p59108624"><a name="zh-cn_topic_0201534309_p59108624"></a><a name="zh-cn_topic_0201534309_p59108624"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p904808818330"><a name="zh-cn_topic_0201534309_p904808818330"></a><a name="zh-cn_topic_0201534309_p904808818330"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p40237373"><a name="zh-cn_topic_0201534309_p40237373"></a><a name="zh-cn_topic_0201534309_p40237373"></a>IPv4时是申请到的<span id="zh-cn_topic_0201534309_text7258172943415"><a name="zh-cn_topic_0201534309_text7258172943415"></a><a name="zh-cn_topic_0201534309_text7258172943415"></a></span><span id="zh-cn_topic_0201534309_text0258152915349"><a name="zh-cn_topic_0201534309_text0258152915349"></a><a name="zh-cn_topic_0201534309_text0258152915349"></a>弹性公网IP</span>地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row6663943910"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p117521510894"><a name="zh-cn_topic_0201534309_p117521510894"></a><a name="zh-cn_topic_0201534309_p117521510894"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p97524108911"><a name="zh-cn_topic_0201534309_p97524108911"></a><a name="zh-cn_topic_0201534309_p97524108911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p167581149102812"><a name="zh-cn_topic_0201534309_p167581149102812"></a><a name="zh-cn_topic_0201534309_p167581149102812"></a>IPv4时无此字段，IPv6时为申请到的<span id="zh-cn_topic_0201534309_text7222333123416"><a name="zh-cn_topic_0201534309_text7222333123416"></a><a name="zh-cn_topic_0201534309_text7222333123416"></a></span><span id="zh-cn_topic_0201534309_text222218331342"><a name="zh-cn_topic_0201534309_text222218331342"></a><a name="zh-cn_topic_0201534309_text222218331342"></a>弹性公网IP</span>地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row2030210714336"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p171101456172118"><a name="zh-cn_topic_0201534309_p171101456172118"></a><a name="zh-cn_topic_0201534309_p171101456172118"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p1811012569218"><a name="zh-cn_topic_0201534309_p1811012569218"></a><a name="zh-cn_topic_0201534309_p1811012569218"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p10645141832513"><a name="zh-cn_topic_0201534309_p10645141832513"></a><a name="zh-cn_topic_0201534309_p10645141832513"></a>IP版本信息，取值范围是4和6</p>
    <a name="zh-cn_topic_0201534309_ul13987110227"></a><a name="zh-cn_topic_0201534309_ul13987110227"></a><ul id="zh-cn_topic_0201534309_ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row283940631880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p182177951880"><a name="zh-cn_topic_0201534309_p182177951880"></a><a name="zh-cn_topic_0201534309_p182177951880"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p60695041880"><a name="zh-cn_topic_0201534309_p60695041880"></a><a name="zh-cn_topic_0201534309_p60695041880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul1693412582014"></a><a name="zh-cn_topic_0201534309_ul1693412582014"></a><ul id="zh-cn_topic_0201534309_ul1693412582014"><li>功能说明：绑定<span id="zh-cn_topic_0201534309_text183334421342"><a name="zh-cn_topic_0201534309_text183334421342"></a><a name="zh-cn_topic_0201534309_text183334421342"></a></span><span id="zh-cn_topic_0201534309_text10333842193417"><a name="zh-cn_topic_0201534309_text10333842193417"></a><a name="zh-cn_topic_0201534309_text10333842193417"></a>弹性公网IP</span>的私有IP地址</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534309_text6408174583415"><a name="zh-cn_topic_0201534309_text6408174583415"></a><a name="zh-cn_topic_0201534309_text6408174583415"></a></span><span id="zh-cn_topic_0201534309_text1540817456342"><a name="zh-cn_topic_0201534309_text1540817456342"></a><a name="zh-cn_topic_0201534309_text1540817456342"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row264614551880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p630030811880"><a name="zh-cn_topic_0201534309_p630030811880"></a><a name="zh-cn_topic_0201534309_p630030811880"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p397229231880"><a name="zh-cn_topic_0201534309_p397229231880"></a><a name="zh-cn_topic_0201534309_p397229231880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul420471472010"></a><a name="zh-cn_topic_0201534309_ul420471472010"></a><ul id="zh-cn_topic_0201534309_ul420471472010"><li>功能说明：端口id。</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534309_text128031349183419"><a name="zh-cn_topic_0201534309_text128031349183419"></a><a name="zh-cn_topic_0201534309_text128031349183419"></a></span><span id="zh-cn_topic_0201534309_text17803749123411"><a name="zh-cn_topic_0201534309_text17803749123411"></a><a name="zh-cn_topic_0201534309_text17803749123411"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row340905521880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p98713501880"><a name="zh-cn_topic_0201534309_p98713501880"></a><a name="zh-cn_topic_0201534309_p98713501880"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p58747301880"><a name="zh-cn_topic_0201534309_p58747301880"></a><a name="zh-cn_topic_0201534309_p58747301880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p19867509217"><a name="zh-cn_topic_0201534309_p19867509217"></a><a name="zh-cn_topic_0201534309_p19867509217"></a>项目ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row548200921880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p112424711880"><a name="zh-cn_topic_0201534309_p112424711880"></a><a name="zh-cn_topic_0201534309_p112424711880"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p92119381880"><a name="zh-cn_topic_0201534309_p92119381880"></a><a name="zh-cn_topic_0201534309_p92119381880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p36292894"><a name="zh-cn_topic_0201534309_p36292894"></a><a name="zh-cn_topic_0201534309_p36292894"></a><span id="zh-cn_topic_0201534309_text2913115243410"><a name="zh-cn_topic_0201534309_text2913115243410"></a><a name="zh-cn_topic_0201534309_text2913115243410"></a></span><span id="zh-cn_topic_0201534309_text9913135213419"><a name="zh-cn_topic_0201534309_text9913135213419"></a><a name="zh-cn_topic_0201534309_text9913135213419"></a>弹性公网IP</span>申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row46164031880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p383843571880"><a name="zh-cn_topic_0201534309_p383843571880"></a><a name="zh-cn_topic_0201534309_p383843571880"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p473107141880"><a name="zh-cn_topic_0201534309_p473107141880"></a><a name="zh-cn_topic_0201534309_p473107141880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p3934181618641"><a name="zh-cn_topic_0201534309_p3934181618641"></a><a name="zh-cn_topic_0201534309_p3934181618641"></a><span id="zh-cn_topic_0201534309_text5294205510349"><a name="zh-cn_topic_0201534309_text5294205510349"></a><a name="zh-cn_topic_0201534309_text5294205510349"></a></span><span id="zh-cn_topic_0201534309_text18294195515344"><a name="zh-cn_topic_0201534309_text18294195515344"></a><a name="zh-cn_topic_0201534309_text18294195515344"></a>弹性公网IP</span>对应带宽ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row626637421880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p425983371880"><a name="zh-cn_topic_0201534309_p425983371880"></a><a name="zh-cn_topic_0201534309_p425983371880"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p463832691880"><a name="zh-cn_topic_0201534309_p463832691880"></a><a name="zh-cn_topic_0201534309_p463832691880"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p2365466"><a name="zh-cn_topic_0201534309_p2365466"></a><a name="zh-cn_topic_0201534309_p2365466"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row576448061880"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p387177161880"><a name="zh-cn_topic_0201534309_p387177161880"></a><a name="zh-cn_topic_0201534309_p387177161880"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p21369006155933"><a name="zh-cn_topic_0201534309_p21369006155933"></a><a name="zh-cn_topic_0201534309_p21369006155933"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul2255712095"></a><a name="zh-cn_topic_0201534309_ul2255712095"></a><ul id="zh-cn_topic_0201534309_ul2255712095"><li>功能说明：<span id="zh-cn_topic_0201534309_text183860582343"><a name="zh-cn_topic_0201534309_text183860582343"></a><a name="zh-cn_topic_0201534309_text183860582343"></a></span><span id="zh-cn_topic_0201534309_text4387145833414"><a name="zh-cn_topic_0201534309_text4387145833414"></a><a name="zh-cn_topic_0201534309_text4387145833414"></a>弹性公网IP</span>的带宽类型</li><li>取值范围：PER，WHOLE。<a name="zh-cn_topic_0201534309_ul729412507220"></a><a name="zh-cn_topic_0201534309_ul729412507220"></a><ul id="zh-cn_topic_0201534309_ul729412507220"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    <a name="zh-cn_topic_0201534309_ul1369035014203"></a><a name="zh-cn_topic_0201534309_ul1369035014203"></a><ul id="zh-cn_topic_0201534309_ul1369035014203"><li>约束：其中IPv6暂不支持WHOLE类型带宽。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row1444049321927"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p605297721941"><a name="zh-cn_topic_0201534309_p605297721941"></a><a name="zh-cn_topic_0201534309_p605297721941"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p5224891921941"><a name="zh-cn_topic_0201534309_p5224891921941"></a><a name="zh-cn_topic_0201534309_p5224891921941"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p374970718414"><a name="zh-cn_topic_0201534309_p374970718414"></a><a name="zh-cn_topic_0201534309_p374970718414"></a>带宽名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row10731123594017"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p979842771215"><a name="zh-cn_topic_0201534309_p979842771215"></a><a name="zh-cn_topic_0201534309_p979842771215"></a>alias</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p137987278128"><a name="zh-cn_topic_0201534309_p137987278128"></a><a name="zh-cn_topic_0201534309_p137987278128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p175531744191218"><a name="zh-cn_topic_0201534309_p175531744191218"></a><a name="zh-cn_topic_0201534309_p175531744191218"></a>弹性公网IP名称</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row1353343333617"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p19564181313543"><a name="zh-cn_topic_0201534309_p19564181313543"></a><a name="zh-cn_topic_0201534309_p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p13564413185412"><a name="zh-cn_topic_0201534309_p13564413185412"></a><a name="zh-cn_topic_0201534309_p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul184004104214"></a><a name="zh-cn_topic_0201534309_ul184004104214"></a><ul id="zh-cn_topic_0201534309_ul184004104214"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li><li>不指定该参数时，默认值是 0，0表示默认企业项目。</li></ul>
    <div class="note" id="zh-cn_topic_0201534309_note996111134561"><a name="zh-cn_topic_0201534309_note996111134561"></a><a name="zh-cn_topic_0201534309_note996111134561"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914_1"><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914_1"></a><a name="zh-cn_topic_0201534309_zh-cn_topic_0201534275_p1915862704914_1"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row17854131416221"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p1388313292268"><a name="zh-cn_topic_0201534309_p1388313292268"></a><a name="zh-cn_topic_0201534309_p1388313292268"></a>public_border_group</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p118831329122611"><a name="zh-cn_topic_0201534309_p118831329122611"></a><a name="zh-cn_topic_0201534309_p118831329122611"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p29889336324"><a name="zh-cn_topic_0201534309_p29889336324"></a><a name="zh-cn_topic_0201534309_p29889336324"></a>功能说明：表示中心站点资源或者边缘站点资源，对接了边缘站点的区域才会返回此字段</p>
    <p id="zh-cn_topic_0201534309_p20127195053611"><a name="zh-cn_topic_0201534309_p20127195053611"></a><a name="zh-cn_topic_0201534309_p20127195053611"></a>取值范围：</p>
    <a name="zh-cn_topic_0201534309_ul1660185933618"></a><a name="zh-cn_topic_0201534309_ul1660185933618"></a><ul id="zh-cn_topic_0201534309_ul1660185933618"><li>center</li><li>边缘站点名称</li></ul>
    <p id="zh-cn_topic_0201534309_p65761507386"><a name="zh-cn_topic_0201534309_p65761507386"></a><a name="zh-cn_topic_0201534309_p65761507386"></a>约束限制：只能绑定与该字段相同的publicip资源</p>
    <a name="zh-cn_topic_0201534309_ul16116154317382"></a><a name="zh-cn_topic_0201534309_ul16116154317382"></a>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row4216111318117"><td class="cellrowborder" valign="top" width="17.958204179582044%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p17216171341115"><a name="zh-cn_topic_0201534309_p17216171341115"></a><a name="zh-cn_topic_0201534309_p17216171341115"></a>allow_share_bandwidth_types</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p13216141361114"><a name="zh-cn_topic_0201534309_p13216141361114"></a><a name="zh-cn_topic_0201534309_p13216141361114"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.214378562143786%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534309_ul1756619360147"></a><a name="zh-cn_topic_0201534309_ul1756619360147"></a><ul id="zh-cn_topic_0201534309_ul1756619360147"><li>功能说明：表示此publicip可以加入的共享带宽类型列表。</li><li>如果列表为空，表示该publicip不能加入任何共享带宽。</li><li>约束：publicip只能加入到有该带宽类型的共享带宽中。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  profile字段说明

    <a name="zh-cn_topic_0201534309_table66651219193417"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534309_row167319197349"><th class="cellrowborder" valign="top" width="18.360000000000003%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534309_p206761195347"><a name="zh-cn_topic_0201534309_p206761195347"></a><a name="zh-cn_topic_0201534309_p206761195347"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.66%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534309_p156812193344"><a name="zh-cn_topic_0201534309_p156812193344"></a><a name="zh-cn_topic_0201534309_p156812193344"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.98%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534309_p17684101933410"><a name="zh-cn_topic_0201534309_p17684101933410"></a><a name="zh-cn_topic_0201534309_p17684101933410"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534309_row962259102216"><td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p962309182220"><a name="zh-cn_topic_0201534309_p962309182220"></a><a name="zh-cn_topic_0201534309_p962309182220"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p136231597223"><a name="zh-cn_topic_0201534309_p136231597223"></a><a name="zh-cn_topic_0201534309_p136231597223"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p26235912225"><a name="zh-cn_topic_0201534309_p26235912225"></a><a name="zh-cn_topic_0201534309_p26235912225"></a>订单的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row18686141920341"><td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p11688201923418"><a name="zh-cn_topic_0201534309_p11688201923418"></a><a name="zh-cn_topic_0201534309_p11688201923418"></a>product_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p169318196347"><a name="zh-cn_topic_0201534309_p169318196347"></a><a name="zh-cn_topic_0201534309_p169318196347"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p149921832153419"><a name="zh-cn_topic_0201534309_p149921832153419"></a><a name="zh-cn_topic_0201534309_p149921832153419"></a>产品的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row167161319173418"><td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p5718101903412"><a name="zh-cn_topic_0201534309_p5718101903412"></a><a name="zh-cn_topic_0201534309_p5718101903412"></a>region_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p47241019143417"><a name="zh-cn_topic_0201534309_p47241019143417"></a><a name="zh-cn_topic_0201534309_p47241019143417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p09201951174716"><a name="zh-cn_topic_0201534309_p09201951174716"></a><a name="zh-cn_topic_0201534309_p09201951174716"></a>region的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534309_row1472971912347"><td class="cellrowborder" valign="top" width="18.360000000000003%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534309_p187311719103415"><a name="zh-cn_topic_0201534309_p187311719103415"></a><a name="zh-cn_topic_0201534309_p187311719103415"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.66%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534309_p9735141923418"><a name="zh-cn_topic_0201534309_p9735141923418"></a><a name="zh-cn_topic_0201534309_p9735141923418"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.98%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534309_p27381919173415"><a name="zh-cn_topic_0201534309_p27381919173415"></a><a name="zh-cn_topic_0201534309_p27381919173415"></a>用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "publicips": [
            {
                "id": "6285e7be-fd9f-497c-bc2d-dd0bdea6efe0",
                "status": "DOWN",
                "profile": {
                  "user_id": "35f2b308f5d64441a6fa7999fbcd4321",
                  "product_id": "00301-48027-0--0",
                  "region_id": "xxx",
                  "order_id": "xxxxxxxxx"
                },
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.9",
                "private_ip_address": "192.168.10.5",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:22:32",
                "bandwidth_id": "3fa5b383-5a73-4dcb-a314-c6128546d855",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                "bandwidth_name": "bandwidth-test",
                "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439",
                "ip_version": 4
            },
            {
                "id": "80d5b82e-43b9-4f82-809a-37bec5793bd4",
                "status": "DOWN",              "user_id": null,
                "type": "5_bgp",
                "public_ip_address": "161.xx.xx.10",
                "private_ip_address": "192.168.10.6",
                "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c",
                "create_time": "2015-07-16 04:23:03",
                "bandwidth_id": "a79fd11a-047b-4f5b-8f12-99c178cc780a",
                "bandwidth_share_type": "PER",
                "bandwidth_size": 5,
                "bandwidth_name": "bandwidth-test1",
                "enterprise_project_id":"0",
                "ip_version": 4
            }
        ]
    }
    ```


## 状态码<a name="zh-cn_topic_0201534309_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534309_section85821649202813"></a>

请参考[错误码](错误码.md)。

