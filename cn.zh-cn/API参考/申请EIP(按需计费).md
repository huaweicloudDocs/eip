# 申请EIP\(按需计费\)<a name="eip_api_0001"></a>

## 功能介绍<a name="zh-cn_topic_0000001366007860_section174075509368"></a>

申请EIP，支持IPv4和IPv6。 弹性公网IP（Elastic IP）提供独立的公网IP资源，包括公网IP地址与公网出口带宽服务。可以与弹性云服务器、裸金属服务器、虚拟IP、弹性负载均衡、NAT网关等资源灵活地绑定及解绑。拥有多种灵活的计费方式，可以满足各种业务场景的需要。

## 调试<a name="zh-cn_topic_0000001366007860_section340875043619"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EIP&api=CreatePublicip)中调试该接口，支持自动认证鉴权。API Explorer可以自动生成SDK代码示例，并提供SDK代码示例调试功能。

## URI<a name="zh-cn_topic_0000001366007860_section940855011365"></a>

POST /v1/\{project\_id\}/publicips

**表 1**  路径参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|project_id|是|String|项目ID，获取项目ID请参见获取项目ID|


## 请求参数<a name="zh-cn_topic_0000001366007860_section1041119500366"></a>

**表 2**  请求Header参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|X-Auth-Token|是|String|用户Token。通过调用IAM服务获取用户Token接口获取（响应消息头中X-Subject-Token的值）|


**表 3**  请求Body参数

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|bandwidth|是|CreatePublicipBandwidthOption object|带宽对象|
|enterprise_project_id|否|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建弹性公网IP时，给弹性公网IP绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。缺省值：**0**最小长度：**0**最大长度：**36**|
|publicip|是|CreatePublicipOption object|弹性公网IP对象|


**表 4**  CreatePublicipBandwidthOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|charge_mode|否|String|功能说明：按流量计费还是按带宽计费。- -取值范围：bandwidth，traffic，不填或者为空时默认是bandwidth。其中IPv6国外默认是bandwidth，国内默认是traffic。--缺省值：**bandwidth**枚举值：**bandwidth****traffic**|
|id|否|String|功能说明：带宽ID,创建WHOLE类型带宽的EIP时可以指定之前的共享带宽创建取值范围：WHOLE类型的带宽ID最大长度：**36**|
|name|否|String|功能说明：带宽名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）如果share_type是PER，该参数必须带,如果share_type是WHOLE并且id有值，该参数会忽略。最小长度：**1**最大长度：**64**|
|share_type|是|String|功能说明：带宽类型-取值范围：PER，WHOLE（PER为独占带宽，WHOLE是共享带宽）。-- 约束：该字段为WHOLE时，必须指定带宽ID。枚举值：**WHOLE****PER**|
|size|否|Integer|功能说明：带宽大小-取值范围：默认1Mbit/s~2000Mbit/s（具体范围以各区域配置为准，请参见控制台对应页面显示）。- 约束：share_type是PER，该参数必须带，如果share_type是WHOLE并且id有值，该参数会忽略。- 注意：调整带宽时的最小单位会根据带宽范围不同存在差异。   - 小于等于300Mbit/s：默认最小单位为1Mbit/s。   - 300Mbit/s~1000Mbit/s：默认最小单位为50Mbit/s。   - 大于1000Mbit/s：默认最小单位为500Mbit/s。|


**表 5**  CreatePublicipOption

|参数|是否必选|参数类型|描述|
|--|--|--|--|
|ip_address|否|String|功能说明：希望申请到的EIP的地址，不指定时由系统自动分配约束：必须为IPv4地址格式，且必须在可用地址池范围内最大长度：**15**|
|type|是|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。|
|ip_version|否|Integer|-功能说明：弹性公网IP的版本- 取值范围：4、6，分别表示创建ipv4和ipv6- 约束：   - 必须是系统具体支持的类型   - 不填或空字符串时，默认创建ipv4缺省值：**4**枚举值：**4****6**|
|alias|否|String|功能说明：弹性公网IP名称 取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最大长度：**64**|
|port_id|否|String|功能说明：端口id 约束：必须是存在的端口id，如果该端口不存在或端口已绑定EIP则会提示出错。最小长度：**36**最大长度：**36**|


## 响应参数<a name="zh-cn_topic_0000001366007860_section17432205063618"></a>

**状态码： 200**

**表 6**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|publicip|PublicipCreateResp object|弹性公网IP对象|


**表 7**  PublicipCreateResp

