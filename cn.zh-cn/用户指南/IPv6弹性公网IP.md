# IPv6弹性公网IP<a name="eip_0006"></a>

## 简介<a name="zh-cn_topic_0128773070_section298043619513"></a>

弹性公网IP支持IPv4地址和IPv6地址，您可以申请一个全新的IPv6弹性公网IP，也可以将已有的IPv4弹性公网IP转换为IPv6的。

开启IPv6转换后，将提供IPv4和IPv6弹性公网IP地址，原有IPv4业务可以快速为IPv6用户提供访问能力。

IPv6弹性公网IP当前暂不收费，后续将择时收费。

## 应用场景<a name="zh-cn_topic_0128773070_section6903103318162"></a>

如果您的应用需要为使用IPv6终端的用户提供访问服务，则您可使用：IPv6弹性公网IP。

如果您的应用既需要为使用IPv6终端的用户提供访问服务，又需要对这些访问来源进行数据分析处理，则您必须使用IPv6双栈。使用IPv6双栈请参考[IPv4/IPv6双栈网络](https://support.huaweicloud.com/usermanual-vpc/vpc_0002.html)。

如果您的应用系统与其他系统（例如：数据库系统）、应用系统之间需要使用IPv6进行内网访问，则您必须使用IPv6双栈。使用IPv6双栈请参考[IPv4/IPv6双栈网络](https://support.huaweicloud.com/usermanual-vpc/vpc_0002.html)。

## 申请IPv6弹性公网IP<a name="zh-cn_topic_0128773070_section011625114590"></a>

参考[申请弹性公网IP](申请弹性公网IP.md)申请弹性公网IP，在申请页面配置参数时，请将“IPv6转换”设置为“开启”，就可以申请一个全新的IPv6弹性公网IP。

## 开启IPv6转换<a name="zh-cn_topic_0128773070_section1951010207215"></a>

当已有的IPv4地址的弹性公网IP需要增加IPv6地址时，可以在弹性公网IP列表页面，找到想转换的IPv4地址弹性公网IP ，单击“操作”列的“开启IPv6转换”，即可将已有的IPv4弹性公网IP转换为IPv6的。转换后，该弹性公网IP将同时拥有IPv4和IPv6地址。

>![](public_sys-resources/icon-note.gif) **说明：** 
>开启IPv6转换后，对原有绑定资源的使用无影响。

## 配置安全组<a name="zh-cn_topic_0128773070_section183541933911"></a>

开启弹性公网IP的IPv6转换后，请务必在安全组的出方向和入方向中放通198.19.0.0/16网段的IP地址，如[表1](#zh-cn_topic_0128773070_table854766319358)所示。因为IPv6 弹性公网IP采用NAT64技术，入方向的源IP地址经过NAT64转换后，会从IPv6地址转换为198.19.0.0/16之间的某个IPv4地址，源端口随机，目的IP为本机的内部私有IPv4地址，目的端口不变。

**表 1**  安全组规则

<a name="zh-cn_topic_0128773070_table854766319358"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128773070_row2051403019358"><th class="cellrowborder" valign="top" width="19.681968196819682%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0128773070_p5102371419358"><a name="zh-cn_topic_0128773070_p5102371419358"></a><a name="zh-cn_topic_0128773070_p5102371419358"></a>方向</p>
</th>
<th class="cellrowborder" valign="top" width="20.782078207820785%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0128773070_p3928016319358"><a name="zh-cn_topic_0128773070_p3928016319358"></a><a name="zh-cn_topic_0128773070_p3928016319358"></a>协议</p>
</th>
<th class="cellrowborder" valign="top" width="59.53595359535954%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0128773070_p2415644494621"><a name="zh-cn_topic_0128773070_p2415644494621"></a><a name="zh-cn_topic_0128773070_p2415644494621"></a>端口和地址</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128773070_row3779122419358"><td class="cellrowborder" valign="top" width="19.681968196819682%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0128773070_p4119033619358"><a name="zh-cn_topic_0128773070_p4119033619358"></a><a name="zh-cn_topic_0128773070_p4119033619358"></a>入方向</p>
</td>
<td class="cellrowborder" valign="top" width="20.782078207820785%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0128773070_p4808290419358"><a name="zh-cn_topic_0128773070_p4808290419358"></a><a name="zh-cn_topic_0128773070_p4808290419358"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="59.53595359535954%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0128773070_p4640703694621"><a name="zh-cn_topic_0128773070_p4640703694621"></a><a name="zh-cn_topic_0128773070_p4640703694621"></a>源地址：198.19.0.0/16</p>
</td>
</tr>
<tr id="zh-cn_topic_0128773070_row22818581398"><td class="cellrowborder" valign="top" width="19.681968196819682%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0128773070_p6301958495"><a name="zh-cn_topic_0128773070_p6301958495"></a><a name="zh-cn_topic_0128773070_p6301958495"></a>出方向</p>
</td>
<td class="cellrowborder" valign="top" width="20.782078207820785%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0128773070_p730158994"><a name="zh-cn_topic_0128773070_p730158994"></a><a name="zh-cn_topic_0128773070_p730158994"></a>全部</p>
</td>
<td class="cellrowborder" valign="top" width="59.53595359535954%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0128773070_p7825131612103"><a name="zh-cn_topic_0128773070_p7825131612103"></a><a name="zh-cn_topic_0128773070_p7825131612103"></a>目的地址：198.19.0.0/16</p>
</td>
</tr>
</tbody>
</table>

## 关闭IPv6转换<a name="zh-cn_topic_0128773070_section86833287319"></a>

当弹性公网IP不需要IPv6地址时，可以在弹性公网IP列表页面，找到想关闭IPv6地址的弹性公网IP ，单击“操作”列的“关闭IPv6转换”，即可删除IPv6地址。删除后，该弹性公网IP仅保留IPv4地址。

