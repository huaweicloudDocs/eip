# API概览<a name="eip_api02_0001"></a>

弹性公网IP所提供的接口分为EIP接口与OpenStack原生接口。

通过配合使用EIP接口和OpenStack原生接口，您可以完整的使用弹性公网IP的所有功能。

对于企业项目用户，只能使用EIP接口，各接口对应的权限说明请参见[权限策略和授权项](权限策略和授权项.md)。

## EIP接口说明<a name="section14330125184315"></a>

**表 1**  EIP接口说明

<a name="table1336185894518"></a>
<table><thead align="left"><tr id="row3362058124511"><th class="cellrowborder" valign="top" width="20.810000000000002%" id="mcps1.2.3.1.1"><p id="p336219586450"><a name="p336219586450"></a><a name="p336219586450"></a><strong id="b10362175817458"><a name="b10362175817458"></a><a name="b10362175817458"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="79.19%" id="mcps1.2.3.1.2"><p id="p1636275810454"><a name="p1636275810454"></a><a name="p1636275810454"></a><strong id="b236225874512"><a name="b236225874512"></a><a name="b236225874512"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row14362205884514"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1947611525917"><a name="p1947611525917"></a><a name="p1947611525917"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0000.html" target="_blank" rel="noopener noreferrer">弹性公网IP</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p9476152399"><a name="p9476152399"></a><a name="p9476152399"></a>弹性公网IP的申请、查询、更新、删除等接口。</p>
</td>
</tr>
<tr id="row103631858124512"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1447619521696"><a name="p1447619521696"></a><a name="p1447619521696"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0000.html" target="_blank" rel="noopener noreferrer">带宽</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p547615217914"><a name="p547615217914"></a><a name="p547615217914"></a>带宽的查询、更新等接口。</p>
</td>
</tr>
<tr id="row736325817457"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p1447695213912"><a name="p1447695213912"></a><a name="p1447695213912"></a><a href="https://support.huaweicloud.com/api-eip/eip_apisharedbandwidth_0000.html" target="_blank" rel="noopener noreferrer">带宽（V2.0）</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><a name="ul15648203810547"></a><a name="ul15648203810547"></a><ul id="ul15648203810547"><li>共享带宽的创建、删除等接口。</li><li>共享带宽插入/移出弹性公网IP操作。</li></ul>
</td>
</tr>
<tr id="row53631958124513"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p17476115218917"><a name="p17476115218917"></a><a name="p17476115218917"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiquota_0000.html" target="_blank" rel="noopener noreferrer">配额</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p14476352194"><a name="p14476352194"></a><a name="p14476352194"></a>配额查询接口。</p>
</td>
</tr>
<tr id="row1736416582452"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p11476752195"><a name="p11476752195"></a><a name="p11476752195"></a><a href="https://support.huaweicloud.com/api-eip/eip_apitag_0000.html" target="_blank" rel="noopener noreferrer">弹性IP资源标签管理</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p54769521599"><a name="p54769521599"></a><a name="p54769521599"></a>弹性公网IP标签的创建、查询、删除等接口。</p>
<p id="p147735213915"><a name="p147735213915"></a><a name="p147735213915"></a>该类型接口目前仅在“华北-北京四”、“华东-上海一”、“华东-上海二”、“西南-贵阳一”区域开放。</p>
</td>
</tr>
</tbody>
</table>

## OpenStack原生接口说明<a name="section3102202117447"></a>

**表 2**  OpenStack原生接口说明

<a name="table101761398465"></a>
<table><thead align="left"><tr id="row1617633924619"><th class="cellrowborder" valign="top" width="20.810000000000002%" id="mcps1.2.3.1.1"><p id="p2176153924610"><a name="p2176153924610"></a><a name="p2176153924610"></a><strong id="b2176183915460"><a name="b2176183915460"></a><a name="b2176183915460"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="79.19%" id="mcps1.2.3.1.2"><p id="p3176143954615"><a name="p3176143954615"></a><a name="p3176143954615"></a><strong id="b1917614397466"><a name="b1917614397466"></a><a name="b1917614397466"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row15136113317137"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p14180031171715"><a name="p14180031171715"></a><a name="p14180031171715"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0001.html" target="_blank" rel="noopener noreferrer">API版本信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p8944330141213"><a name="p8944330141213"></a><a name="p8944330141213"></a>当前API所有可用版本的查询、分页查询。</p>
</td>
</tr>
<tr id="row6185339124618"><td class="cellrowborder" valign="top" width="20.810000000000002%" headers="mcps1.2.3.1.1 "><p id="p5944163031217"><a name="p5944163031217"></a><a name="p5944163031217"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0005.html" target="_blank" rel="noopener noreferrer">浮动IP</a></p>
</td>
<td class="cellrowborder" valign="top" width="79.19%" headers="mcps1.2.3.1.2 "><p id="p19443303128"><a name="p19443303128"></a><a name="p19443303128"></a>浮动IP的查询、创建、更新、删除等接口。</p>
</td>
</tr>
</tbody>
</table>

