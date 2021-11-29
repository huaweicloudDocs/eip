# 弹性公网IP<a name="eip_apipermission_0002"></a>

<a name="zh-cn_topic_0201534207_table3381441153612"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534207_row134361241153612"><th class="cellrowborder" valign="top" width="13.23%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0201534207_p423285813514"><a name="zh-cn_topic_0201534207_p423285813514"></a><a name="zh-cn_topic_0201534207_p423285813514"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="29.330000000000002%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0201534207_p24367414363"><a name="zh-cn_topic_0201534207_p24367414363"></a><a name="zh-cn_topic_0201534207_p24367414363"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="20.06%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0201534207_p2436194193616"><a name="zh-cn_topic_0201534207_p2436194193616"></a><a name="zh-cn_topic_0201534207_p2436194193616"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.89%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0201534207_p5985736163016"><a name="zh-cn_topic_0201534207_p5985736163016"></a><a name="zh-cn_topic_0201534207_p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="21.490000000000002%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0201534207_p8985133619300"><a name="zh-cn_topic_0201534207_p8985133619300"></a><a name="zh-cn_topic_0201534207_p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534207_row943674133617"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p13232958145117"><a name="zh-cn_topic_0201534207_p13232958145117"></a><a name="zh-cn_topic_0201534207_p13232958145117"></a>申请<span id="zh-cn_topic_0201534207_text10897104815286"><a name="zh-cn_topic_0201534207_text10897104815286"></a><a name="zh-cn_topic_0201534207_text10897104815286"></a></span><span id="zh-cn_topic_0201534207_text1689724812819"><a name="zh-cn_topic_0201534207_text1689724812819"></a><a name="zh-cn_topic_0201534207_text1689724812819"></a>弹性公网IP</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p144365416368"><a name="zh-cn_topic_0201534207_p144365416368"></a><a name="zh-cn_topic_0201534207_p144365416368"></a>POST /v1/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p17904175011365"><a name="zh-cn_topic_0201534207_p17904175011365"></a><a name="zh-cn_topic_0201534207_p17904175011365"></a>vpc:publicIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p15756115919276"><a name="zh-cn_topic_0201534207_p15756115919276"></a><a name="zh-cn_topic_0201534207_p15756115919276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p193691154133112"><a name="zh-cn_topic_0201534207_p193691154133112"></a><a name="zh-cn_topic_0201534207_p193691154133112"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534207_row343704173619"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p1623218589512"><a name="zh-cn_topic_0201534207_p1623218589512"></a><a name="zh-cn_topic_0201534207_p1623218589512"></a>查询<span id="zh-cn_topic_0201534207_text11285177584"><a name="zh-cn_topic_0201534207_text11285177584"></a><a name="zh-cn_topic_0201534207_text11285177584"></a></span><span id="zh-cn_topic_0201534207_text42816171584"><a name="zh-cn_topic_0201534207_text42816171584"></a><a name="zh-cn_topic_0201534207_text42816171584"></a>弹性公网IP</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p174371341133618"><a name="zh-cn_topic_0201534207_p174371341133618"></a><a name="zh-cn_topic_0201534207_p174371341133618"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p8360152113611"><a name="zh-cn_topic_0201534207_p8360152113611"></a><a name="zh-cn_topic_0201534207_p8360152113611"></a>vpc:publicIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p1475655902719"><a name="zh-cn_topic_0201534207_p1475655902719"></a><a name="zh-cn_topic_0201534207_p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p153706545313"><a name="zh-cn_topic_0201534207_p153706545313"></a><a name="zh-cn_topic_0201534207_p153706545313"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534207_row34371241143616"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p182321558155116"><a name="zh-cn_topic_0201534207_p182321558155116"></a><a name="zh-cn_topic_0201534207_p182321558155116"></a>查询<span id="zh-cn_topic_0201534207_text4675527175812"><a name="zh-cn_topic_0201534207_text4675527175812"></a><a name="zh-cn_topic_0201534207_text4675527175812"></a></span><span id="zh-cn_topic_0201534207_text8675142785815"><a name="zh-cn_topic_0201534207_text8675142785815"></a><a name="zh-cn_topic_0201534207_text8675142785815"></a>弹性公网IP</span>列表</p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p16437174193619"><a name="zh-cn_topic_0201534207_p16437174193619"></a><a name="zh-cn_topic_0201534207_p16437174193619"></a>GET /v1/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p35961753143612"><a name="zh-cn_topic_0201534207_p35961753143612"></a><a name="zh-cn_topic_0201534207_p35961753143612"></a>vpc:publicIps:list</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p167561459142711"><a name="zh-cn_topic_0201534207_p167561459142711"></a><a name="zh-cn_topic_0201534207_p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p1370175418319"><a name="zh-cn_topic_0201534207_p1370175418319"></a><a name="zh-cn_topic_0201534207_p1370175418319"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534207_row443713412363"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p623295805113"><a name="zh-cn_topic_0201534207_p623295805113"></a><a name="zh-cn_topic_0201534207_p623295805113"></a>更新<span id="zh-cn_topic_0201534207_text4983204019588"><a name="zh-cn_topic_0201534207_text4983204019588"></a><a name="zh-cn_topic_0201534207_text4983204019588"></a></span><span id="zh-cn_topic_0201534207_text10983114025819"><a name="zh-cn_topic_0201534207_text10983114025819"></a><a name="zh-cn_topic_0201534207_text10983114025819"></a>弹性公网IP</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p4437194193614"><a name="zh-cn_topic_0201534207_p4437194193614"></a><a name="zh-cn_topic_0201534207_p4437194193614"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p1060705413366"><a name="zh-cn_topic_0201534207_p1060705413366"></a><a name="zh-cn_topic_0201534207_p1060705413366"></a>vpc:publicIps:update</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p9757145912271"><a name="zh-cn_topic_0201534207_p9757145912271"></a><a name="zh-cn_topic_0201534207_p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p19370155411318"><a name="zh-cn_topic_0201534207_p19370155411318"></a><a name="zh-cn_topic_0201534207_p19370155411318"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534207_row10437144143617"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p923213587517"><a name="zh-cn_topic_0201534207_p923213587517"></a><a name="zh-cn_topic_0201534207_p923213587517"></a>删除<span id="zh-cn_topic_0201534207_text9422745175810"><a name="zh-cn_topic_0201534207_text9422745175810"></a><a name="zh-cn_topic_0201534207_text9422745175810"></a></span><span id="zh-cn_topic_0201534207_text144221945115816"><a name="zh-cn_topic_0201534207_text144221945115816"></a><a name="zh-cn_topic_0201534207_text144221945115816"></a>弹性公网IP</span></p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p2437114115362"><a name="zh-cn_topic_0201534207_p2437114115362"></a><a name="zh-cn_topic_0201534207_p2437114115362"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p986195516362"><a name="zh-cn_topic_0201534207_p986195516362"></a><a name="zh-cn_topic_0201534207_p986195516362"></a>vpc:publicIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p187577594276"><a name="zh-cn_topic_0201534207_p187577594276"></a><a name="zh-cn_topic_0201534207_p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p10370105493116"><a name="zh-cn_topic_0201534207_p10370105493116"></a><a name="zh-cn_topic_0201534207_p10370105493116"></a>√</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534207_row06971339262"><td class="cellrowborder" valign="top" width="13.23%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534207_p643581217266"><a name="zh-cn_topic_0201534207_p643581217266"></a><a name="zh-cn_topic_0201534207_p643581217266"></a>申请<span id="zh-cn_topic_0201534207_text16341125116584"><a name="zh-cn_topic_0201534207_text16341125116584"></a><a name="zh-cn_topic_0201534207_text16341125116584"></a></span><span id="zh-cn_topic_0201534207_text9341135115817"><a name="zh-cn_topic_0201534207_text9341135115817"></a><a name="zh-cn_topic_0201534207_text9341135115817"></a>弹性公网IP</span>（包年/包月）</p>
</td>
<td class="cellrowborder" valign="top" width="29.330000000000002%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534207_p17435812172618"><a name="zh-cn_topic_0201534207_p17435812172618"></a><a name="zh-cn_topic_0201534207_p17435812172618"></a>POST /v2.0/{project_id}/publicips</p>
</td>
<td class="cellrowborder" valign="top" width="20.06%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534207_p343511262614"><a name="zh-cn_topic_0201534207_p343511262614"></a><a name="zh-cn_topic_0201534207_p343511262614"></a>vpc:publicIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.89%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534207_p1023909163617"><a name="zh-cn_topic_0201534207_p1023909163617"></a><a name="zh-cn_topic_0201534207_p1023909163617"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="21.490000000000002%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534207_p82391694362"><a name="zh-cn_topic_0201534207_p82391694362"></a><a name="zh-cn_topic_0201534207_p82391694362"></a>√</p>
</td>
</tr>
</tbody>
</table>

