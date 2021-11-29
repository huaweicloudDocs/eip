# 浮动IP（Openstack Neutron API）<a name="eip_apipermission_0006"></a>

<a name="zh-cn_topic_0201534306_table620116613438"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534306_row122422612431"><th class="cellrowborder" valign="top" width="12.920000000000002%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0201534306_p6174435204812"><a name="zh-cn_topic_0201534306_p6174435204812"></a><a name="zh-cn_topic_0201534306_p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="30.099999999999998%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0201534306_p8174113504816"><a name="zh-cn_topic_0201534306_p8174113504816"></a><a name="zh-cn_topic_0201534306_p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="25.22%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0201534306_p8701346133717"><a name="zh-cn_topic_0201534306_p8701346133717"></a><a name="zh-cn_topic_0201534306_p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.299999999999999%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0201534306_p5985736163016"><a name="zh-cn_topic_0201534306_p5985736163016"></a><a name="zh-cn_topic_0201534306_p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="16.46%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0201534306_p8985133619300"><a name="zh-cn_topic_0201534306_p8985133619300"></a><a name="zh-cn_topic_0201534306_p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534306_row11242186124315"><td class="cellrowborder" valign="top" width="12.920000000000002%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534306_p1942012471564"><a name="zh-cn_topic_0201534306_p1942012471564"></a><a name="zh-cn_topic_0201534306_p1942012471564"></a>查询浮动IP列表</p>
</td>
<td class="cellrowborder" valign="top" width="30.099999999999998%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534306_p16242156154311"><a name="zh-cn_topic_0201534306_p16242156154311"></a><a name="zh-cn_topic_0201534306_p16242156154311"></a>GET /v2.0/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534306_p5358141413439"><a name="zh-cn_topic_0201534306_p5358141413439"></a><a name="zh-cn_topic_0201534306_p5358141413439"></a>vpc:floatingIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.299999999999999%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534306_p1475655902719"><a name="zh-cn_topic_0201534306_p1475655902719"></a><a name="zh-cn_topic_0201534306_p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.46%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534306_p153706545313"><a name="zh-cn_topic_0201534306_p153706545313"></a><a name="zh-cn_topic_0201534306_p153706545313"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534306_row1424216134314"><td class="cellrowborder" valign="top" width="12.920000000000002%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534306_p9420164712614"><a name="zh-cn_topic_0201534306_p9420164712614"></a><a name="zh-cn_topic_0201534306_p9420164712614"></a>查询浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="30.099999999999998%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534306_p1124219664317"><a name="zh-cn_topic_0201534306_p1124219664317"></a><a name="zh-cn_topic_0201534306_p1124219664317"></a>GET /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534306_p1818716161433"><a name="zh-cn_topic_0201534306_p1818716161433"></a><a name="zh-cn_topic_0201534306_p1818716161433"></a>vpc:floatingIps:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.299999999999999%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534306_p167561459142711"><a name="zh-cn_topic_0201534306_p167561459142711"></a><a name="zh-cn_topic_0201534306_p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.46%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534306_p1370175418319"><a name="zh-cn_topic_0201534306_p1370175418319"></a><a name="zh-cn_topic_0201534306_p1370175418319"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534306_row192471262439"><td class="cellrowborder" valign="top" width="12.920000000000002%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534306_p13420547366"><a name="zh-cn_topic_0201534306_p13420547366"></a><a name="zh-cn_topic_0201534306_p13420547366"></a>创建浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="30.099999999999998%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534306_p92473619434"><a name="zh-cn_topic_0201534306_p92473619434"></a><a name="zh-cn_topic_0201534306_p92473619434"></a>POST /v2.0/floatingips</p>
</td>
<td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534306_p142981517134319"><a name="zh-cn_topic_0201534306_p142981517134319"></a><a name="zh-cn_topic_0201534306_p142981517134319"></a>vpc:floatingIps:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.299999999999999%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534306_p9757145912271"><a name="zh-cn_topic_0201534306_p9757145912271"></a><a name="zh-cn_topic_0201534306_p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.46%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534306_p19370155411318"><a name="zh-cn_topic_0201534306_p19370155411318"></a><a name="zh-cn_topic_0201534306_p19370155411318"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534306_row1724719674312"><td class="cellrowborder" valign="top" width="12.920000000000002%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534306_p16420347065"><a name="zh-cn_topic_0201534306_p16420347065"></a><a name="zh-cn_topic_0201534306_p16420347065"></a>更新浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="30.099999999999998%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534306_p1224756134320"><a name="zh-cn_topic_0201534306_p1224756134320"></a><a name="zh-cn_topic_0201534306_p1224756134320"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534306_p17326101812436"><a name="zh-cn_topic_0201534306_p17326101812436"></a><a name="zh-cn_topic_0201534306_p17326101812436"></a>vpc:floatingIps:update</p>
</td>
<td class="cellrowborder" valign="top" width="15.299999999999999%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534306_p187577594276"><a name="zh-cn_topic_0201534306_p187577594276"></a><a name="zh-cn_topic_0201534306_p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.46%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534306_p10370105493116"><a name="zh-cn_topic_0201534306_p10370105493116"></a><a name="zh-cn_topic_0201534306_p10370105493116"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534306_row102470615434"><td class="cellrowborder" valign="top" width="12.920000000000002%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534306_p1542119471269"><a name="zh-cn_topic_0201534306_p1542119471269"></a><a name="zh-cn_topic_0201534306_p1542119471269"></a>删除浮动IP</p>
</td>
<td class="cellrowborder" valign="top" width="30.099999999999998%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534306_p9247126204318"><a name="zh-cn_topic_0201534306_p9247126204318"></a><a name="zh-cn_topic_0201534306_p9247126204318"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
</td>
<td class="cellrowborder" valign="top" width="25.22%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534306_p64451919134314"><a name="zh-cn_topic_0201534306_p64451919134314"></a><a name="zh-cn_topic_0201534306_p64451919134314"></a>vpc:floatingIps:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.299999999999999%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534306_p1267045134615"><a name="zh-cn_topic_0201534306_p1267045134615"></a><a name="zh-cn_topic_0201534306_p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="16.46%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534306_p6670155114465"><a name="zh-cn_topic_0201534306_p6670155114465"></a><a name="zh-cn_topic_0201534306_p6670155114465"></a>×</p>
</td>
</tr>
</tbody>
</table>

