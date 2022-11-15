# 浮动IP（Openstack Neutron API）<a name="eip_apipermission_0006"></a>

|权限|对应API接口|授权项(Action)|IAM项目(Project)|企业项目(Enterprise Project)|
|--|--|--|--|--|
|查询浮动IP列表|GET /v2.0/floatingips|vpc:floatingIps:get|√|×|
|查询浮动IP|GET /v2.0/floatingips/{floatingip_id}|vpc:floatingIps:get|√|×|
|创建浮动IP|POST /v2.0/floatingips|vpc:floatingIps:create|√|×|
|更新浮动IP|PUT /v2.0/floatingips/{floatingip_id}|vpc:floatingIps:update|√|×|
|删除浮动IP|DELETE /v2.0/floatingips/{floatingip_id}|vpc:floatingIps:delete|√|×|


