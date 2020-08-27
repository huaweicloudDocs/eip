# 示例一：指定共享带宽ID创建弹性公网IP<a name="eip_apieg_0001"></a>

## 操作场景<a name="section142267511571"></a>

本章节指导用户通过调用API来指定共享带宽ID创建弹性公网IP。

## 前提条件<a name="section10234151977"></a>

您需要规划EIP所在的区域信息，并根据区域确定调用API的Endpoint，详细信息请参见[终端节点（Endpoint）](终端节点（Endpoint）.md)。

当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考3[3.2 认证鉴权](认证鉴权.md)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。

## 操作步骤<a name="section12608714143014"></a>

1.  创建共享带宽。
    1.  发送“POST https://\{Endpoint\}/v2.0/\{project\_id\}/bandwidths”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下：

        ```
        { 
             "bandwidth": { 
                 "name": "bandwidth123", 
                 "size": 10, 
                 "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439" 
             } 
         }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下，id就是bandwidth\_id。

            ```
            { 
               "bandwidth": { 
                 "id": "1bffc5f2-ff19-45a6-96d2-dfdca49cc387", 
                 "name": "bandwidth123", 
                 "size": 10, 
                 "share_type": "WHOLE", 
                 "publicip_info": [], 
                 "tenant_id": "26ae5181a416420998eb2093aaed84d9", 
                 "bandwidth_type": "share", 
                 "charge_mode": "bandwidth", 
                 "enterprise_project_id": "0", 
                 "status": "NORMAL", 
                 "created_at": "2020-04-21T07:58:02Z",  
                 "updated_at": "2020-04-21T07:58:02Z"  
               } 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。

2.  查询带宽详情。
    1.  发送“Get https://\{Endpoint\}//v1/\{project\_id\}/bandwidths/\{bandwidth\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下，id就是bandwidth\_id。

            ```
            { 
                 "bandwidth": { 
                     "id": "a97a827c-3636-4eda-82ce-7aaeeaacd2af", 
                     "name": "bandwidth-fd7fE3", 
                     "size": 6, 
                     "share_type": "PER", 
                     "publicip_info": [ 
                         { 
                             "publicip_id": "ff156c26-bcc9-4541-a75c-42baf8b9748f", 
                             "publicip_address": "114.xx.xx.244", 
                             "ip_version": 4, 
                             "publicip_type": "5_sbgp" 
                         } 
                     ], 
                     "tenant_id": "b3292dde618e40408e30cd87455a0652", 
                     "bandwidth_type": "sbgp", 
                     "charge_mode": "bandwidth", 
                     "enterprise_project_id": "0", 
                     "status": "NORMAL", 
                     "created_at": "2020-04-21T07:58:02Z", 
                     "updated_at": "2020-04-21T07:58:02Z" 
                 } 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。

3.  指定共享带宽ID创建弹性公网IP。
    1.  发送“POST https://\{Endpoint\}/v1/\{project\_id\}/publicips”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下：

        ```
        {     
             "publicip": {         
                 "type": "5_bgp",         
                 "ip_version": 6        
          },    
             "bandwidth": {        
                 "name": "bandwidth123",        
                 "size": 5,         
                 "share_type": "WHOLE", 
                 "id":"ebfa375c-3f93-465e-81a3-bd66e578ee9d" 
             },          
             "enterprise_project_id":"0"   
         }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
                 "publicip": { 
                     "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706", 
                     "status": "PENDING_CREATE", 
                     "type": "5_bgp", 
                     "public_ip_address": "161.xx.xx.7", 
                     "tenant_id": "8b7e35ad379141fc9df3e178bd64f55c", 
                     "ip_version": 4, 
                     "create_time": "2015-07-16 04:10:52", 
                     "bandwidth_size": 0, 
                     "enterprise_project_id":"b261ac1f-2489-4bc7-b31b-c33c3346a439" 
                 } 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。

4.  查询弹性公网IP详情。
    1.  发送“GET /v1/\{project\_id\}/publicips/\{publicip\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。

        ```
        { 
             "publicip": {
                    "id": "3ec9fea0-2d4c-49e2-8aca-ce883eae547d",
                    "type": "5_bgp",
                    "public_ip_address": "10.246.164.87",
                    "status": "DOWN",
                    "tenant_id": "060576782980d5762f9ec014dd2f1148",
                    "create_time": "2020-08-13 12:55:27",
                    "bandwidth_id": "1f570558-46cc-4f78-8a70-db108a617494",
                    "bandwidth_name": "bandwidth-zzzzzz",
                    "bandwidth_share_type": "WHOLE",
                    "bandwidth_size": 6,
                    "profile": {},
                    "enterprise_project_id": "a380829c-db6f-4db3-b5b6-cc377f7a3ff8",
                    "ip_version": 4
                }
         }
        ```



