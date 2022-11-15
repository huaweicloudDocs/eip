# IPv6转换（申请/释放IPv6弹性公网IP）<a name="eip_0006_02"></a>

## 操作场景<a name="section35171201192"></a>

如果您想使部署应用的ECS面向Internet客户端提供IPv6服务，但您的ECS规格不支持IPv6网络，或者您不想通过搭建IPv6网络来实现该需求，那么您可以通过弹性公网IP的IPv6转换功能来快速实现该能力。

## 开启IPv6转换（申请IPv6弹性公网IP）<a name="zh-cn_topic_0128773070_section1951010207215"></a>

-   方法一：

    参考[申请弹性公网IP](申请弹性公网IP.md)来申请弹性公网IP，在申请页面配置参数时，请将“IPv6转换”设置为“开启”，就可以在申请IPv4地址的同时申请一个IPv6弹性公网IP。

    开启IPv6转换后，该弹性公网IP将同时拥有IPv4和IPv6地址，原有IPv4业务可以快速为IPv6用户提供访问能力。

-   方法二：

    当已有的IPv4地址的弹性公网IP需要增加IPv6地址时，可以在弹性公网IP列表页面，找到想转换的IPv4弹性公网IP ，单击操作列“更多”下的“开启IPv6转换”，即可将已有的IPv4弹性公网IP转换为IPv6的。

    开启IPv6转换后，该弹性公网IP将同时拥有IPv4和IPv6地址，原有IPv4业务可以快速为IPv6用户提供访问能力。


>![](public_sys-resources/icon-note.gif) **说明：** 
>开启IPv6转换后，对原有绑定资源的使用无影响。
>目前，支持开启IPv6转换的区域有：华北-北京一、华北-北京四、华东-上海一、华东-上海二、华南-广州。

## 配置安全组<a name="zh-cn_topic_0128773070_section183541933911"></a>

开启弹性公网IP的IPv6转换后，请务必在安全组的出方向和入方向中放通198.19.0.0/16网段的IP地址，如[表1](#zh-cn_topic_0128773070_table854766319358)所示。因为IPv6 弹性公网IP采用NAT64技术，入方向的源IP地址经过NAT64转换后，会将IPv6地址转换为198.19.0.0/16之间的某个IPv4地址，源端口随机，目的IP为本机的内部私有IPv4地址，目的端口不变。

配置安全组操作请参考[《虚拟私有云用户指南》](https://support.huaweicloud.com/usermanual-vpc/zh-cn_topic_0030969470.html)。

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

## 关闭IPv6转换（释放IPv6弹性公网IP）<a name="zh-cn_topic_0128773070_section86833287319"></a>

当弹性公网IP不再需要IPv6地址时，可以在弹性公网IP列表页面，找到想关闭IPv6地址的弹性公网IP ，单击“操作”列的“关闭IPv6转换”，即可删除IPv6地址。删除后，该弹性公网IP仅保留IPv4地址。

