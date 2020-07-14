# 查询浮动IP列表<a name="eip_openstackapi_0006"></a>

## 功能介绍<a name="zh-cn_topic_0201534068_section310981132148"></a>

查询提交请求的租户有权限操作的所有浮动IP地址。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md#eip_openstackapi_0004)。

查询指定的浮动IP的详细信息，可利用[查询浮动IP](查询浮动IP.md#eip_openstackapi_0007)接口进行查询。

## URI<a name="zh-cn_topic_0201534068_section548377002148"></a>

GET /v2.0/floatingips

参数说明请参见[表1](#zh-cn_topic_0201534068_table107561756154818)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534068_table107561756154818"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534068_row167571556104810"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534068_p0685313416"><a name="zh-cn_topic_0201534068_p0685313416"></a><a name="zh-cn_topic_0201534068_p0685313416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.809999999999999%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534068_p768561134110"><a name="zh-cn_topic_0201534068_p768561134110"></a><a name="zh-cn_topic_0201534068_p768561134110"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.63%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534068_p368681134120"><a name="zh-cn_topic_0201534068_p368681134120"></a><a name="zh-cn_topic_0201534068_p368681134120"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.559999999999995%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534068_p668612124119"><a name="zh-cn_topic_0201534068_p668612124119"></a><a name="zh-cn_topic_0201534068_p668612124119"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534068_row27572562488"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p176864111411"><a name="zh-cn_topic_0201534068_p176864111411"></a><a name="zh-cn_topic_0201534068_p176864111411"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p136865110419"><a name="zh-cn_topic_0201534068_p136865110419"></a><a name="zh-cn_topic_0201534068_p136865110419"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p16861211413"><a name="zh-cn_topic_0201534068_p16861211413"></a><a name="zh-cn_topic_0201534068_p16861211413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p1068611114119"><a name="zh-cn_topic_0201534068_p1068611114119"></a><a name="zh-cn_topic_0201534068_p1068611114119"></a>浮动IP地址的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row1757105620480"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p868615164111"><a name="zh-cn_topic_0201534068_p868615164111"></a><a name="zh-cn_topic_0201534068_p868615164111"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p1468611134120"><a name="zh-cn_topic_0201534068_p1468611134120"></a><a name="zh-cn_topic_0201534068_p1468611134120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p1668716114415"><a name="zh-cn_topic_0201534068_p1668716114415"></a><a name="zh-cn_topic_0201534068_p1668716114415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p76878124112"><a name="zh-cn_topic_0201534068_p76878124112"></a><a name="zh-cn_topic_0201534068_p76878124112"></a>浮动IP地址(IPv6格式)。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row16757125613485"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p1668781104117"><a name="zh-cn_topic_0201534068_p1668781104117"></a><a name="zh-cn_topic_0201534068_p1668781104117"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p1668731204116"><a name="zh-cn_topic_0201534068_p1668731204116"></a><a name="zh-cn_topic_0201534068_p1668731204116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p1687610411"><a name="zh-cn_topic_0201534068_p1687610411"></a><a name="zh-cn_topic_0201534068_p1687610411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p14687611411"><a name="zh-cn_topic_0201534068_p14687611411"></a><a name="zh-cn_topic_0201534068_p14687611411"></a>外部网络的id。</p>
<p id="zh-cn_topic_0201534068_p4687818419"><a name="zh-cn_topic_0201534068_p4687818419"></a><a name="zh-cn_topic_0201534068_p4687818419"></a>只能使用固定的外网，外部网络的信息请通过</p>
<p id="zh-cn_topic_0201534068_p9687151144115"><a name="zh-cn_topic_0201534068_p9687151144115"></a><a name="zh-cn_topic_0201534068_p9687151144115"></a>GET /v2.0/networks?router:external=True或</p>
<p id="zh-cn_topic_0201534068_p1568711118416"><a name="zh-cn_topic_0201534068_p1568711118416"></a><a name="zh-cn_topic_0201534068_p1568711118416"></a>GET /v2.0/networks?name={floating_network}或neutron net-external-list方式查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row67574563489"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p106871419413"><a name="zh-cn_topic_0201534068_p106871419413"></a><a name="zh-cn_topic_0201534068_p106871419413"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p1268712115416"><a name="zh-cn_topic_0201534068_p1268712115416"></a><a name="zh-cn_topic_0201534068_p1268712115416"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p6687015419"><a name="zh-cn_topic_0201534068_p6687015419"></a><a name="zh-cn_topic_0201534068_p6687015419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p668714111415"><a name="zh-cn_topic_0201534068_p668714111415"></a><a name="zh-cn_topic_0201534068_p668714111415"></a>所属路由器id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row17757155634812"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p1868717104113"><a name="zh-cn_topic_0201534068_p1868717104113"></a><a name="zh-cn_topic_0201534068_p1868717104113"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p26871119419"><a name="zh-cn_topic_0201534068_p26871119419"></a><a name="zh-cn_topic_0201534068_p26871119419"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p66889116414"><a name="zh-cn_topic_0201534068_p66889116414"></a><a name="zh-cn_topic_0201534068_p66889116414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p14688213413"><a name="zh-cn_topic_0201534068_p14688213413"></a><a name="zh-cn_topic_0201534068_p14688213413"></a>端口id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row1375718561481"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p868818134116"><a name="zh-cn_topic_0201534068_p868818134116"></a><a name="zh-cn_topic_0201534068_p868818134116"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p568817111417"><a name="zh-cn_topic_0201534068_p568817111417"></a><a name="zh-cn_topic_0201534068_p568817111417"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p96881617413"><a name="zh-cn_topic_0201534068_p96881617413"></a><a name="zh-cn_topic_0201534068_p96881617413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p1668816118413"><a name="zh-cn_topic_0201534068_p1668816118413"></a><a name="zh-cn_topic_0201534068_p1668816118413"></a>关联端口的私有IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row11758105613489"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p968813113416"><a name="zh-cn_topic_0201534068_p968813113416"></a><a name="zh-cn_topic_0201534068_p968813113416"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p468815111414"><a name="zh-cn_topic_0201534068_p468815111414"></a><a name="zh-cn_topic_0201534068_p468815111414"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p12688141154119"><a name="zh-cn_topic_0201534068_p12688141154119"></a><a name="zh-cn_topic_0201534068_p12688141154119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p10487112"><a name="zh-cn_topic_0201534068_p10487112"></a><a name="zh-cn_topic_0201534068_p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row15163151102"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p19997422102"><a name="zh-cn_topic_0201534068_p19997422102"></a><a name="zh-cn_topic_0201534068_p19997422102"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p11100114281018"><a name="zh-cn_topic_0201534068_p11100114281018"></a><a name="zh-cn_topic_0201534068_p11100114281018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p1610054213103"><a name="zh-cn_topic_0201534068_p1610054213103"></a><a name="zh-cn_topic_0201534068_p1610054213103"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p5100134217101"><a name="zh-cn_topic_0201534068_p5100134217101"></a><a name="zh-cn_topic_0201534068_p5100134217101"></a>每页显示的条目数量。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row8578219101016"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p17100142191012"><a name="zh-cn_topic_0201534068_p17100142191012"></a><a name="zh-cn_topic_0201534068_p17100142191012"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p1110011422102"><a name="zh-cn_topic_0201534068_p1110011422102"></a><a name="zh-cn_topic_0201534068_p1110011422102"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p8100442111010"><a name="zh-cn_topic_0201534068_p8100442111010"></a><a name="zh-cn_topic_0201534068_p8100442111010"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p18100164214106"><a name="zh-cn_topic_0201534068_p18100164214106"></a><a name="zh-cn_topic_0201534068_p18100164214106"></a>取值为上一页数据的最后一条记录的id，当marker参数为无效id时，response将响应错误码400。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row5971723121020"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534068_p210013424100"><a name="zh-cn_topic_0201534068_p210013424100"></a><a name="zh-cn_topic_0201534068_p210013424100"></a>page_reverse</p>
</td>
<td class="cellrowborder" valign="top" width="15.809999999999999%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534068_p11008425103"><a name="zh-cn_topic_0201534068_p11008425103"></a><a name="zh-cn_topic_0201534068_p11008425103"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="16.63%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534068_p1310015428101"><a name="zh-cn_topic_0201534068_p1310015428101"></a><a name="zh-cn_topic_0201534068_p1310015428101"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="42.559999999999995%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534068_p310016420106"><a name="zh-cn_topic_0201534068_p310016420106"></a><a name="zh-cn_topic_0201534068_p310016420106"></a>False/True，是否设置分页的顺序。</p>
</td>
</tr>
</tbody>
</table>

样例：

```
GET https://{Endpoint}/v2.0/floatingips?id={fip_id}&router_id={router_id}&floating_network_id={net_id}&floating_ip_address={floating_ip}&port_id={port_id}&fixed_ip_address={fixed_ip}&tenant_id={tenant_id}
```

## 请求消息<a name="zh-cn_topic_0201534068_section656683442148"></a>

无。

## 响应消息<a name="zh-cn_topic_0201534068_section236032922148"></a>

**表 2**  响应参数

<a name="zh-cn_topic_0201534068_table328184742148"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534068_row308815332148"><th class="cellrowborder" valign="top" width="15.559999999999999%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534068_p183762202148"><a name="zh-cn_topic_0201534068_p183762202148"></a><a name="zh-cn_topic_0201534068_p183762202148"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534068_p120788402148"><a name="zh-cn_topic_0201534068_p120788402148"></a><a name="zh-cn_topic_0201534068_p120788402148"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.11%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534068_p608097322148"><a name="zh-cn_topic_0201534068_p608097322148"></a><a name="zh-cn_topic_0201534068_p608097322148"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534068_row266412852148"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p104605152148"><a name="zh-cn_topic_0201534068_p104605152148"></a><a name="zh-cn_topic_0201534068_p104605152148"></a>floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p109471238618"><a name="zh-cn_topic_0201534068_p109471238618"></a><a name="zh-cn_topic_0201534068_p109471238618"></a>Array of <a href="#zh-cn_topic_0201534068_table8139247714">floatingip</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="61.11%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p499181352148"><a name="zh-cn_topic_0201534068_p499181352148"></a><a name="zh-cn_topic_0201534068_p499181352148"></a>floatingip对象列表，参见<a href="#zh-cn_topic_0201534068_table8139247714">表3</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row5845204094319"><td class="cellrowborder" valign="top" width="15.559999999999999%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p13826463430"><a name="zh-cn_topic_0201534068_p13826463430"></a><a name="zh-cn_topic_0201534068_p13826463430"></a>floatingips_links</p>
</td>
<td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p12821546204317"><a name="zh-cn_topic_0201534068_p12821546204317"></a><a name="zh-cn_topic_0201534068_p12821546204317"></a>Array of <a href="#zh-cn_topic_0201534068_table62331111162">floatingips_link</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="61.11%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p5821246164319"><a name="zh-cn_topic_0201534068_p5821246164319"></a><a name="zh-cn_topic_0201534068_p5821246164319"></a>floatingips_link对象列表，参见<a href="#zh-cn_topic_0201534068_table62331111162">表4</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  floatingip对象

<a name="zh-cn_topic_0201534068_table8139247714"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534068_row18132240714"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534068_p101201250870"><a name="zh-cn_topic_0201534068_p101201250870"></a><a name="zh-cn_topic_0201534068_p101201250870"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534068_p161211850674"><a name="zh-cn_topic_0201534068_p161211850674"></a><a name="zh-cn_topic_0201534068_p161211850674"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534068_p41217502719"><a name="zh-cn_topic_0201534068_p41217502719"></a><a name="zh-cn_topic_0201534068_p41217502719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534068_row2014192410713"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p6028218019164"><a name="zh-cn_topic_0201534068_p6028218019164"></a><a name="zh-cn_topic_0201534068_p6028218019164"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p5101843519164"><a name="zh-cn_topic_0201534068_p5101843519164"></a><a name="zh-cn_topic_0201534068_p5101843519164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p6000412319164"><a name="zh-cn_topic_0201534068_p6000412319164"></a><a name="zh-cn_topic_0201534068_p6000412319164"></a>网络状态，可以为ACTIVE， DOWN或ERROR。</p>
<a name="zh-cn_topic_0201534068_ul10603143175810"></a><a name="zh-cn_topic_0201534068_ul10603143175810"></a><ul id="zh-cn_topic_0201534068_ul10603143175810"><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ERROR：异常</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row4141241070"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p5513524919164"><a name="zh-cn_topic_0201534068_p5513524919164"></a><a name="zh-cn_topic_0201534068_p5513524919164"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p212111505713"><a name="zh-cn_topic_0201534068_p212111505713"></a><a name="zh-cn_topic_0201534068_p212111505713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p4121850371"><a name="zh-cn_topic_0201534068_p4121850371"></a><a name="zh-cn_topic_0201534068_p4121850371"></a>浮动IP地址的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row16518828181314"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p1276893520133"><a name="zh-cn_topic_0201534068_p1276893520133"></a><a name="zh-cn_topic_0201534068_p1276893520133"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p147682350136"><a name="zh-cn_topic_0201534068_p147682350136"></a><a name="zh-cn_topic_0201534068_p147682350136"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p876820352133"><a name="zh-cn_topic_0201534068_p876820352133"></a><a name="zh-cn_topic_0201534068_p876820352133"></a>项目ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row614132416712"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p1912112509713"><a name="zh-cn_topic_0201534068_p1912112509713"></a><a name="zh-cn_topic_0201534068_p1912112509713"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p11211850072"><a name="zh-cn_topic_0201534068_p11211850072"></a><a name="zh-cn_topic_0201534068_p11211850072"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p16122205017713"><a name="zh-cn_topic_0201534068_p16122205017713"></a><a name="zh-cn_topic_0201534068_p16122205017713"></a>浮动IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row115102414717"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p61223503712"><a name="zh-cn_topic_0201534068_p61223503712"></a><a name="zh-cn_topic_0201534068_p61223503712"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p1812220507714"><a name="zh-cn_topic_0201534068_p1812220507714"></a><a name="zh-cn_topic_0201534068_p1812220507714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p16122550274"><a name="zh-cn_topic_0201534068_p16122550274"></a><a name="zh-cn_topic_0201534068_p16122550274"></a>外部网络的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row19155241277"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p201223504719"><a name="zh-cn_topic_0201534068_p201223504719"></a><a name="zh-cn_topic_0201534068_p201223504719"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p1122155015714"><a name="zh-cn_topic_0201534068_p1122155015714"></a><a name="zh-cn_topic_0201534068_p1122155015714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p812212506713"><a name="zh-cn_topic_0201534068_p812212506713"></a><a name="zh-cn_topic_0201534068_p812212506713"></a>所属路由器id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row101514247714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p412218502718"><a name="zh-cn_topic_0201534068_p412218502718"></a><a name="zh-cn_topic_0201534068_p412218502718"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p612213506716"><a name="zh-cn_topic_0201534068_p612213506716"></a><a name="zh-cn_topic_0201534068_p612213506716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p141228504716"><a name="zh-cn_topic_0201534068_p141228504716"></a><a name="zh-cn_topic_0201534068_p141228504716"></a>端口id</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row3164249715"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p01237508720"><a name="zh-cn_topic_0201534068_p01237508720"></a><a name="zh-cn_topic_0201534068_p01237508720"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p111239501770"><a name="zh-cn_topic_0201534068_p111239501770"></a><a name="zh-cn_topic_0201534068_p111239501770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p1712316501972"><a name="zh-cn_topic_0201534068_p1712316501972"></a><a name="zh-cn_topic_0201534068_p1712316501972"></a>关联端口的私有IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row21662416711"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p812355018717"><a name="zh-cn_topic_0201534068_p812355018717"></a><a name="zh-cn_topic_0201534068_p812355018717"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p612316509712"><a name="zh-cn_topic_0201534068_p612316509712"></a><a name="zh-cn_topic_0201534068_p612316509712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p1597110240277"><a name="zh-cn_topic_0201534068_p1597110240277"></a><a name="zh-cn_topic_0201534068_p1597110240277"></a>项目ID</p>
<p id="zh-cn_topic_0201534068_p51231950174"><a name="zh-cn_topic_0201534068_p51231950174"></a><a name="zh-cn_topic_0201534068_p51231950174"></a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row11176241720"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p11222111885214"><a name="zh-cn_topic_0201534068_p11222111885214"></a><a name="zh-cn_topic_0201534068_p11222111885214"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p122232018115215"><a name="zh-cn_topic_0201534068_p122232018115215"></a><a name="zh-cn_topic_0201534068_p122232018115215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p18223161825216"><a name="zh-cn_topic_0201534068_p18223161825216"></a><a name="zh-cn_topic_0201534068_p18223161825216"></a>DNS名称</p>
<p id="zh-cn_topic_0201534068_p3622189141"><a name="zh-cn_topic_0201534068_p3622189141"></a><a name="zh-cn_topic_0201534068_p3622189141"></a>该参数当前仅在“华南-广州”开放</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row17174241670"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p492133065713"><a name="zh-cn_topic_0201534068_p492133065713"></a><a name="zh-cn_topic_0201534068_p492133065713"></a>dns_domain</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p16929300573"><a name="zh-cn_topic_0201534068_p16929300573"></a><a name="zh-cn_topic_0201534068_p16929300573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p3921230175711"><a name="zh-cn_topic_0201534068_p3921230175711"></a><a name="zh-cn_topic_0201534068_p3921230175711"></a>DNS域地址</p>
<p id="zh-cn_topic_0201534068_p16100171118144"><a name="zh-cn_topic_0201534068_p16100171118144"></a><a name="zh-cn_topic_0201534068_p16100171118144"></a>该参数当前仅在“华南-广州”开放</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row1418142410714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p1953114119914"><a name="zh-cn_topic_0201534068_p1953114119914"></a><a name="zh-cn_topic_0201534068_p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p595318416919"><a name="zh-cn_topic_0201534068_p595318416919"></a><a name="zh-cn_topic_0201534068_p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p1395374115919"><a name="zh-cn_topic_0201534068_p1395374115919"></a><a name="zh-cn_topic_0201534068_p1395374115919"></a>资源创建时间</p>
<p id="zh-cn_topic_0201534068_p1232884613478"><a name="zh-cn_topic_0201534068_p1232884613478"></a><a name="zh-cn_topic_0201534068_p1232884613478"></a>采用UTC时间</p>
<p id="zh-cn_topic_0201534068_p2070141994713"><a name="zh-cn_topic_0201534068_p2070141994713"></a><a name="zh-cn_topic_0201534068_p2070141994713"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row1188246714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p139719548912"><a name="zh-cn_topic_0201534068_p139719548912"></a><a name="zh-cn_topic_0201534068_p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p53971154594"><a name="zh-cn_topic_0201534068_p53971154594"></a><a name="zh-cn_topic_0201534068_p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p1339713549918"><a name="zh-cn_topic_0201534068_p1339713549918"></a><a name="zh-cn_topic_0201534068_p1339713549918"></a>资源更新时间</p>
<p id="zh-cn_topic_0201534068_p876511114816"><a name="zh-cn_topic_0201534068_p876511114816"></a><a name="zh-cn_topic_0201534068_p876511114816"></a>采用UTC时间</p>
<p id="zh-cn_topic_0201534068_p137222218476"><a name="zh-cn_topic_0201534068_p137222218476"></a><a name="zh-cn_topic_0201534068_p137222218476"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
</tbody>
</table>

**表 4**  floatingips\_link对象

<a name="zh-cn_topic_0201534068_table62331111162"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534068_row1823611191619"><th class="cellrowborder" valign="top" width="23.122312231223123%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534068_p19231111161619"><a name="zh-cn_topic_0201534068_p19231111161619"></a><a name="zh-cn_topic_0201534068_p19231111161619"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.552555255525554%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534068_p112301121618"><a name="zh-cn_topic_0201534068_p112301121618"></a><a name="zh-cn_topic_0201534068_p112301121618"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.325132513251326%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534068_p1323611171617"><a name="zh-cn_topic_0201534068_p1323611171617"></a><a name="zh-cn_topic_0201534068_p1323611171617"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534068_row15260111169"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p192851171616"><a name="zh-cn_topic_0201534068_p192851171616"></a><a name="zh-cn_topic_0201534068_p192851171616"></a>href</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p122815111167"><a name="zh-cn_topic_0201534068_p122815111167"></a><a name="zh-cn_topic_0201534068_p122815111167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p12813117167"><a name="zh-cn_topic_0201534068_p12813117167"></a><a name="zh-cn_topic_0201534068_p12813117167"></a>API链接</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534068_row132891118162"><td class="cellrowborder" valign="top" width="23.122312231223123%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534068_p1728171118161"><a name="zh-cn_topic_0201534068_p1728171118161"></a><a name="zh-cn_topic_0201534068_p1728171118161"></a>rel</p>
</td>
<td class="cellrowborder" valign="top" width="25.552555255525554%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534068_p42820114167"><a name="zh-cn_topic_0201534068_p42820114167"></a><a name="zh-cn_topic_0201534068_p42820114167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.325132513251326%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534068_p5289119162"><a name="zh-cn_topic_0201534068_p5289119162"></a><a name="zh-cn_topic_0201534068_p5289119162"></a>API链接与该API版本的关系</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0201534068_section466100362148"></a>

请求样例

```
GET https://{Endpoint}/v2.0/floatingips?limit=1
```

响应样例

```
{
    "floatingips": [
        {
            "id": "03a9abc0-bd98-4cb1-b0bd-58dda3dfd675",
            "status": "DOWN",
            "router_id": null,
            "tenant_id": "b3292dde618e40408e30cd87455a0652",
            "project_id": "b3292dde618e40408e30cd87455a0652",
            "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
            "fixed_ip_address": null,
            "floating_ip_address": "49.4.29.131",
            "port_id": null,
            "created_at": "2020-04-21T13:22:15",
            "updated_at": "2020-04-21T13:22:17"
        }
    ],
    "floatingips_links": [
        {
            "href": "https://vpc.cn-north-1.myhuaweicloud.com/v2.0/floatingips?limit=1&marker=03a9abc0-bd98-4cb1-b0bd-58dda3dfd675",
            "rel": "next"
        },
        {
            "href": "https://vpc.cn-north-1.myhuaweicloud.com/v2.0/floatingips?limit=1&marker=03a9abc0-bd98-4cb1-b0bd-58dda3dfd675&page_reverse=true",
            "rel": "previous"
        }
    ]
}
```

## 状态码<a name="zh-cn_topic_0201534068_section10470352390"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534068_section85821649202813"></a>

请参见[错误码](错误码.md)。

