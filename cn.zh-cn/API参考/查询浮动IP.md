# 查询浮动IP<a name="eip_openstackapi_0007"></a>

## 功能介绍<a name="zh-cn_topic_0201534072_section433032482159"></a>

该接口用于查询指定浮动IP详情，包括浮动IP状态，浮动IP所属路由器ID，浮动IP的外部网络ID等等。

## URI<a name="zh-cn_topic_0201534072_section269019862159"></a>

GET /v2.0/floatingips/\{floatingip\_id\}

## 请求消息<a name="zh-cn_topic_0201534072_section513321362159"></a>

无。

## 响应消息<a name="zh-cn_topic_0201534072_section414903182159"></a>

**表 1**  响应参数

<a name="zh-cn_topic_0201534072_table52726292159"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534072_row483206142159"><th class="cellrowborder" valign="top" width="21.349999999999998%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534072_p216556632159"><a name="zh-cn_topic_0201534072_p216556632159"></a><a name="zh-cn_topic_0201534072_p216556632159"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="8.99%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534072_p92783132159"><a name="zh-cn_topic_0201534072_p92783132159"></a><a name="zh-cn_topic_0201534072_p92783132159"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="69.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534072_p72773912159"><a name="zh-cn_topic_0201534072_p72773912159"></a><a name="zh-cn_topic_0201534072_p72773912159"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534072_row525977702159"><td class="cellrowborder" valign="top" width="21.349999999999998%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p325609822159"><a name="zh-cn_topic_0201534072_p325609822159"></a><a name="zh-cn_topic_0201534072_p325609822159"></a>floatingip</p>
</td>
<td class="cellrowborder" valign="top" width="8.99%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p201938822159"><a name="zh-cn_topic_0201534072_p201938822159"></a><a name="zh-cn_topic_0201534072_p201938822159"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="69.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p191679172159"><a name="zh-cn_topic_0201534072_p191679172159"></a><a name="zh-cn_topic_0201534072_p191679172159"></a>floatingip对象列表，参见<a href="#zh-cn_topic_0201534072_table8139247714">表2</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 2**  floatingip对象

