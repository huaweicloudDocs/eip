# 弹性公网IP<a name="eip_apipermission_0002"></a>

|权限|对应API接口|授权项(Action)|IAM项目(Project)|企业项目(Enterprise Project)|
|--|--|--|--|--|
|申请弹性公网IP|POST /v1/{project_id}/publicips|vpc:publicIps:create|√|√|
|查询弹性公网IP|GET /v1/{project_id}/publicips/{publicip_id}|vpc:publicIps:get|√|√|
|查询弹性公网IP列表|GET /v1/{project_id}/publicips|vpc:publicIps:list|√|√|
|更新弹性公网IP|PUT /v1/{project_id}/publicips/{publicip_id}|vpc:publicIps:update|√|√|
|删除弹性公网IP|DELETE /v1/{project_id}/publicips/{publicip_id}|vpc:publicIps:delete|√|√|
|申请弹性公网IP（包年/包月）|POST /v2.0/{project_id}/publicips|vpc:publicIps:create|√|√|


