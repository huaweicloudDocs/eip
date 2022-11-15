# IPv6概述<a name="eip_0006_01"></a>

## 简介<a name="zh-cn_topic_0128773070_section298043619513"></a>

弹性公网IP支持IPv4地址和IPv6地址，您可以申请一个全新的IPv6弹性公网IP，也可以通过IPv6转换功能将已有的IPv4弹性公网IP映射为公网IPv6地址。

开启IPv6转换后，将提供IPv4和IPv6弹性公网IP地址，原有IPv4业务可以快速为IPv6用户提供访问能力。

IPv4弹性公网IP收取费用，IPv6弹性公网IP当前暂不收费，后续将择时收费。

## IPv4/IPv6双栈网络应用场景<a name="section182413208373"></a>

如果您的ECS规格支持IPv6网络，那么您可以使用IPv4/IPv6双栈网络，场景示例和资源规划如[表1](#table105590377292)所示。

**表 1**  IPv4/IPv6双栈网络的应用场景及资源规划

<a name="table105590377292"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133505069_row1455915377291"><th class="cellrowborder" valign="top" width="10.489999999999998%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0133505069_p155591237112916"><a name="zh-cn_topic_0133505069_p155591237112916"></a><a name="zh-cn_topic_0133505069_p155591237112916"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="17.59%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0133505069_p255918376297"><a name="zh-cn_topic_0133505069_p255918376297"></a><a name="zh-cn_topic_0133505069_p255918376297"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="40.38%" id="mcps1.2.6.1.3"><p id="p72488217461"><a name="p72488217461"></a><a name="p72488217461"></a>条件</p>
</th>
<th class="cellrowborder" valign="top" width="10.71%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0133505069_p14559237132910"><a name="zh-cn_topic_0133505069_p14559237132910"></a><a name="zh-cn_topic_0133505069_p14559237132910"></a>子网网段类型</p>
</th>
<th class="cellrowborder" valign="top" width="20.830000000000002%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0133505069_p105590375296"><a name="zh-cn_topic_0133505069_p105590375296"></a><a name="zh-cn_topic_0133505069_p105590375296"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="row1623913713308"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="p2531102113011"><a name="p2531102113011"></a><a name="p2531102113011"></a>IPv4内网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="p823910763016"><a name="p823910763016"></a><a name="p823910763016"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="b3598102811426"><a name="b3598102811426"></a><a name="b3598102811426"></a>IPV4</strong>进行内网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="ul2222123744117"></a><a name="ul2222123744117"></a><ul id="ul2222123744117"><li>VPC的子网未开启IPv6。</li><li>实例未绑定<span id="text371061683314"><a name="text371061683314"></a><a name="text371061683314"></a></span><span id="text0188181915330"><a name="text0188181915330"></a><a name="text0188181915330"></a>弹性公网IP</span>。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><p id="p42391178307"><a name="p42391178307"></a><a name="p42391178307"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><p id="p72391278305"><a name="p72391278305"></a><a name="p72391278305"></a><strong id="b157256983916"><a name="b157256983916"></a><a name="b157256983916"></a>IPv4私网地址：</strong>支持IPv4内网通信。</p>
</td>
</tr>
<tr id="row335801012302"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="p1053217216303"><a name="p1053217216303"></a><a name="p1053217216303"></a>IPv4公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="p10359910103013"><a name="p10359910103013"></a><a name="p10359910103013"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="b68551133174214"><a name="b68551133174214"></a><a name="b68551133174214"></a>IPV4</strong>进行公网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="ul1917195612413"></a><a name="ul1917195612413"></a><ul id="ul1917195612413"><li>VPC的子网未开启IPv6。</li><li>实例绑定<span id="text0181856104113"><a name="text0181856104113"></a><a name="text0181856104113"></a></span><span id="text19181956164110"><a name="text19181956164110"></a><a name="text19181956164110"></a>弹性公网IP</span>。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><p id="p18569197113411"><a name="p18569197113411"></a><a name="p18569197113411"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="ul121841172514"></a><a name="ul121841172514"></a><ul id="ul121841172514"><li><strong id="b1299612141059"><a name="b1299612141059"></a><a name="b1299612141059"></a>IPv4私网地址：</strong>支持IPv4内网通信。</li><li><strong id="b13705131314398"><a name="b13705131314398"></a><a name="b13705131314398"></a>IPv4公网地址：</strong>支持IPv4公网通信。</li></ul>
</td>
</tr>
<tr id="row19576052134216"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="p1957719529426"><a name="p1957719529426"></a><a name="p1957719529426"></a>IPv6内网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="p1657717526427"><a name="p1657717526427"></a><a name="p1657717526427"></a>在ECS上部署应用，需要与其他系统（比如数据库）之间使用<strong id="b9866154016423"><a name="b9866154016423"></a><a name="b9866154016423"></a>IPV6</strong>进行内网互访。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="ul588432014475"></a><a name="ul588432014475"></a><ul id="ul588432014475"><li>VPC的子网开启IPv6。</li><li>创建ECS时，网络配置如下：<a name="ul1757174118501"></a><a name="ul1757174118501"></a><ul id="ul1757174118501"><li><strong id="b1989219481537"><a name="b1989219481537"></a><a name="b1989219481537"></a>规格：</strong>选择支持IPv6网络的ECS规格。关于ECS哪些规格支持IPv6网络，请参见<a href="https://support.huaweicloud.com/productdesc-ecs/ecs_01_0019.html" target="_blank" rel="noopener noreferrer">《弹性云服务器用户指南》</a></li><li><strong id="b19667201414818"><a name="b19667201414818"></a><a name="b19667201414818"></a>VPC和子网：</strong>选择已开启IPv6的子网及子网所属的VPC。</li><li>选择“<strong id="b291301913813"><a name="b291301913813"></a><a name="b291301913813"></a>自动分配IPv6地址</strong>”。</li><li><strong id="b21401728282"><a name="b21401728282"></a><a name="b21401728282"></a>共享带宽：</strong>暂不配置。</li></ul>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><a name="ul1075885351019"></a><a name="ul1075885351019"></a><ul id="ul1075885351019"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="ul3341172910111"></a><a name="ul3341172910111"></a><ul id="ul3341172910111"><li><strong id="b139801430133718"><a name="b139801430133718"></a><a name="b139801430133718"></a>IPv4私网地址+IPv4 EIP：</strong>实例绑定IPv4 EIP，支持IPv4公网通信。</li><li><strong id="b23555252111"><a name="b23555252111"></a><a name="b23555252111"></a>IPv4私网地址：</strong>实例不绑定IPv4 EIP，支持IPv4内网通信。</li><li><strong id="b9812814195"><a name="b9812814195"></a><a name="b9812814195"></a>IPv6地址：</strong>IPv6地址不加入共享带宽，支持IPv6内网通信。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0133505069_row14559183702918"><td class="cellrowborder" valign="top" width="10.489999999999998%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0133505069_p1559103711297"><a name="zh-cn_topic_0133505069_p1559103711297"></a><a name="zh-cn_topic_0133505069_p1559103711297"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="17.59%" headers="mcps1.2.6.1.2 "><p id="p16133835171413"><a name="p16133835171413"></a><a name="p16133835171413"></a>搭建IPv6网络，使ECS可以访问Internet上的<strong id="b4341449144214"><a name="b4341449144214"></a><a name="b4341449144214"></a>IPv6</strong>服务。</p>
</td>
<td class="cellrowborder" valign="top" width="40.38%" headers="mcps1.2.6.1.3 "><a name="ul139761521161417"></a><a name="ul139761521161417"></a><ul id="ul139761521161417"><li>VPC的子网开启IPv6。</li><li>创建ECS时，网络配置如下：<a name="ul1942019095714"></a><a name="ul1942019095714"></a><ul id="ul1942019095714"><li><strong id="b197762131413"><a name="b197762131413"></a><a name="b197762131413"></a>规格：</strong>选择支持IPv6网络的ECS规格。关于ECS哪些规格支持IPv6网络，请参见<a href="https://support.huaweicloud.com/productdesc-ecs/ecs_01_0019.html" target="_blank" rel="noopener noreferrer">《弹性云服务器用户指南》</a></li><li><strong id="b19771921161410"><a name="b19771921161410"></a><a name="b19771921161410"></a>VPC和子网：</strong>选择已开启IPv6的子网及子网所属的VPC。</li><li>选择“<strong id="b1197722161420"><a name="b1197722161420"></a><a name="b1197722161420"></a>自动分配IPv6地址</strong>”。</li><li><strong id="b1797752121414"><a name="b1797752121414"></a><a name="b1797752121414"></a>共享带宽：</strong>选择一个共享带宽。</li></ul>
</li></ul>
<div class="note" id="note18818202845720"><a name="note18818202845720"></a><a name="note18818202845720"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p13818728135720"><a name="p13818728135720"></a><a name="p13818728135720"></a>该场景的具体实现请参见<a href="https://support.huaweicloud.com/qs-vpc/qs_ipv6.html" target="_blank" rel="noopener noreferrer">搭建IPv6网络</a>。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="10.71%" headers="mcps1.2.6.1.4 "><a name="ul1358217161183"></a><a name="ul1358217161183"></a><ul id="ul1358217161183"><li>IPv4网段</li><li>IPv6网段</li></ul>
</td>
<td class="cellrowborder" valign="top" width="20.830000000000002%" headers="mcps1.2.6.1.5 "><a name="ul2841104394015"></a><a name="ul2841104394015"></a><ul id="ul2841104394015"><li><strong id="b084194317408"><a name="b084194317408"></a><a name="b084194317408"></a>IPv4私网地址+IPv4 EIP：</strong>实例绑定IPv4 EIP，支持IPv4公网通信。</li><li><strong id="b18411431404"><a name="b18411431404"></a><a name="b18411431404"></a>IPv4私网地址：</strong>实例不绑定IPv4 EIP，支持IPv4内网通信。</li></ul>
<a name="ul1522674132211"></a><a name="ul1522674132211"></a><ul id="ul1522674132211"><li><strong id="b9226341162217"><a name="b9226341162217"></a><a name="b9226341162217"></a>IPv6地址+共享带宽：</strong>同时支持IPv6公网通信和IPv6内网通信。</li></ul>
</td>
</tr>
</tbody>
</table>

使用IPv4/IPv6双栈网络请参考[IPv4/IPv6双栈网络](https://support.huaweicloud.com/usermanual-vpc/vpc_0002.html)。

## **IPv6转换**功能应用场景<a name="section1219854425115"></a>

如果您想使部署应用的ECS面向Internet客户端提供IPv6服务，但您的ECS规格不支持IPv6网络，或者您不想通过搭建IPv6网络来实现该需求，那么您可以通过弹性公网IP的IPv6转换功能快速实现该能力。场景示例和资源规划如[表2](#table104846201827)。

**表 2**  IPv6 EIP（开启IPv6转换）网络的应用场景及资源规划

<a name="table104846201827"></a>
<table><thead align="left"><tr id="zh-cn_topic_0133505069_row10563044205914"><th class="cellrowborder" valign="top" width="11.28%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0133505069_p1756315441597"><a name="zh-cn_topic_0133505069_p1756315441597"></a><a name="zh-cn_topic_0133505069_p1756315441597"></a>应用场景</p>
</th>
<th class="cellrowborder" valign="top" width="22.63%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0133505069_p1456364475911"><a name="zh-cn_topic_0133505069_p1456364475911"></a><a name="zh-cn_topic_0133505069_p1456364475911"></a>场景示例</p>
</th>
<th class="cellrowborder" valign="top" width="20.54%" id="mcps1.2.6.1.3"><p id="p239913024617"><a name="p239913024617"></a><a name="p239913024617"></a>条件</p>
</th>
<th class="cellrowborder" valign="top" width="13.389999999999999%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0133505069_p856374416599"><a name="zh-cn_topic_0133505069_p856374416599"></a><a name="zh-cn_topic_0133505069_p856374416599"></a>子网网段类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.16%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0133505069_p71425413219"><a name="zh-cn_topic_0133505069_p71425413219"></a><a name="zh-cn_topic_0133505069_p71425413219"></a>ECS</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0133505069_row1956304410594"><td class="cellrowborder" valign="top" width="11.28%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0133505069_p55632448596"><a name="zh-cn_topic_0133505069_p55632448596"></a><a name="zh-cn_topic_0133505069_p55632448596"></a>IPv6公网通信</p>
</td>
<td class="cellrowborder" valign="top" width="22.63%" headers="mcps1.2.6.1.2 "><p id="p14719514615"><a name="p14719514615"></a><a name="p14719514615"></a>不搭建IPv6网络，使ECS为Internet上的客户端提供IPv6服务。</p>
</td>
<td class="cellrowborder" valign="top" width="20.54%" headers="mcps1.2.6.1.3 "><a name="ul184717564611"></a><a name="ul184717564611"></a><ul id="ul184717564611"><li>实例绑定<span id="text44601156144811"><a name="text44601156144811"></a><a name="text44601156144811"></a></span><span id="text25101758154816"><a name="text25101758154816"></a><a name="text25101758154816"></a>弹性公网IP</span>。</li><li>开启IPv6转换。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="13.389999999999999%" headers="mcps1.2.6.1.4 "><p id="p6782192011211"><a name="p6782192011211"></a><a name="p6782192011211"></a>IPv4网段</p>
</td>
<td class="cellrowborder" valign="top" width="32.16%" headers="mcps1.2.6.1.5 "><a name="ul19807846241"></a><a name="ul19807846241"></a><ul id="ul19807846241"><li><strong id="b163617451972"><a name="b163617451972"></a><a name="b163617451972"></a>IPv4私网地址：</strong>支持IPv4内网通信。</li><li><strong id="b1273120509711"><a name="b1273120509711"></a><a name="b1273120509711"></a>IPv4 EIP地址（开启IPv6转换）：</strong>同时支持IPv4公网通信和IPv6公网通信。</li></ul>
</td>
</tr>
</tbody>
</table>

## IPv6网络应用场景及资源规划<a name="section410011344121"></a>

**图 1**  IPv6网络应用场景及资源规划<a name="fig18359258135814"></a>  
![](figures/IPv6网络应用场景及资源规划.png "IPv6网络应用场景及资源规划")

