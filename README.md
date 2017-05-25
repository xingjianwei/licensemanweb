# licensemanweb

## Restful API 定义
```
/api/v1
```

1. 对象（objects）：代表在系统中的一个永久资源（实体）。通过操作这些资源的属性，客户端可以对该对象做创建、修改、删除和获取操作。
* Machine
* License
* Custom
* User
2. 列表（list）：一个或多个资源类别的集合。列表有一个通用元数据的有限集合。
* CustomLIst
* UserList
3. 简单类别（simple）：该类别包含作用在对象上的特殊行为和非持久实体。
* Status

## API详细说明
1. GET /<资源名的复数格式>：获得某一类型的资源列表，例如GET /users 返回一个user资源列表。
2. POST /<资源名的复数格式>：创建一个资源，该资源来自用户提供的JSON对象。
3. GET /<资源名复数格式>/<名字>：通过给出的名称（Name）获得单个资源，例如GET /users/admin 返回一个名称为“admin”的Pod。
4. DELETE /<资源名复数格式>/<名字>：通过给出的名字删除单个资源。
5. PUT /<资源名复数格式>/<名字>：通过给出的资源名和客户端提供的JSON对象来更新或创建资源。
