# 更新弹性公网IP<a name="eip_api_0004"></a>

## 功能介绍<a name="zh-cn_topic_0201534286_section43589445"></a>

更新弹性公网IP，将弹性公网IP跟一个网卡绑定或者解绑定，转换IP地址版本类型。

## 调试<a name="zh-cn_topic_0201534286_section1062181918110"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&version=v2&api=UpdatePublicip)中直接运行调试该接口。

## URI<a name="zh-cn_topic_0201534286_section56760689"></a>

PUT /v1/\{project\_id\}/publicips/\{publicip\_id\}

参数说明请参见[表1](#zh-cn_topic_0201534286_table25231885)。

**表 1**  参数说明

<a name="zh-cn_topic_0201534286_table25231885"></a>
<table><thead align="left"><tr id="zh-cn_topic_0201534286_row34804713"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534286_p609510"><a name="zh-cn_topic_0201534286_p609510"></a><a name="zh-cn_topic_0201534286_p609510"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534286_p49370368"><a name="zh-cn_topic_0201534286_p49370368"></a><a name="zh-cn_topic_0201534286_p49370368"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534286_p39576862"><a name="zh-cn_topic_0201534286_p39576862"></a><a name="zh-cn_topic_0201534286_p39576862"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0201534286_row51609257"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p19600264"><a name="zh-cn_topic_0201534286_p19600264"></a><a name="zh-cn_topic_0201534286_p19600264"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p44117540"><a name="zh-cn_topic_0201534286_p44117540"></a><a name="zh-cn_topic_0201534286_p44117540"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p10487112"><a name="zh-cn_topic_0201534286_p10487112"></a><a name="zh-cn_topic_0201534286_p10487112"></a>项目ID，获取项目ID请参见<a href="获取项目ID.md#eip_api06_0004">获取项目ID</a>。</p>
</td>
</tr>
<tr id="zh-cn_topic_0201534286_row16540805"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p64736823"><a name="zh-cn_topic_0201534286_p64736823"></a><a name="zh-cn_topic_0201534286_p64736823"></a>publicip_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p9191297"><a name="zh-cn_topic_0201534286_p9191297"></a><a name="zh-cn_topic_0201534286_p9191297"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p6297612"><a name="zh-cn_topic_0201534286_p6297612"></a><a name="zh-cn_topic_0201534286_p6297612"></a><span id="zh-cn_topic_0201534286_text1431316332138"><a name="zh-cn_topic_0201534286_text1431316332138"></a><a name="zh-cn_topic_0201534286_text1431316332138"></a></span><span id="zh-cn_topic_0201534286_text1431383314138"><a name="zh-cn_topic_0201534286_text1431383314138"></a><a name="zh-cn_topic_0201534286_text1431383314138"></a>弹性公网IP</span>唯一标识</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0201534286_section41084157"></a>

-   请求参数

    **表 2**  请求参数

    <a name="zh-cn_topic_0201534286_table46814673152226"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534286_row46264343152226"><th class="cellrowborder" valign="top" width="15.409999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534286_p56424328152226"><a name="zh-cn_topic_0201534286_p56424328152226"></a><a name="zh-cn_topic_0201534286_p56424328152226"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.98%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534286_p6967894152226"><a name="zh-cn_topic_0201534286_p6967894152226"></a><a name="zh-cn_topic_0201534286_p6967894152226"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534286_p27528552152226"><a name="zh-cn_topic_0201534286_p27528552152226"></a><a name="zh-cn_topic_0201534286_p27528552152226"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.18%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534286_p15220263152226"><a name="zh-cn_topic_0201534286_p15220263152226"></a><a name="zh-cn_topic_0201534286_p15220263152226"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534286_row24881786152226"><td class="cellrowborder" valign="top" width="15.409999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534286_p2158794152226"><a name="zh-cn_topic_0201534286_p2158794152226"></a><a name="zh-cn_topic_0201534286_p2158794152226"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.98%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534286_p40644606152226"><a name="zh-cn_topic_0201534286_p40644606152226"></a><a name="zh-cn_topic_0201534286_p40644606152226"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534286_p3878783152226"><a name="zh-cn_topic_0201534286_p3878783152226"></a><a name="zh-cn_topic_0201534286_p3878783152226"></a><a href="#zh-cn_topic_0201534286_table23403840">publicip</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.18%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0201534286_p9060565152226"><a name="zh-cn_topic_0201534286_p9060565152226"></a><a name="zh-cn_topic_0201534286_p9060565152226"></a><span id="zh-cn_topic_0201534286_text442483841316"><a name="zh-cn_topic_0201534286_text442483841316"></a><a name="zh-cn_topic_0201534286_text442483841316"></a></span><span id="zh-cn_topic_0201534286_text16424138181315"><a name="zh-cn_topic_0201534286_text16424138181315"></a><a name="zh-cn_topic_0201534286_text16424138181315"></a>弹性公网IP</span>对象，请参见<a href="#zh-cn_topic_0201534286_table23403840">表3</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  publicip字段说明

    <a name="zh-cn_topic_0201534286_table23403840"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534286_row4798296"><th class="cellrowborder" valign="top" width="15.35%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0201534286_p53117702"><a name="zh-cn_topic_0201534286_p53117702"></a><a name="zh-cn_topic_0201534286_p53117702"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.11%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0201534286_p7566645"><a name="zh-cn_topic_0201534286_p7566645"></a><a name="zh-cn_topic_0201534286_p7566645"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.6%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0201534286_p3809944218819"><a name="zh-cn_topic_0201534286_p3809944218819"></a><a name="zh-cn_topic_0201534286_p3809944218819"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.94%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0201534286_p8918541"><a name="zh-cn_topic_0201534286_p8918541"></a><a name="zh-cn_topic_0201534286_p8918541"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534286_row51313205"><td class="cellrowborder" valign="top" width="15.35%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534286_p62728917"><a name="zh-cn_topic_0201534286_p62728917"></a><a name="zh-cn_topic_0201534286_p62728917"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534286_p47877526"><a name="zh-cn_topic_0201534286_p47877526"></a><a name="zh-cn_topic_0201534286_p47877526"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.6%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534286_p6615596018819"><a name="zh-cn_topic_0201534286_p6615596018819"></a><a name="zh-cn_topic_0201534286_p6615596018819"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.94%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534286_ul1580299162914"></a><a name="zh-cn_topic_0201534286_ul1580299162914"></a><ul id="zh-cn_topic_0201534286_ul1580299162914"><li>功能说明：端口id。</li><li>约束：必须是存在的端口id，如果不带该参数或者值为空时为解除绑定<span id="zh-cn_topic_0201534286_text11296114151312"><a name="zh-cn_topic_0201534286_text11296114151312"></a><a name="zh-cn_topic_0201534286_text11296114151312"></a></span><span id="zh-cn_topic_0201534286_text5296134101313"><a name="zh-cn_topic_0201534286_text5296134101313"></a><a name="zh-cn_topic_0201534286_text5296134101313"></a>弹性公网IP</span>，如果该端口不存在或端口已绑定<span id="zh-cn_topic_0201534286_text180394391310"><a name="zh-cn_topic_0201534286_text180394391310"></a><a name="zh-cn_topic_0201534286_text180394391310"></a></span><span id="zh-cn_topic_0201534286_text118032432136"><a name="zh-cn_topic_0201534286_text118032432136"></a><a name="zh-cn_topic_0201534286_text118032432136"></a>弹性公网IP</span>则会提示出错，和ip_version字段互斥，不能同时更新。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row126751018141713"><td class="cellrowborder" valign="top" width="15.35%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534286_p23901530141713"><a name="zh-cn_topic_0201534286_p23901530141713"></a><a name="zh-cn_topic_0201534286_p23901530141713"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534286_p17391163017175"><a name="zh-cn_topic_0201534286_p17391163017175"></a><a name="zh-cn_topic_0201534286_p17391163017175"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.6%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534286_p13391130151713"><a name="zh-cn_topic_0201534286_p13391130151713"></a><a name="zh-cn_topic_0201534286_p13391130151713"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.94%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534286_ul181841019112919"></a><a name="zh-cn_topic_0201534286_ul181841019112919"></a><ul id="zh-cn_topic_0201534286_ul181841019112919"><li>功能说明：IP版本信息。</li><li>取值范围：4和6<a name="zh-cn_topic_0201534286_ul9525142083711"></a><a name="zh-cn_topic_0201534286_ul9525142083711"></a><ul id="zh-cn_topic_0201534286_ul9525142083711"><li>4：IPv4</li><li>6：IPv6</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534286_ul11875851417"></a><a name="zh-cn_topic_0201534286_ul11875851417"></a><ul id="zh-cn_topic_0201534286_ul11875851417"><li>必须是系统支持的IP版本类型</li><li>和port_id互斥：不能同时设置port_id和ip_version字段。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row9838194915408"><td class="cellrowborder" valign="top" width="15.35%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0201534286_p19833814131013"><a name="zh-cn_topic_0201534286_p19833814131013"></a><a name="zh-cn_topic_0201534286_p19833814131013"></a>alias</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.11%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0201534286_p2083301414101"><a name="zh-cn_topic_0201534286_p2083301414101"></a><a name="zh-cn_topic_0201534286_p2083301414101"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.6%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0201534286_p1883381418108"><a name="zh-cn_topic_0201534286_p1883381418108"></a><a name="zh-cn_topic_0201534286_p1883381418108"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.94%" headers="mcps1.2.5.1.4 "><a name="zh-cn_topic_0201534286_ul17228652131119"></a><a name="zh-cn_topic_0201534286_ul17228652131119"></a><ul id="zh-cn_topic_0201534286_ul17228652131119"><li>功能说明：弹性公网IP名称</li><li>取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例1（EIP绑定一张网卡）

    ```
    PUT https://{Endpoint}/v1/{project_id}/publicips/{publicip_id}
    
    {
        "publicip": {
            "port_id": "f588ccfa-8750-4d7c-bf5d-2ede24414706"
        }
    }
    ```


-   请求样例2（转换为IPv6 EIP）

    ```
    PUT https://{Endpoint}/v1/{project_id}/publicips/{publicip_id}
    
    {
        "publicip": {
            "ip_version ": 6 
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0201534286_section34213098"></a>

-   响应参数

    **表 4**  响应参数

    <a name="zh-cn_topic_0201534286_table32985183152250"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534286_row10178394152250"><th class="cellrowborder" valign="top" width="18.34%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534286_p19143548152250"><a name="zh-cn_topic_0201534286_p19143548152250"></a><a name="zh-cn_topic_0201534286_p19143548152250"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.509999999999998%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534286_p40138407152250"><a name="zh-cn_topic_0201534286_p40138407152250"></a><a name="zh-cn_topic_0201534286_p40138407152250"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.15%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534286_p29985535152250"><a name="zh-cn_topic_0201534286_p29985535152250"></a><a name="zh-cn_topic_0201534286_p29985535152250"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534286_row12909284152250"><td class="cellrowborder" valign="top" width="18.34%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p39019069152250"><a name="zh-cn_topic_0201534286_p39019069152250"></a><a name="zh-cn_topic_0201534286_p39019069152250"></a>publicip</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.509999999999998%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p50907501152250"><a name="zh-cn_topic_0201534286_p50907501152250"></a><a name="zh-cn_topic_0201534286_p50907501152250"></a><a href="#zh-cn_topic_0201534286_table83964341880">publicip</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.15%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p366643152250"><a name="zh-cn_topic_0201534286_p366643152250"></a><a name="zh-cn_topic_0201534286_p366643152250"></a><span id="zh-cn_topic_0201534286_text2082852181316"><a name="zh-cn_topic_0201534286_text2082852181316"></a><a name="zh-cn_topic_0201534286_text2082852181316"></a></span><span id="zh-cn_topic_0201534286_text782552191316"><a name="zh-cn_topic_0201534286_text782552191316"></a><a name="zh-cn_topic_0201534286_text782552191316"></a>弹性公网IP</span>对象，请参见<a href="#zh-cn_topic_0201534286_table83964341880">表5</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  publicip字段说明

    <a name="zh-cn_topic_0201534286_table83964341880"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534286_row608739661880"><th class="cellrowborder" valign="top" width="18.318168183181683%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534286_p318442431880"><a name="zh-cn_topic_0201534286_p318442431880"></a><a name="zh-cn_topic_0201534286_p318442431880"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.82741725827417%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534286_p201897271880"><a name="zh-cn_topic_0201534286_p201897271880"></a><a name="zh-cn_topic_0201534286_p201897271880"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.85441455854414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534286_p247551571880"><a name="zh-cn_topic_0201534286_p247551571880"></a><a name="zh-cn_topic_0201534286_p247551571880"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534286_row590107001880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p151373871880"><a name="zh-cn_topic_0201534286_p151373871880"></a><a name="zh-cn_topic_0201534286_p151373871880"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p623914921880"><a name="zh-cn_topic_0201534286_p623914921880"></a><a name="zh-cn_topic_0201534286_p623914921880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p205460611880"><a name="zh-cn_topic_0201534286_p205460611880"></a><a name="zh-cn_topic_0201534286_p205460611880"></a><span id="zh-cn_topic_0201534286_text1480155511314"><a name="zh-cn_topic_0201534286_text1480155511314"></a><a name="zh-cn_topic_0201534286_text1480155511314"></a></span><span id="zh-cn_topic_0201534286_text16481555171315"><a name="zh-cn_topic_0201534286_text16481555171315"></a><a name="zh-cn_topic_0201534286_text16481555171315"></a>弹性公网IP</span>唯一标识</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row506968211880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p128018091880"><a name="zh-cn_topic_0201534286_p128018091880"></a><a name="zh-cn_topic_0201534286_p128018091880"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p394853281880"><a name="zh-cn_topic_0201534286_p394853281880"></a><a name="zh-cn_topic_0201534286_p394853281880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul263945115243"></a><a name="zh-cn_topic_0201534286_ul263945115243"></a><ul id="zh-cn_topic_0201534286_ul263945115243"><li>功能说明：<span id="zh-cn_topic_0201534286_text4273258121317"><a name="zh-cn_topic_0201534286_text4273258121317"></a><a name="zh-cn_topic_0201534286_text4273258121317"></a></span><span id="zh-cn_topic_0201534286_text15273458151319"><a name="zh-cn_topic_0201534286_text15273458151319"></a><a name="zh-cn_topic_0201534286_text15273458151319"></a>弹性公网IP</span>的状态</li><li>取值范围：<a name="zh-cn_topic_0201534286_ul7905205815810"></a><a name="zh-cn_topic_0201534286_ul7905205815810"></a><ul id="zh-cn_topic_0201534286_ul7905205815810"><li>FREEZED：冻结</li><li>BIND_ERROR：绑定失败</li><li>BINDING：绑定中</li><li>PENDING_DELETE：释放中</li><li>PENDING_CREATE：创建中</li><li>PENDING_UPDATE：更新中</li><li>DOWN：未绑定</li><li>ACTIVE：绑定</li><li>ELB：绑定ELB</li><li>ERROR：异常失败</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row16130133562319"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p09743162419"><a name="zh-cn_topic_0201534286_p09743162419"></a><a name="zh-cn_topic_0201534286_p09743162419"></a>profile</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p12971231132410"><a name="zh-cn_topic_0201534286_p12971231132410"></a><a name="zh-cn_topic_0201534286_p12971231132410"></a><a href="#zh-cn_topic_0201534286_table66651219193417">profile</a> object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p5644118182514"><a name="zh-cn_topic_0201534286_p5644118182514"></a><a name="zh-cn_topic_0201534286_p5644118182514"></a>功能说明：额外参数，包括订单id、产品id等信息，详情请参见<a href="#zh-cn_topic_0201534286_table66651219193417">表6</a>。</p>
    <p id="zh-cn_topic_0201534286_p16644118152519"><a name="zh-cn_topic_0201534286_p16644118152519"></a><a name="zh-cn_topic_0201534286_p16644118152519"></a>约束：如果profile不为空，说明是包周期的<span id="zh-cn_topic_0201534286_text1242916461411"><a name="zh-cn_topic_0201534286_text1242916461411"></a><a name="zh-cn_topic_0201534286_text1242916461411"></a></span><span id="zh-cn_topic_0201534286_text1542911419140"><a name="zh-cn_topic_0201534286_text1542911419140"></a><a name="zh-cn_topic_0201534286_text1542911419140"></a>弹性公网IP</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row230260811880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p30749271"><a name="zh-cn_topic_0201534286_p30749271"></a><a name="zh-cn_topic_0201534286_p30749271"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p379401841880"><a name="zh-cn_topic_0201534286_p379401841880"></a><a name="zh-cn_topic_0201534286_p379401841880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul7176216121014"></a><a name="zh-cn_topic_0201534286_ul7176216121014"></a><ul id="zh-cn_topic_0201534286_ul7176216121014"><li>功能说明：<span id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text941224173012"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text941224173012"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text941224173012"></a></span><span id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4412641113015"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4412641113015"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4412641113015"></a>弹性公网IP</span>的类型</li><li>取值范围：<em id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i16850184017499"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i16850184017499"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i16850184017499"></a>5_telcom（电信），5_union（联通），5_bgp（全动态BGP），5_sbgp（静态BGP）</em><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul585004064911"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul585004064911"></a><ul id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul585004064911"><li>东北-大连：5_telcom、5_union</li><li>华南-广州：5_bgp、5_sbgp</li><li>华东-上海一：<em id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i541911467911"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i541911467911"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_i541911467911"></a>5_bgp</em>、5_sbgp</li><li>华东-上海二：5_bgp、5_sbgp</li><li>华北-北京一：5_bgp、5_sbgp</li><li><span id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4018327273"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4018327273"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_text4018327273"></a>中国-香港</span>：5_bgp</li><li>亚太-曼谷：5_bgp</li><li>亚太-新加坡：5_bgp</li><li>非洲-约翰内斯堡：5_bgp</li><li>西南-贵阳一：5_sbgp</li><li>华北-北京四：5_bgp、5_sbgp</li><li>拉美-圣地亚哥：5_bgp</li><li>拉美-圣保罗一：5_bgp</li><li>拉美-墨西哥城一：5_bgp</li><li>拉美-布宜诺斯艾利一：5_bgp</li><li>拉美-利马一：5_bgp</li><li>拉美-圣地亚哥二：5_bgp</li></ul>
    </li><li>约束：<a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul9738153015499"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul9738153015499"></a><ul id="zh-cn_topic_0201534286_zh-cn_topic_0201534274_ul9738153015499"><li>必须是系统具体支持的类型</li><li>publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row389218135338"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p3576115214619"><a name="zh-cn_topic_0201534286_p3576115214619"></a><a name="zh-cn_topic_0201534286_p3576115214619"></a>public_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p35761552124618"><a name="zh-cn_topic_0201534286_p35761552124618"></a><a name="zh-cn_topic_0201534286_p35761552124618"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p19576252174619"><a name="zh-cn_topic_0201534286_p19576252174619"></a><a name="zh-cn_topic_0201534286_p19576252174619"></a>IPv4时是申请到的<span id="zh-cn_topic_0201534286_text817712711146"><a name="zh-cn_topic_0201534286_text817712711146"></a><a name="zh-cn_topic_0201534286_text817712711146"></a></span><span id="zh-cn_topic_0201534286_text31771927201410"><a name="zh-cn_topic_0201534286_text31771927201410"></a><a name="zh-cn_topic_0201534286_text31771927201410"></a>弹性公网IP</span>地址，IPv6时是IPv6地址对应的IPv4地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row6663943910"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p117521510894"><a name="zh-cn_topic_0201534286_p117521510894"></a><a name="zh-cn_topic_0201534286_p117521510894"></a>public_ipv6_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p97524108911"><a name="zh-cn_topic_0201534286_p97524108911"></a><a name="zh-cn_topic_0201534286_p97524108911"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p167581149102812"><a name="zh-cn_topic_0201534286_p167581149102812"></a><a name="zh-cn_topic_0201534286_p167581149102812"></a>IPv4时无此字段，IPv6时为申请到的<span id="zh-cn_topic_0201534286_text714903514150"><a name="zh-cn_topic_0201534286_text714903514150"></a><a name="zh-cn_topic_0201534286_text714903514150"></a></span><span id="zh-cn_topic_0201534286_text0149435121516"><a name="zh-cn_topic_0201534286_text0149435121516"></a><a name="zh-cn_topic_0201534286_text0149435121516"></a>弹性公网IP</span>地址</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row2030210714336"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p5577105234617"><a name="zh-cn_topic_0201534286_p5577105234617"></a><a name="zh-cn_topic_0201534286_p5577105234617"></a>ip_version</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p2577165217467"><a name="zh-cn_topic_0201534286_p2577165217467"></a><a name="zh-cn_topic_0201534286_p2577165217467"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p10645141832513"><a name="zh-cn_topic_0201534286_p10645141832513"></a><a name="zh-cn_topic_0201534286_p10645141832513"></a>IP版本信息，取值范围是4和6</p>
    <a name="zh-cn_topic_0201534286_ul13987110227"></a><a name="zh-cn_topic_0201534286_ul13987110227"></a><ul id="zh-cn_topic_0201534286_ul13987110227"><li>4：表示IPv4</li><li>6：表示IPv6</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row283940631880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p182177951880"><a name="zh-cn_topic_0201534286_p182177951880"></a><a name="zh-cn_topic_0201534286_p182177951880"></a>private_ip_address</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p60695041880"><a name="zh-cn_topic_0201534286_p60695041880"></a><a name="zh-cn_topic_0201534286_p60695041880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul1693412582014"></a><a name="zh-cn_topic_0201534286_ul1693412582014"></a><ul id="zh-cn_topic_0201534286_ul1693412582014"><li>功能说明：绑定<span id="zh-cn_topic_0201534286_text28951341151511"><a name="zh-cn_topic_0201534286_text28951341151511"></a><a name="zh-cn_topic_0201534286_text28951341151511"></a></span><span id="zh-cn_topic_0201534286_text198953415153"><a name="zh-cn_topic_0201534286_text198953415153"></a><a name="zh-cn_topic_0201534286_text198953415153"></a>弹性公网IP</span>的私有IP地址</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534286_text1879311449153"><a name="zh-cn_topic_0201534286_text1879311449153"></a><a name="zh-cn_topic_0201534286_text1879311449153"></a></span><span id="zh-cn_topic_0201534286_text1779316449153"><a name="zh-cn_topic_0201534286_text1779316449153"></a><a name="zh-cn_topic_0201534286_text1779316449153"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row264614551880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p630030811880"><a name="zh-cn_topic_0201534286_p630030811880"></a><a name="zh-cn_topic_0201534286_p630030811880"></a>port_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p397229231880"><a name="zh-cn_topic_0201534286_p397229231880"></a><a name="zh-cn_topic_0201534286_p397229231880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul420471472010"></a><a name="zh-cn_topic_0201534286_ul420471472010"></a><ul id="zh-cn_topic_0201534286_ul420471472010"><li>功能说明：端口id。</li><li>约束：只有绑定了的<span id="zh-cn_topic_0201534286_text144209488151"><a name="zh-cn_topic_0201534286_text144209488151"></a><a name="zh-cn_topic_0201534286_text144209488151"></a></span><span id="zh-cn_topic_0201534286_text54209481153"><a name="zh-cn_topic_0201534286_text54209481153"></a><a name="zh-cn_topic_0201534286_text54209481153"></a>弹性公网IP</span>查询才会返回该参数</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row340905521880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p98713501880"><a name="zh-cn_topic_0201534286_p98713501880"></a><a name="zh-cn_topic_0201534286_p98713501880"></a>tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p58747301880"><a name="zh-cn_topic_0201534286_p58747301880"></a><a name="zh-cn_topic_0201534286_p58747301880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p269114516312"><a name="zh-cn_topic_0201534286_p269114516312"></a><a name="zh-cn_topic_0201534286_p269114516312"></a>项目ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row548200921880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p112424711880"><a name="zh-cn_topic_0201534286_p112424711880"></a><a name="zh-cn_topic_0201534286_p112424711880"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p92119381880"><a name="zh-cn_topic_0201534286_p92119381880"></a><a name="zh-cn_topic_0201534286_p92119381880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p36292894"><a name="zh-cn_topic_0201534286_p36292894"></a><a name="zh-cn_topic_0201534286_p36292894"></a><span id="zh-cn_topic_0201534286_text1175715325168"><a name="zh-cn_topic_0201534286_text1175715325168"></a><a name="zh-cn_topic_0201534286_text1175715325168"></a></span><span id="zh-cn_topic_0201534286_text075733212164"><a name="zh-cn_topic_0201534286_text075733212164"></a><a name="zh-cn_topic_0201534286_text075733212164"></a>弹性公网IP</span>申请时间（UTC）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row46164031880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p383843571880"><a name="zh-cn_topic_0201534286_p383843571880"></a><a name="zh-cn_topic_0201534286_p383843571880"></a>bandwidth_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p473107141880"><a name="zh-cn_topic_0201534286_p473107141880"></a><a name="zh-cn_topic_0201534286_p473107141880"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p3934181618641"><a name="zh-cn_topic_0201534286_p3934181618641"></a><a name="zh-cn_topic_0201534286_p3934181618641"></a><span id="zh-cn_topic_0201534286_text334073671610"><a name="zh-cn_topic_0201534286_text334073671610"></a><a name="zh-cn_topic_0201534286_text334073671610"></a></span><span id="zh-cn_topic_0201534286_text13402366164"><a name="zh-cn_topic_0201534286_text13402366164"></a><a name="zh-cn_topic_0201534286_text13402366164"></a>弹性公网IP</span>对应带宽ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row626637421880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p425983371880"><a name="zh-cn_topic_0201534286_p425983371880"></a><a name="zh-cn_topic_0201534286_p425983371880"></a>bandwidth_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p463832691880"><a name="zh-cn_topic_0201534286_p463832691880"></a><a name="zh-cn_topic_0201534286_p463832691880"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p2365466"><a name="zh-cn_topic_0201534286_p2365466"></a><a name="zh-cn_topic_0201534286_p2365466"></a>带宽大小，单位为Mbit/s。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row576448061880"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p387177161880"><a name="zh-cn_topic_0201534286_p387177161880"></a><a name="zh-cn_topic_0201534286_p387177161880"></a>bandwidth_share_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p21369006155933"><a name="zh-cn_topic_0201534286_p21369006155933"></a><a name="zh-cn_topic_0201534286_p21369006155933"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul2255712095"></a><a name="zh-cn_topic_0201534286_ul2255712095"></a><ul id="zh-cn_topic_0201534286_ul2255712095"><li>功能说明：<span id="zh-cn_topic_0201534286_text111001423131619"><a name="zh-cn_topic_0201534286_text111001423131619"></a><a name="zh-cn_topic_0201534286_text111001423131619"></a></span><span id="zh-cn_topic_0201534286_text310011232164"><a name="zh-cn_topic_0201534286_text310011232164"></a><a name="zh-cn_topic_0201534286_text310011232164"></a>弹性公网IP</span>的带宽类型</li><li>取值范围：PER，WHOLE。<a name="zh-cn_topic_0201534286_ul729412507220"></a><a name="zh-cn_topic_0201534286_ul729412507220"></a><ul id="zh-cn_topic_0201534286_ul729412507220"><li>PER：独享带宽</li><li>WHOLE：共享带宽</li></ul>
    </li></ul>
    <a name="zh-cn_topic_0201534286_ul1369035014203"></a><a name="zh-cn_topic_0201534286_ul1369035014203"></a><ul id="zh-cn_topic_0201534286_ul1369035014203"><li>约束：其中IPv6暂不支持WHOLE类型带宽。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row1444049321927"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p605297721941"><a name="zh-cn_topic_0201534286_p605297721941"></a><a name="zh-cn_topic_0201534286_p605297721941"></a>bandwidth_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p5224891921941"><a name="zh-cn_topic_0201534286_p5224891921941"></a><a name="zh-cn_topic_0201534286_p5224891921941"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p374970718414"><a name="zh-cn_topic_0201534286_p374970718414"></a><a name="zh-cn_topic_0201534286_p374970718414"></a>带宽名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row12157418184110"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p979842771215"><a name="zh-cn_topic_0201534286_p979842771215"></a><a name="zh-cn_topic_0201534286_p979842771215"></a>alias</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p137987278128"><a name="zh-cn_topic_0201534286_p137987278128"></a><a name="zh-cn_topic_0201534286_p137987278128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p175531744191218"><a name="zh-cn_topic_0201534286_p175531744191218"></a><a name="zh-cn_topic_0201534286_p175531744191218"></a>弹性公网IP名称</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row1353343333617"><td class="cellrowborder" valign="top" width="18.318168183181683%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p19564181313543"><a name="zh-cn_topic_0201534286_p19564181313543"></a><a name="zh-cn_topic_0201534286_p19564181313543"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.82741725827417%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p13564413185412"><a name="zh-cn_topic_0201534286_p13564413185412"></a><a name="zh-cn_topic_0201534286_p13564413185412"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.85441455854414%" headers="mcps1.2.4.1.3 "><a name="zh-cn_topic_0201534286_ul184004104214"></a><a name="zh-cn_topic_0201534286_ul184004104214"></a><ul id="zh-cn_topic_0201534286_ul184004104214"><li>企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。</li><li>创建弹性公网IP时，给弹性公网IP绑定企业项目ID。</li><li>不指定该参数时，默认值是 0，0表示默认企业项目。</li></ul>
    <div class="note" id="zh-cn_topic_0201534286_note19041412125118"><a name="zh-cn_topic_0201534286_note19041412125118"></a><a name="zh-cn_topic_0201534286_note19041412125118"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0201534286_zh-cn_topic_0201534275_p1915862704914"><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534275_p1915862704914"></a><a name="zh-cn_topic_0201534286_zh-cn_topic_0201534275_p1915862704914"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0126101490.html" target="_blank" rel="noopener noreferrer">《企业管理用户指南》</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    **表 6**  profile字段说明

    <a name="zh-cn_topic_0201534286_table66651219193417"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0201534286_row167319197349"><th class="cellrowborder" valign="top" width="18.54%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0201534286_p206761195347"><a name="zh-cn_topic_0201534286_p206761195347"></a><a name="zh-cn_topic_0201534286_p206761195347"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.740000000000002%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0201534286_p156812193344"><a name="zh-cn_topic_0201534286_p156812193344"></a><a name="zh-cn_topic_0201534286_p156812193344"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.720000000000006%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0201534286_p17684101933410"><a name="zh-cn_topic_0201534286_p17684101933410"></a><a name="zh-cn_topic_0201534286_p17684101933410"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0201534286_row962259102216"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p962309182220"><a name="zh-cn_topic_0201534286_p962309182220"></a><a name="zh-cn_topic_0201534286_p962309182220"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.740000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p136231597223"><a name="zh-cn_topic_0201534286_p136231597223"></a><a name="zh-cn_topic_0201534286_p136231597223"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.720000000000006%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p26235912225"><a name="zh-cn_topic_0201534286_p26235912225"></a><a name="zh-cn_topic_0201534286_p26235912225"></a>订单的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row18686141920341"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p11688201923418"><a name="zh-cn_topic_0201534286_p11688201923418"></a><a name="zh-cn_topic_0201534286_p11688201923418"></a>product_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.740000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p169318196347"><a name="zh-cn_topic_0201534286_p169318196347"></a><a name="zh-cn_topic_0201534286_p169318196347"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.720000000000006%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p149921832153419"><a name="zh-cn_topic_0201534286_p149921832153419"></a><a name="zh-cn_topic_0201534286_p149921832153419"></a>产品的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row167161319173418"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p5718101903412"><a name="zh-cn_topic_0201534286_p5718101903412"></a><a name="zh-cn_topic_0201534286_p5718101903412"></a>region_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.740000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p47241019143417"><a name="zh-cn_topic_0201534286_p47241019143417"></a><a name="zh-cn_topic_0201534286_p47241019143417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.720000000000006%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p09201951174716"><a name="zh-cn_topic_0201534286_p09201951174716"></a><a name="zh-cn_topic_0201534286_p09201951174716"></a>region的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0201534286_row1472971912347"><td class="cellrowborder" valign="top" width="18.54%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0201534286_p187311719103415"><a name="zh-cn_topic_0201534286_p187311719103415"></a><a name="zh-cn_topic_0201534286_p187311719103415"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.740000000000002%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0201534286_p9735141923418"><a name="zh-cn_topic_0201534286_p9735141923418"></a><a name="zh-cn_topic_0201534286_p9735141923418"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.720000000000006%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0201534286_p27381919173415"><a name="zh-cn_topic_0201534286_p27381919173415"></a><a name="zh-cn_topic_0201534286_p27381919173415"></a>用户的id</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例1（EIP绑定一张网卡）

    ```
    {
      "publicip": {
        "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb",
        "status": "ACTIVE",
        "type": "5_bgp",
        "port_id": "a135e9b8-1630-40d2-a6c5-eb534a61efbe",
        "public_ip_address": "10.xx.xx.162",
        "private_ip_address": "192.168.1.131",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-03-27 01:33:18",
        "bandwidth_size": 7,
        "ip_version": 4
      }
    }
    ```


-   响应样例2（转换为IPv6 EIP）

    ```
    {
      "publicip": {
        "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb",
        "status": "DOWN",
        "type": "5_bgp",
        "public_ip_address": "10.xx.xx.162",
        "public_ipv6_address": "cdcd:xx:xx:xx::a9a:4aa2",
        "tenant_id": "26ae5181a416420998eb2093aaed84d9",
        "create_time": "2019-03-27 01:33:18",
        "bandwidth_size": 7,
        "ip_version": 6
      }
    }
    ```


## 状态码<a name="zh-cn_topic_0201534286_section31981619"></a>

请参见[状态码](状态码.md#eip_api05_0001)。

## 错误码<a name="zh-cn_topic_0201534286_section85821649202813"></a>

请参考[错误码](错误码.md)。