<a name="zh-cn_topic_0201534072_table8139247714"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534072_row18132240714"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534072_p101201250870"><a name="zh-cn_topic_0201534072_p101201250870"></a><a name="zh-cn_topic_0201534072_p101201250870"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534072_p161211850674"><a name="zh-cn_topic_0201534072_p161211850674"></a><a name="zh-cn_topic_0201534072_p161211850674"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534072_p41217502719"><a name="zh-cn_topic_0201534072_p41217502719"></a><a name="zh-cn_topic_0201534072_p41217502719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534072_row2014192410713"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p6028218019164"><a name="zh-cn_topic_0201534072_p6028218019164"></a><a name="zh-cn_topic_0201534072_p6028218019164"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p5101843519164"><a name="zh-cn_topic_0201534072_p5101843519164"></a><a name="zh-cn_topic_0201534072_p5101843519164"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p6000412319164"><a name="zh-cn_topic_0201534072_p6000412319164"></a><a name="zh-cn_topic_0201534072_p6000412319164"></a>网络状态，可以为ACTIVE， DOWN或ERROR。</p>
<a name="zh-cn_topic_0201534072_ul10603143175810"></a><a name="zh-cn_topic_0201534072_ul10603143175810"></a><ul id="zh-cn_topic_0201534072_ul10603143175810"><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ERROR：异常</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row4141241070"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p5513524919164"><a name="zh-cn_topic_0201534072_p5513524919164"></a><a name="zh-cn_topic_0201534072_p5513524919164"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p212111505713"><a name="zh-cn_topic_0201534072_p212111505713"></a><a name="zh-cn_topic_0201534072_p212111505713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p4121850371"><a name="zh-cn_topic_0201534072_p4121850371"></a><a name="zh-cn_topic_0201534072_p4121850371"></a>浮动IP地址的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row29903910157"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p1276893520133"><a name="zh-cn_topic_0201534072_p1276893520133"></a><a name="zh-cn_topic_0201534072_p1276893520133"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p147682350136"><a name="zh-cn_topic_0201534072_p147682350136"></a><a name="zh-cn_topic_0201534072_p147682350136"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p876820352133"><a name="zh-cn_topic_0201534072_p876820352133"></a><a name="zh-cn_topic_0201534072_p876820352133"></a>项目ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row614132416712"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p1912112509713"><a name="zh-cn_topic_0201534072_p1912112509713"></a><a name="zh-cn_topic_0201534072_p1912112509713"></a>floating_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p11211850072"><a name="zh-cn_topic_0201534072_p11211850072"></a><a name="zh-cn_topic_0201534072_p11211850072"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p16122205017713"><a name="zh-cn_topic_0201534072_p16122205017713"></a><a name="zh-cn_topic_0201534072_p16122205017713"></a>浮动IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row115102414717"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p61223503712"><a name="zh-cn_topic_0201534072_p61223503712"></a><a name="zh-cn_topic_0201534072_p61223503712"></a>floating_network_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p1812220507714"><a name="zh-cn_topic_0201534072_p1812220507714"></a><a name="zh-cn_topic_0201534072_p1812220507714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p16122550274"><a name="zh-cn_topic_0201534072_p16122550274"></a><a name="zh-cn_topic_0201534072_p16122550274"></a>外部网络的id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row19155241277"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p201223504719"><a name="zh-cn_topic_0201534072_p201223504719"></a><a name="zh-cn_topic_0201534072_p201223504719"></a>router_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p1122155015714"><a name="zh-cn_topic_0201534072_p1122155015714"></a><a name="zh-cn_topic_0201534072_p1122155015714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p812212506713"><a name="zh-cn_topic_0201534072_p812212506713"></a><a name="zh-cn_topic_0201534072_p812212506713"></a>所属路由器id。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row101514247714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p412218502718"><a name="zh-cn_topic_0201534072_p412218502718"></a><a name="zh-cn_topic_0201534072_p412218502718"></a>port_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p612213506716"><a name="zh-cn_topic_0201534072_p612213506716"></a><a name="zh-cn_topic_0201534072_p612213506716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p141228504716"><a name="zh-cn_topic_0201534072_p141228504716"></a><a name="zh-cn_topic_0201534072_p141228504716"></a>端口id</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row3164249715"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p01237508720"><a name="zh-cn_topic_0201534072_p01237508720"></a><a name="zh-cn_topic_0201534072_p01237508720"></a>fixed_ip_address</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p111239501770"><a name="zh-cn_topic_0201534072_p111239501770"></a><a name="zh-cn_topic_0201534072_p111239501770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p1712316501972"><a name="zh-cn_topic_0201534072_p1712316501972"></a><a name="zh-cn_topic_0201534072_p1712316501972"></a>关联端口的私有IP地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row21662416711"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p812355018717"><a name="zh-cn_topic_0201534072_p812355018717"></a><a name="zh-cn_topic_0201534072_p812355018717"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p612316509712"><a name="zh-cn_topic_0201534072_p612316509712"></a><a name="zh-cn_topic_0201534072_p612316509712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p10487112"><a name="zh-cn_topic_0201534072_p10487112"></a><a name="zh-cn_topic_0201534072_p10487112"></a>项目ID</p>
<p id="zh-cn_topic_0201534072_p51231950174"><a name="zh-cn_topic_0201534072_p51231950174"></a><a name="zh-cn_topic_0201534072_p51231950174"></a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row11176241720"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p11222111885214"><a name="zh-cn_topic_0201534072_p11222111885214"></a><a name="zh-cn_topic_0201534072_p11222111885214"></a>dns_name</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p122232018115215"><a name="zh-cn_topic_0201534072_p122232018115215"></a><a name="zh-cn_topic_0201534072_p122232018115215"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p18223161825216"><a name="zh-cn_topic_0201534072_p18223161825216"></a><a name="zh-cn_topic_0201534072_p18223161825216"></a>DNS名称</p>
<p id="zh-cn_topic_0201534072_p158413185159"><a name="zh-cn_topic_0201534072_p158413185159"></a><a name="zh-cn_topic_0201534072_p158413185159"></a>该参数当前仅在“华南-广州”开放</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row17174241670"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p492133065713"><a name="zh-cn_topic_0201534072_p492133065713"></a><a name="zh-cn_topic_0201534072_p492133065713"></a>dns_domain</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p16929300573"><a name="zh-cn_topic_0201534072_p16929300573"></a><a name="zh-cn_topic_0201534072_p16929300573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p3921230175711"><a name="zh-cn_topic_0201534072_p3921230175711"></a><a name="zh-cn_topic_0201534072_p3921230175711"></a>DNS域地址</p>
<p id="zh-cn_topic_0201534072_p0228152112155"><a name="zh-cn_topic_0201534072_p0228152112155"></a><a name="zh-cn_topic_0201534072_p0228152112155"></a>该参数当前仅在“华南-广州”开放</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row1418142410714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p1953114119914"><a name="zh-cn_topic_0201534072_p1953114119914"></a><a name="zh-cn_topic_0201534072_p1953114119914"></a>created_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p595318416919"><a name="zh-cn_topic_0201534072_p595318416919"></a><a name="zh-cn_topic_0201534072_p595318416919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p1395374115919"><a name="zh-cn_topic_0201534072_p1395374115919"></a><a name="zh-cn_topic_0201534072_p1395374115919"></a>资源创建时间</p>
<p id="zh-cn_topic_0201534072_p1232884613478"><a name="zh-cn_topic_0201534072_p1232884613478"></a><a name="zh-cn_topic_0201534072_p1232884613478"></a>采用UTC时间</p>
<p id="zh-cn_topic_0201534072_p2070141994713"><a name="zh-cn_topic_0201534072_p2070141994713"></a><a name="zh-cn_topic_0201534072_p2070141994713"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534072_row1188246714"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534072_p139719548912"><a name="zh-cn_topic_0201534072_p139719548912"></a><a name="zh-cn_topic_0201534072_p139719548912"></a>updated_at</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534072_p53971154594"><a name="zh-cn_topic_0201534072_p53971154594"></a><a name="zh-cn_topic_0201534072_p53971154594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534072_p1339713549918"><a name="zh-cn_topic_0201534072_p1339713549918"></a><a name="zh-cn_topic_0201534072_p1339713549918"></a>资源更新时间</p>
<p id="zh-cn_topic_0201534072_p876511114816"><a name="zh-cn_topic_0201534072_p876511114816"></a><a name="zh-cn_topic_0201534072_p876511114816"></a>采用UTC时间</p>
<p id="zh-cn_topic_0201534072_p137222218476"><a name="zh-cn_topic_0201534072_p137222218476"></a><a name="zh-cn_topic_0201534072_p137222218476"></a>格式：YYYY-MM-DDTHH:MM:SS</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="zh-cn_topic_0201534072_section382935262159"></a>

请求样例

```
GET https://{Endpoint}/v2.0/floatingips/1a3a2818-d9b4-4a9c-8a19-5252c499d1cd
```

响应样例

```
{
    "floatingip": {
        "id": "1a3a2818-d9b4-4a9c-8a19-5252c499d1cd",
        "status": "DOWN",
        "router_id": null,
        "tenant_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "project_id": "bbfe8c41dd034a07bebd592bf03b4b0c",
        "floating_network_id": "0a2228f2-7f8a-45f1-8e09-9039e1d09975",
        "fixed_ip_address": null,
        "floating_ip_address": "99.99.99.84",
        "port_id": null,
        "created_at": "2017-10-19T12:21:28",
        "updated_at": "2018-07-30T12:52:13"
    }
}
```

## 状态码<a name="zh-cn_topic_0201534072_section10470352390"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534072_section85821649202813"></a>

请参见[错误码](错误码.md)。

