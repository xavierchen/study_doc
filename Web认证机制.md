## Web认证机制  ##

- **Web认证的方式及应用场景**
- **统一登录**
- **Openstack**认证系统

### web认证方式及应用场景 ###

#### Http协议内建的认证方式 ####

1. http basic authentication
2. digest authentication

#### Form-based ####

1. 客户端通过form，讲用户名和密码post给服务器
2. 服务端通过一些逻辑判断有效性
3. 认证成功，返回cookie,失败提示再次认证

1. 高度可定制
2. 服务端保存客户端信息
3. 客户端要有cookie表明身份
4. 客户端cookie的生命周期和安全性相关
#### 证书认证 ####

#### 微软提供的认证方式 ####

### 统一登录 ###

1. 什么是统一登录
2. 统一登录解决什么问题
3. 统一登录的技术实现机制
4. 优缺点分析

#### 统一登录的实现机制 ####

1. 用户访问业务系统A
2. 业务系统A跳转
3. 输入用户名和密码
4. 验证用户信息
5. 查用户信息
6. 认证成功，生成Ticket并跳转回业务系统
7. 访问业务系统B，带Ticket
8. 验证Ticket

#### 统一登录技术要点 ####

1. 如何实现跨域
2. 如何防止信息传递过程被篡改
3. 如何高效存储大量临时性的信任数据