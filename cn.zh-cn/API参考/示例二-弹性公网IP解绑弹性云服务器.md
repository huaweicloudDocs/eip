# 示例二：弹性公网IP解绑弹性云服务器<a name="eip_apieg_0003"></a>

## 操作场景<a name="section679692012810"></a>

本章节指导用户通过调用API来为云服务器解绑弹性公网IP。

## 前提条件<a name="section979752010288"></a>

-   已创建弹性云服务器，具体请参见[创建ECS](https://support.huaweicloud.com/qs-ecs/ecs_02_0009.html)。
-   当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[3.2 认证鉴权](认证鉴权.md)。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。


## 操作步骤<a name="section108026205288"></a>

1.  查询弹性公网IP详情。
    1.  发送“GET /v1/\{project\_id\}/publicips/\{publicip\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
               "publicip": { 
                 "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb", 
                 "status": "ACTIVE", 
                 "type": "5_bgp", 
                 "port_id": "a135e9b8-1630-40d2-a6c5-eb534a61efbe", 
                 "public_ip_address": "10.xx.xx.162", 
                 "private_ip_address": "192.168.1.131", 
            "port_id": "a135e9b8-1630-40d2-a6c5-eb534a61efbe",
                 "tenant_id": "26ae5181a416420998eb2093aaed84d9", 
                 "create_time": "2019-03-27 01:33:18", 
                 "bandwidth_size": 7, 
                 "ip_version": 4 
               } 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。

2.  弹性公网IP解绑云服务器网卡。
    1.  发送“PUT /v1/\{project\_id\}/publicips/\{publicip\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  Request Body中传入参数如下：

        ```
        {     
             "publicip": {         
                 "port_id": ""      
             }
         }
        ```

    1.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
               "publicip": { 
                 "id": "f6318bef-6508-4ea5-a48f-6152b6b1a8fb", 
                 "status": "ACTIVE", 
                 "type": "5_bgp",  
                 "public_ip_address": "10.xx.xx.162", 
                 "private_ip_address": "192.168.1.131", 
                 "tenant_id": "26ae5181a416420998eb2093aaed84d9", 
                 "create_time": "2019-03-27 01:33:18", 
                 "bandwidth_size": 7, 
                 "ip_version": 4 
               } 
             }
            ```


    -   请求异常时，错误码请参见[7.2 错误码](错误码.md)  。


