# 购买公网IP池<a name="eipPools_0002"></a>

## 操作场景<a name="section567518141511"></a>

公网IP池需要购买才能使用，仅支持包年包月计费模式。可以购买多个公网IP池。

公网IP池的IP资源不占用EIP的配额。

>![](public_sys-resources/icon-note.gif) **说明：** 
>该功能目前正在公测中，需要申请公测通过后，才可以正常使用，目前只支持以下区域：华东-上海一、华南-广州、华北-北京四。单击[申请公测](https://account.huaweicloud.com/usercenter/?region=cn-south-1#/applyBeta?serviceCodeP=eip_pool)。

## 操作步骤<a name="section14486185641517"></a>

1.  登录管理控制台。
2.  在管理控制台左上角单击![](figures/icon-region-4.png)，选择区域和项目。
3.  在系统首页，选择“网络 \> 弹性公网IP ”。
4.  在左侧导航栏，选择“弹性公网IP和带宽 \> 公网IP池 ”。
5.  在页面右上角，单击“购买公网IP池”并按照提示配置参数。

    **表 1**  参数说明

    <a name="zh-cn_topic_0118498850_tb8e92f5357304d0297e9c203270c546e"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0118498850_r66aedde49c144d8a84278fc61dadffdd"><th class="cellrowborder" valign="top" width="31.65%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118498850_aafd79e8ecf074d0da2b802ca103815d1"><a name="zh-cn_topic_0118498850_aafd79e8ecf074d0da2b802ca103815d1"></a><a name="zh-cn_topic_0118498850_aafd79e8ecf074d0da2b802ca103815d1"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.29%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118498850_a30252599cf9146418f791259ec182081"><a name="zh-cn_topic_0118498850_a30252599cf9146418f791259ec182081"></a><a name="zh-cn_topic_0118498850_a30252599cf9146418f791259ec182081"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.06%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118498850_a02cb30a37b3a49abb2a82c12344214df"><a name="zh-cn_topic_0118498850_a02cb30a37b3a49abb2a82c12344214df"></a><a name="zh-cn_topic_0118498850_a02cb30a37b3a49abb2a82c12344214df"></a>取值样例</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row10633143201315"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="p13634194361312"><a name="p13634194361312"></a><a name="p13634194361312"></a>计费模式</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p156342433138"><a name="p156342433138"></a><a name="p156342433138"></a>公网IP池的计费模式，支持包年/包月模式。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p18634943171317"><a name="p18634943171317"></a><a name="p18634943171317"></a>包年/包月</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118498850_row69311030161113"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118498850_p1211443310119"><a name="zh-cn_topic_0118498850_p1211443310119"></a><a name="zh-cn_topic_0118498850_p1211443310119"></a>区域</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118498850_p411903317112"><a name="zh-cn_topic_0118498850_p411903317112"></a><a name="zh-cn_topic_0118498850_p411903317112"></a>不同区域的资源之间内网不互通。请选择靠近您客户的区域，可以降低网络时延、提高访问速度。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118498850_p17860245175818"><a name="zh-cn_topic_0118498850_p17860245175818"></a><a name="zh-cn_topic_0118498850_p17860245175818"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118498850_row1755815445016"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="p5511134451716"><a name="p5511134451716"></a><a name="p5511134451716"></a>IP总配额</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p1510144141716"><a name="p1510144141716"></a><a name="p1510144141716"></a>公网IP池中EIP的配额。</p>
    <p id="p11993512132914"><a name="p11993512132914"></a><a name="p11993512132914"></a>公网IP池为EIP分配全动态BGP线路，持续保证网络稳定、高效。您可以在完成公网IP池购买后前往EIP购买页购买对应配额数量的EIP。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p65071544101712"><a name="p65071544101712"></a><a name="p65071544101712"></a>50</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118498850_row1798051216168"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118498850_p44256235163"><a name="zh-cn_topic_0118498850_p44256235163"></a><a name="zh-cn_topic_0118498850_p44256235163"></a>名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118498850_p134282234164"><a name="zh-cn_topic_0118498850_p134282234164"></a><a name="zh-cn_topic_0118498850_p134282234164"></a>公网IP池的名称。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118498850_p2430182381611"><a name="zh-cn_topic_0118498850_p2430182381611"></a><a name="zh-cn_topic_0118498850_p2430182381611"></a>eipPool-test</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118498850_row72697164367"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="p822885133210"><a name="p822885133210"></a><a name="p822885133210"></a>描述</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p1399275111429"><a name="p1399275111429"></a><a name="p1399275111429"></a>公网IP池的描述信息，可以定义公网IP池的用途及使用场景。非必填项。</p>
    <p id="p12593482111429"><a name="p12593482111429"></a><a name="p12593482111429"></a>描述信息内容不能超过255个字符，且不能包含“&lt;”和“&gt;”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p13439131111429"><a name="p13439131111429"></a><a name="p13439131111429"></a>-</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0118498850_row271187493651"><td class="cellrowborder" valign="top" width="31.65%" headers="mcps1.2.4.1.1 "><p id="p1222345153214"><a name="p1222345153214"></a><a name="p1222345153214"></a>购买时长</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.29%" headers="mcps1.2.4.1.2 "><p id="p670514023313"><a name="p670514023313"></a><a name="p670514023313"></a>设置公网IP池的购买时长。</p>
    <p id="p9221135133211"><a name="p9221135133211"></a><a name="p9221135133211"></a>公网IP池暂不支持退订，请合理选择购买时长。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.06%" headers="mcps1.2.4.1.3 "><p id="p1822012593218"><a name="p1822012593218"></a><a name="p1822012593218"></a>3个月</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“立即购买”。

## 后续操作<a name="section6214425372"></a>

后续购买按需计费的弹性公网IP时，可选择已购买的公网IP池来购买对应配额的EIP。详情请参见[申请弹性公网IP](申请弹性公网IP.md)。

选择公网IP池方式购买的EIP将无需支付IP费用，只需支付对应的带宽费用。

