# 删除浮动IP<a name="eip_openstackapi_0010"></a>

## 功能介绍<a name="zh-cn_topic_0201534157_section1285101621658"></a>

删除浮动IP。

## 调试<a name="zh-cn_topic_0201534157_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&version=v2&api=NeutronDeleteFloatingIp)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0201534157_section4025916121658"></a>

DELETE /v2.0/floatingips/\{floatingip\_id\}

参数说明请参见[表1](#zh-cn_topic_0201534157_table49321613135118)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534157_table49321613135118"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534157_row89331813135112"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534157_p116676362558"><a name="zh-cn_topic_0201534157_p116676362558"></a><a name="zh-cn_topic_0201534157_p116676362558"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534157_p16671836175513"><a name="zh-cn_topic_0201534157_p16671836175513"></a><a name="zh-cn_topic_0201534157_p16671836175513"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534157_p1766716366555"><a name="zh-cn_topic_0201534157_p1766716366555"></a><a name="zh-cn_topic_0201534157_p1766716366555"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534157_p116679360559"><a name="zh-cn_topic_0201534157_p116679360559"></a><a name="zh-cn_topic_0201534157_p116679360559"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534157_row4934113125120"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534157_p1036313125105"><a name="zh-cn_topic_0201534157_p1036313125105"></a><a name="zh-cn_topic_0201534157_p1036313125105"></a>floatingip_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534157_p11667113619558"><a name="zh-cn_topic_0201534157_p11667113619558"></a><a name="zh-cn_topic_0201534157_p11667113619558"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534157_p26672036175513"><a name="zh-cn_topic_0201534157_p26672036175513"></a><a name="zh-cn_topic_0201534157_p26672036175513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534157_p566713367557"><a name="zh-cn_topic_0201534157_p566713367557"></a><a name="zh-cn_topic_0201534157_p566713367557"></a>浮动IP地址的id。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534157_section5856898621658"></a>

无。

## 响应消息<a name="zh-cn_topic_0201534157_section1555365521658"></a>

无。

## 样例<a name="zh-cn_topic_0201534157_section6432601621658"></a>

请求样例

```
DELETE https://{Endpoint}/v2.0/floatingips/a95ec431-8473-463b-aede-34fb048ee3a7
```

响应样例

无。

## 状态码<a name="zh-cn_topic_0201534157_section10470352390"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534157_section85821649202813"></a>

请参见[错误码](错误码.md)。