|参数|参数类型|描述|
|--|--|--|
|bandwidth_size|Integer|带宽大小，单位为Mbit/s。|
|create_time|String|EIP申请时间（UTC时间）|
|id|String|EIP唯一标识最大长度：**36**|
|public_ip_address|String|IPv4时是申请到的EIP地址，IPv6时是IPv6地址对应的IPv4地址最大长度：**15**|
|status|String|功能说明：EIP的状态- 取值范围：冻结FREEZED，绑定失败BIND_ERROR，绑定中BINDING，释放中PENDING_DELETE， 创建中PENDING_CREATE，创建中NOTIFYING，释放中NOTIFY_DELETE，更新中PENDING_UPDATE， 未绑定DOWN ，绑定ACTIVE，绑定ELB，绑定VPN，失败ERROR。枚举值：**FREEZED****BIND_ERROR****BINDING****PENDING_DELETE****PENDING_CREATE****NOTIFYING****NOTIFY_DELETE****PENDING_UPDATE****DOWN****ACTIVE****ELB****ERROR****VPN**|
|tenant_id|String|项目ID最大长度：**36**|
|type|String|功能说明：EIP的类型取值范围：5_bgp（全动态BGP），5_sbgp（静态BGP）华南-广州：5_bgp、5_sbgp华东-上海一：5_bgp、5_sbgp华东-上海二：5_bgp、5_sbgp华北-北京一：5_bgp、5_sbgp中国-香港：5_bgp亚太-曼谷：5_bgp亚太-新加坡：5_bgp非洲-约翰内斯堡：5_bgp西南-贵阳一：5_bgp、5_sbgp华北-北京四：5_bgp、5_sbgp拉美-圣地亚哥：5_bgp拉美-圣保罗一：5_bgp拉美-墨西哥城一：5_bgp拉美-布宜诺斯艾利一：5_bgp拉美-利马一：5_bgp拉美-圣地亚哥二： 5_bgp约束：必须是系统具体支持的类型。publicip_id为IPv4端口，所以"type"字段未给定时，默认为5_bgp。最大长度：**36**|
|public_ipv6_address|String|IPv4时无此字段，IPv6时为申请到的EIP地址最大长度：**39**|
|ip_version|Integer|IP版本信息，取值范围是4和6枚举值：**4****6**|
|enterprise_project_id|String|企业项目ID。最大长度36字节，带“-”连字符的UUID格式，或者是字符串“0”。- 创建弹性公网IP时，给弹性公网IP绑定企业项目ID。- 不指定该参数时，默认值是 0>关于企业项目ID的获取及企业项目特性的详细信息，请参见《企业管理用户指南》。最大长度：**36**|
|alias|String|功能说明：弹性公网IP名称取值范围：1-64个字符，支持数字、字母、中文、_(下划线)、-（中划线）、.（点）最大长度：**64**|


**状态码： 400**

**表 8**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 401**

**表 9**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 403**

**表 10**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 404**

**表 11**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 405**

**表 12**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 406**

**表 13**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 407**

**表 14**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 408**

**表 15**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 409**

**表 16**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 500**

**表 17**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 501**

**表 18**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 502**

**表 19**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 503**

**表 20**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


**状态码： 504**

**表 21**  响应Body参数

|参数|参数类型|描述|
|--|--|--|
|message|String|服务异常错误信息描述最小长度：**0**最大长度：**256**|
|code|String|服务异常错误信息编码最小长度：**0**最大长度：**36**|


## 请求示例<a name="zh-cn_topic_0000001366007860_section6741175093613"></a>

-   IPv4 EIP独享带宽

    ```
    POST https://{Endpoint}/v1/{project_id}/publicips
    
    {
      "bandwidth" : {
        "size" : 10,
        "share_type" : "PER",
        "name" : "bandwidth123"
      },
      "publicip" : {
        "ip_version" : 4,
        "type" : "5_bgp"
      }
    }
    ```

-   ```
{
  "bandwidth" : {
    "size" : 5,
    "share_type" : "WHOLE",
    "name" : "bandwidth123"
  },
  "publicip" : {
    "ip_version" : 6,
    "type" : "5_bgp"
  }
}
```


## 响应示例<a name="zh-cn_topic_0000001366007860_section7742115014360"></a>

**状态码： 200**

POST操作正常返回

```
{
  "application/json-1" : {
    "publicip" : {
      "tenant_id" : "8b7e35ad379141fc9df3e178bd64f55c",
      "bandwidth_size" : 0,
      "public_ip_address" : "161.xx.xx.7",
      "ip_version" : 4,
      "create_time" : "2015-07-16 04:10:52",
      "id" : "f588ccfa-8750-4d7c-bf5d-2ede24414706",
      "type" : "5_bgp",
      "status" : "PENDING_CREATE"
    }
  },
  "application/json-2" : {
    "publicip" : {
      "id" : "3ff2bf48-b82d-4bf3-88e7-9e55ecdedc34",
      "status" : "PENDING_CREATE",
      "type" : "5_bgp",
      "public_ip_address" : "10.154.79.48",
      "public_ipv6_address" : "cdcd:910a:2222:5498::a9a:4f30",
      "tenant_id" : "26ae5181a416420998eb2093aaed84d9",
      "create_time" : "2019-01-17T11:54:48.000Z",
      "bandwidth_size" : 0,
      "ip_version" : 6
    }
  }
}
```

## 状态码<a name="zh-cn_topic_0000001366007860_section674215033614"></a>

|状态码|描述|
|--|--|
|200|POST操作正常返回|
|400|服务器未能处理请求|
|401|被请求的页面需要用户名和密码|
|403|对被请求页面的访问被禁止|
|404|服务器无法找到被请求的页面|
|405|请求中指定的方法不被允许|
|406|服务器生成的响应无法被客户端所接受|
|407|用户必须首先使用代理服务器进行验证，这样请求才会被处理|
|408|请求超出了服务器的等待时间|
|409|由于冲突，请求无法被完成|
|500|请求未完成。服务异常|
|501|请求未完成。服务器不支持所请求的功能|
|502|请求未完成。服务器从上游服务器收到一个无效的响应|
|503|请求未完成。系统暂时异常|
|504|网关超时|


## 错误码<a name="zh-cn_topic_0000001366007860_section16743135083620"></a>

请参见[错误码](错误码.md)。

