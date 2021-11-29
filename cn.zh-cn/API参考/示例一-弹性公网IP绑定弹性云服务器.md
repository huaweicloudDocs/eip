# 示例一：弹性公网IP绑定弹性云服务器<a name="eip_apieg_0002"></a>

## 操作场景<a name="section7138121042816"></a>

本章节指导用户通过调用API来为弹性云服务器绑定弹性公网IP。

## 前提条件<a name="section121461310112815"></a>

-   已创建弹性云服务器，具体请参见[创建ECS](https://support.huaweicloud.com/qs-ecs/ecs_02_0009.html)。
-   当您使用Token认证方式完成认证鉴权时，需要获取用户Token并在调用接口时增加“X-Auth-Token”到业务接口请求消息头中。Token认证，具体操作请参考[3.2 认证鉴权](认证鉴权.md)。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >通过IAM服务获取到的Token有效期为24小时，需要使用同一个Token鉴权时，可以先将Token缓存，避免频繁调用。


## 操作步骤<a name="section19170191052819"></a>

1.  通过云服务器的ID查询网卡信息，API详情请参考[查询端口](https://support.huaweicloud.com/api-vpc/vpc_port01_0002.html)。
    1.  发送“GET  https://VPC的Endpoint/v1/\{project\_id\}/ports?device\_id=\{ecs\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
                 "ports": [{ 
                     "id": "02c72193-efec-42fb-853b-c33f2b802467", 
                     "name": "", 
                     "status": "ACTIVE", 
                     "admin_state_up": true, 
                     "fixed_ips": [{ 
                         "subnet_id": "213cb9d-3122-2ac1-1a29-91ffc1231a12", 
                         "ip_address": "192.168.0.75" 
                     }], 
                     "mac_address": "fa:16:3e:47:5f:c1", 
                     "network_id": "4779ab1c-7c1a-44b1-a02e-93dfc361b32d", 
                     "tenant_id": "db82c9e1415a464ea68048baa8acc6b8", 
                     "project_id": "db82c9e1415a464ea68048baa8acc6b8", 
                     "device_id": "ea61f836-b52f-41bf-9d06-685644001d6f", 
                     "device_owner": "compute:br-iaas-odin1a", 
                     "security_groups": [ 
                         "e0598d96-9451-4f8a-8de0-b8b4d451d9e7" 
                     ], 
                     "extra_dhcp_opts": [], 
                     "allowed_address_pairs": [], 
                     "binding:vnic_type": "normal", 
                     "binding:vif_details": { 
                         "primary_interface": true 
                     }, 
                     "binding:profile": {}, 
                     "port_security_enabled": true, 
                     "created_at": "2020-06-20T08:07:29", 
                     "updated_at": "2020-06-20T08:07:29" 
                 }] 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。

2.  创建弹性公网IP。
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

3.  弹性公网IP绑定云服务器网卡。
    1.  发送“PUT /v1/\{project\_id\}/publicips/\{publicip\_id\}”，project\_id为项目ID。
    2.  在Request Header中增加“X-Auth-Token”。
    3.  在Request Body中传入参数如下：

        ```
        {     
             "publicip": {         
                 "port_id": "02c72193-efec-42fb-853b-c33f2b802467"      
             }
         }
        ```

    4.  查看请求响应结果。
        -   请求成功时，响应参数如下：

            ```
            { 
               "publicip": { 
                 "id": "f588ccfa-8750-4d7c-bf5d-2ede24414706", 
                 "status": "ACTIVE", 
                 "type": "5_bgp", 
                 "port_id": "02c72193-efec-42fb-853b-c33f2b802467", 
                 "public_ip_address": "10.xx.xx.162", 
                 "private_ip_address": "192.168.1.131", 
                 "tenant_id": "26ae5181a416420998eb2093aaed84d9", 
                 "create_time": "2019-03-27 01:33:18", 
                 "bandwidth_size": 7, 
                 "ip_version": 4 
               } 
             }
            ```

        -   请求异常时，错误码请参见[7.2 错误码](错误码.md)。



