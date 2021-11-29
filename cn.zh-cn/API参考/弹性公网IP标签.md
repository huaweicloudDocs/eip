# 弹性公网IP标签<a name="eip_apipermission_0005"></a>

<a name="zh-cn_topic_0201534116_table1877617451848"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534116_row12776124514415"><th class="cellrowborder" valign="top" width="15.518448155184483%" id="mcps1.1.6.1.1"><p id="zh-cn_topic_0201534116_p6174435204812"><a name="zh-cn_topic_0201534116_p6174435204812"></a><a name="zh-cn_topic_0201534116_p6174435204812"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="32.396760323967605%" id="mcps1.1.6.1.2"><p id="zh-cn_topic_0201534116_p8174113504816"><a name="zh-cn_topic_0201534116_p8174113504816"></a><a name="zh-cn_topic_0201534116_p8174113504816"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="21.11788821117888%" id="mcps1.1.6.1.3"><p id="zh-cn_topic_0201534116_p8701346133717"><a name="zh-cn_topic_0201534116_p8701346133717"></a><a name="zh-cn_topic_0201534116_p8701346133717"></a>授权项(Action)</p>
</th>
<th class="cellrowborder" valign="top" width="15.918408159184082%" id="mcps1.1.6.1.4"><p id="zh-cn_topic_0201534116_p5985736163016"><a name="zh-cn_topic_0201534116_p5985736163016"></a><a name="zh-cn_topic_0201534116_p5985736163016"></a>IAM项目(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="15.04849515048495%" id="mcps1.1.6.1.5"><p id="zh-cn_topic_0201534116_p8985133619300"><a name="zh-cn_topic_0201534116_p8985133619300"></a><a name="zh-cn_topic_0201534116_p8985133619300"></a>企业项目(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534116_row197771453415"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p1177710451042"><a name="zh-cn_topic_0201534116_p1177710451042"></a><a name="zh-cn_topic_0201534116_p1177710451042"></a>创建<span id="zh-cn_topic_0201534116_text10897104815286"><a name="zh-cn_topic_0201534116_text10897104815286"></a><a name="zh-cn_topic_0201534116_text10897104815286"></a></span><span id="zh-cn_topic_0201534116_text1689724812819"><a name="zh-cn_topic_0201534116_text1689724812819"></a><a name="zh-cn_topic_0201534116_text1689724812819"></a>弹性公网IP</span>资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p1994810358574"><a name="zh-cn_topic_0201534116_p1994810358574"></a><a name="zh-cn_topic_0201534116_p1994810358574"></a>POST /v2.0/{project_id}/publicips/{publicip_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p877715451249"><a name="zh-cn_topic_0201534116_p877715451249"></a><a name="zh-cn_topic_0201534116_p877715451249"></a>vpc:publicipTags:create</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p1475655902719"><a name="zh-cn_topic_0201534116_p1475655902719"></a><a name="zh-cn_topic_0201534116_p1475655902719"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p153706545313"><a name="zh-cn_topic_0201534116_p153706545313"></a><a name="zh-cn_topic_0201534116_p153706545313"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534116_row127773451142"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p177771457412"><a name="zh-cn_topic_0201534116_p177771457412"></a><a name="zh-cn_topic_0201534116_p177771457412"></a>查询<span id="zh-cn_topic_0201534116_text7979133714599"><a name="zh-cn_topic_0201534116_text7979133714599"></a><a name="zh-cn_topic_0201534116_text7979133714599"></a></span><span id="zh-cn_topic_0201534116_text397913745915"><a name="zh-cn_topic_0201534116_text397913745915"></a><a name="zh-cn_topic_0201534116_text397913745915"></a>弹性公网IP</span>资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p177774455413"><a name="zh-cn_topic_0201534116_p177774455413"></a><a name="zh-cn_topic_0201534116_p177774455413"></a>GET /v2.0/{project_id}/publicips/{publicip_id}/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p97779454415"><a name="zh-cn_topic_0201534116_p97779454415"></a><a name="zh-cn_topic_0201534116_p97779454415"></a>vpc:publicipTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p167561459142711"><a name="zh-cn_topic_0201534116_p167561459142711"></a><a name="zh-cn_topic_0201534116_p167561459142711"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p1370175418319"><a name="zh-cn_topic_0201534116_p1370175418319"></a><a name="zh-cn_topic_0201534116_p1370175418319"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534116_row117775452419"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p577714515414"><a name="zh-cn_topic_0201534116_p577714515414"></a><a name="zh-cn_topic_0201534116_p577714515414"></a>删除<span id="zh-cn_topic_0201534116_text6529104118591"><a name="zh-cn_topic_0201534116_text6529104118591"></a><a name="zh-cn_topic_0201534116_text6529104118591"></a></span><span id="zh-cn_topic_0201534116_text35301541105913"><a name="zh-cn_topic_0201534116_text35301541105913"></a><a name="zh-cn_topic_0201534116_text35301541105913"></a>弹性公网IP</span>资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p10777124513414"><a name="zh-cn_topic_0201534116_p10777124513414"></a><a name="zh-cn_topic_0201534116_p10777124513414"></a>DELETE /v2.0/{project_id}/publicips/{publicip_id}/tags/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p27775454417"><a name="zh-cn_topic_0201534116_p27775454417"></a><a name="zh-cn_topic_0201534116_p27775454417"></a>vpc:publicipTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p9757145912271"><a name="zh-cn_topic_0201534116_p9757145912271"></a><a name="zh-cn_topic_0201534116_p9757145912271"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p19370155411318"><a name="zh-cn_topic_0201534116_p19370155411318"></a><a name="zh-cn_topic_0201534116_p19370155411318"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534116_row5777114510411"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p1077794511419"><a name="zh-cn_topic_0201534116_p1077794511419"></a><a name="zh-cn_topic_0201534116_p1077794511419"></a>批量创建和删除<span id="zh-cn_topic_0201534116_text179216452597"><a name="zh-cn_topic_0201534116_text179216452597"></a><a name="zh-cn_topic_0201534116_text179216452597"></a></span><span id="zh-cn_topic_0201534116_text14792445105913"><a name="zh-cn_topic_0201534116_text14792445105913"></a><a name="zh-cn_topic_0201534116_text14792445105913"></a>弹性公网IP</span>资源标签</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p6777144516417"><a name="zh-cn_topic_0201534116_p6777144516417"></a><a name="zh-cn_topic_0201534116_p6777144516417"></a>POST /v2.0/{project_id}/publicips/{publicip_id}/tags/action</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p12618529014"><a name="zh-cn_topic_0201534116_p12618529014"></a><a name="zh-cn_topic_0201534116_p12618529014"></a>vpc:publicipTags:create</p>
<p id="zh-cn_topic_0201534116_p27771845341"><a name="zh-cn_topic_0201534116_p27771845341"></a><a name="zh-cn_topic_0201534116_p27771845341"></a>vpc:publicipTags:delete</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p187577594276"><a name="zh-cn_topic_0201534116_p187577594276"></a><a name="zh-cn_topic_0201534116_p187577594276"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p10370105493116"><a name="zh-cn_topic_0201534116_p10370105493116"></a><a name="zh-cn_topic_0201534116_p10370105493116"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534116_row1141921219586"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p1242216120589"><a name="zh-cn_topic_0201534116_p1242216120589"></a><a name="zh-cn_topic_0201534116_p1242216120589"></a>查询<span id="zh-cn_topic_0201534116_text19933750145914"><a name="zh-cn_topic_0201534116_text19933750145914"></a><a name="zh-cn_topic_0201534116_text19933750145914"></a></span><span id="zh-cn_topic_0201534116_text4933115095920"><a name="zh-cn_topic_0201534116_text4933115095920"></a><a name="zh-cn_topic_0201534116_text4933115095920"></a>弹性公网IP</span>资源实例</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p842291235811"><a name="zh-cn_topic_0201534116_p842291235811"></a><a name="zh-cn_topic_0201534116_p842291235811"></a>POST /v2.0/{project_id}/publicips/resource_instances/action</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p16422151245812"><a name="zh-cn_topic_0201534116_p16422151245812"></a><a name="zh-cn_topic_0201534116_p16422151245812"></a>vpc:publicipTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p1267045134615"><a name="zh-cn_topic_0201534116_p1267045134615"></a><a name="zh-cn_topic_0201534116_p1267045134615"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p6670155114465"><a name="zh-cn_topic_0201534116_p6670155114465"></a><a name="zh-cn_topic_0201534116_p6670155114465"></a>×</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534116_row65981915155810"><td class="cellrowborder" valign="top" width="15.518448155184483%" headers="mcps1.1.6.1.1 "><p id="zh-cn_topic_0201534116_p11599181585812"><a name="zh-cn_topic_0201534116_p11599181585812"></a><a name="zh-cn_topic_0201534116_p11599181585812"></a>查询<span id="zh-cn_topic_0201534116_text155491954155920"><a name="zh-cn_topic_0201534116_text155491954155920"></a><a name="zh-cn_topic_0201534116_text155491954155920"></a></span><span id="zh-cn_topic_0201534116_text12549105417594"><a name="zh-cn_topic_0201534116_text12549105417594"></a><a name="zh-cn_topic_0201534116_text12549105417594"></a>弹性公网IP</span>项目标签</p>
</td>
<td class="cellrowborder" valign="top" width="32.396760323967605%" headers="mcps1.1.6.1.2 "><p id="zh-cn_topic_0201534116_p197780456413"><a name="zh-cn_topic_0201534116_p197780456413"></a><a name="zh-cn_topic_0201534116_p197780456413"></a>GET /v2.0/{project_id}/publicips/tags</p>
</td>
<td class="cellrowborder" valign="top" width="21.11788821117888%" headers="mcps1.1.6.1.3 "><p id="zh-cn_topic_0201534116_p5599171518589"><a name="zh-cn_topic_0201534116_p5599171518589"></a><a name="zh-cn_topic_0201534116_p5599171518589"></a>vpc:publicipTags:get</p>
</td>
<td class="cellrowborder" valign="top" width="15.918408159184082%" headers="mcps1.1.6.1.4 "><p id="zh-cn_topic_0201534116_p5670165120466"><a name="zh-cn_topic_0201534116_p5670165120466"></a><a name="zh-cn_topic_0201534116_p5670165120466"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="15.04849515048495%" headers="mcps1.1.6.1.5 "><p id="zh-cn_topic_0201534116_p167055174612"><a name="zh-cn_topic_0201534116_p167055174612"></a><a name="zh-cn_topic_0201534116_p167055174612"></a>×</p>
</td>
</tr>
</tbody>
</table>

