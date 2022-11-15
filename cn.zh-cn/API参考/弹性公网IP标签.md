# 弹性公网IP标签<a name="eip_apipermission_0005"></a>

|权限|对应API接口|授权项(Action)|IAM项目(Project)|企业项目(Enterprise Project)|
|--|--|--|--|--|
|创建弹性公网IP资源标签|POST /v2.0/{project_id}/publicips/{publicip_id}/tags|vpc:publicipTags:create|√|×|
|查询弹性公网IP资源标签|GET /v2.0/{project_id}/publicips/{publicip_id}/tags|vpc:publicipTags:get|√|×|
|删除弹性公网IP资源标签|DELETE /v2.0/{project_id}/publicips/{publicip_id}/tags/{key}|vpc:publicipTags:delete|√|×|
|批量创建和删除弹性公网IP资源标签|POST /v2.0/{project_id}/publicips/{publicip_id}/tags/action|vpc:publicipTags:createvpc:publicipTags:delete|√|×|
|查询弹性公网IP资源实例|POST /v2.0/{project_id}/publicips/resource_instances/action|vpc:publicipTags:get|√|×|
|查询弹性公网IP项目标签|GET /v2.0/{project_id}/publicips/tags|vpc:publicipTags:get|√|×|


