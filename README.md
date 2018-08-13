<!-- MarkdownTOC autolink="true" autoanchor="true"  uri_encoding="false" -->

- [全局错误码](#全局错误码)
- [API](#api)
    - [公共请求参数](#公共请求参数)
    - [Application](#application)
        - [获取应用列表](#获取应用列表)
        - [更新应用属性](#更新应用属性)
        - [删除应用](#删除应用)
        - [获取用户应用列表](#获取用户应用列表)
        - [应用实例](#应用实例)
            - [获取应用实例](#获取应用实例)
            - [添加应用实例](#添加应用实例)
            - [删除应用实例](#删除应用实例)
        - [应用负责人](#应用负责人)
            - [获取应用负责人信息](#获取应用负责人信息)
            - [添加应用负责人信息](#添加应用负责人信息)
            - [删除应用负责人](#删除应用负责人)
        - [监控信息](#监控信息)
        - [实例日志](#实例日志)
        - [子应用](#子应用)
        - [依赖应用](#依赖应用)
        - [被依赖应用](#被依赖应用)
        - [发布配置](#发布配置)
        - [更新发布配置](#更新发布配置)
            - [链接发布模板](#链接发布模板)
            - [移除发布模板](#移除发布模板)
    - [发布任务](#发布任务)
        - [获取发布任务](#获取发布任务)
        - [新建发布任务](#新建发布任务)
        - [批准任务](#批准任务)
        - [拒绝任务](#拒绝任务)
        - [执行任务](#执行任务)
        - [关闭任务](#关闭任务)
        - [委托任务](#委托任务)
        - [子任务](#子任务)
            - [新建子发布任务](#新建子发布任务)
            - [新建子回滚任务](#新建子回滚任务)
    - [产品线](#产品线)
        - [获取产品线列表](#获取产品线列表)
        - [获取产品线应用](#获取产品线应用)
        - [添加应用](#添加应用)
        - [删除应用](#删除应用-1)
    - [主机](#主机)
        - [获取主机列表](#获取主机列表)
        - [获取主机初始化任务](#获取主机初始化任务)
        - [创建主机初始化任务](#创建主机初始化任务)
        - [获取主机关联应用](#获取主机关联应用)
        - [获取主机启动任务](#获取主机启动任务)
            - [启动主机](#启动主机)
            - [批量启动主机](#批量启动主机)
        - [获取主机停止任务](#获取主机停止任务)
            - [停止主机](#停止主机)
            - [批量停止主机](#批量停止主机)
        - [重启主机](#重启主机)
            - [获取主机重启任务](#获取主机重启任务)
            - [重启主机](#重启主机-1)
        - [批量重启主机](#批量重启主机)
        - [更改主机状态](#更改主机状态)
        - [下架主机](#下架主机)
        - [更新主机zbx配置](#更新主机zbx配置)
    - [资源申请](#资源申请)
        - [申请服务器](#申请服务器)
            - [获取服务器申请列表](#获取服务器申请列表)
            - [新建服务器申请](#新建服务器申请)
            - [获取服务器申请详情](#获取服务器申请详情)
            - [更新服务器申请](#更新服务器申请)
            - [同意服务器申请](#同意服务器申请)
            - [拒绝服务器申请](#拒绝服务器申请)
            - [关闭服务器申请](#关闭服务器申请)
        - [申请域名](#申请域名)
            - [获取域名申请列表](#获取域名申请列表)
            - [新建域名申请](#新建域名申请)
            - [获取域名申请详情](#获取域名申请详情)
            - [更新域名申请](#更新域名申请)
            - [批准域名申请](#批准域名申请)
            - [拒绝域名申请](#拒绝域名申请)
            - [关闭域名申请](#关闭域名申请)
        - [申请域名SSL证书](#申请域名ssl证书)
            - [获取ssl证书申请列表](#获取ssl证书申请列表)
            - [新建ssl证书申请](#新建ssl证书申请)
            - [获取ssl证书申请详情](#获取ssl证书申请详情)
            - [更新ssl证书申请](#更新ssl证书申请)
            - [同意ssl证书申请](#同意ssl证书申请)
            - [拒绝ssl证书申请](#拒绝ssl证书申请)
            - [关闭ssl证书申请](#关闭ssl证书申请)
    - [DNS服务](#dns服务)
        - [获取服务器列表](#获取服务器列表)
        - [添加域名服务器](#添加域名服务器)
        - [获取服务器域名列表](#获取服务器域名列表)
        - [添加域名](#添加域名)
        - [更新域名](#更新域名)
        - [删除域名](#删除域名)
        - [域名记录](#域名记录)
            - [获取域名记录列表](#获取域名记录列表)
            - [添加域名记录](#添加域名记录)
            - [更新域名记录](#更新域名记录)
            - [删除域名记录](#删除域名记录)
            - [禁用域名记录](#禁用域名记录)
    - [发布模板](#发布模板)
        - [获取发布模板列表](#获取发布模板列表)
        - [新建发布模板](#新建发布模板)
        - [获取发布模板详情](#获取发布模板详情)
        - [更新发布模板](#更新发布模板)
            - [删除发布模板](#删除发布模板)
        - [发布脚本](#发布脚本)
            - [获取发布脚本列表](#获取发布脚本列表)
            - [新建发布脚本](#新建发布脚本)
            - [获取发布脚本](#获取发布脚本)
            - [更新发布脚本](#更新发布脚本)
            - [获取脚本关联应用](#获取脚本关联应用)
            - [删除发布脚本](#删除发布脚本)
        - [登录凭据](#登录凭据)
            - [获取密码登录凭据列表](#获取密码登录凭据列表)
            - [创建密码登录凭据](#创建密码登录凭据)
            - [更新密码登录凭据](#更新密码登录凭据)
            - [删除密码登录凭据](#删除密码登录凭据)
    - [用户](#用户)
        - [获取用户列表](#获取用户列表)
        - [获取用户详情](#获取用户详情)
        - [更新用户](#更新用户)
        - [分配用户角色](#分配用户角色)
        - [移除用户角色](#移除用户角色)
        - [禁用用户](#禁用用户)
        - [启用用户](#启用用户)
        - [更改密码](#更改密码)
        - [忘记密码](#忘记密码)
    - [角色](#角色)
        - [获取角色列表](#获取角色列表)
        - [更新角色信息](#更新角色信息)
        - [获取角色用户列表](#获取角色用户列表)
        - [添加用户](#添加用户)
        - [移除用户](#移除用户)
        - [删除角色](#删除角色)
    - [系统授权](#系统授权)
        - [资源权限](#资源权限)
            - [用户应用授权](#用户应用授权)
            - [角色应用授权](#角色应用授权)
            - [获取用户应用权限](#获取用户应用权限)
            - [获取角色应用权限](#获取角色应用权限)
            - [用户主机授权](#用户主机授权)
            - [角色主机授权](#角色主机授权)
            - [获取用户主机权限](#获取用户主机权限)
            - [获取角色主机权限](#获取角色主机权限)
            - [获取应用用户授权](#获取应用用户授权)
            - [更新应用用户授权](#更新应用用户授权)
            - [获取应用角色授权](#获取应用角色授权)
            - [获取主机用户授权](#获取主机用户授权)
            - [更新主机用户授权](#更新主机用户授权)
            - [获取主机角色授权](#获取主机角色授权)
            - [更新主机角色授权](#更新主机角色授权)
        - [功能模块权限](#功能模块权限)
            - [用户功能授权](#用户功能授权)
            - [角色功能授权](#角色功能授权)
    - [第三方导航管理](#第三方导航管理)
        - [获取导航列表](#获取导航列表)
        - [新建导航](#新建导航)
        - [更新导航](#更新导航)
        - [获取导航详情](#获取导航详情)
        - [删除导航](#删除导航)
    - [APIAuthTokens](#apiauthtokens)
        - [获取auth token列表](#获取auth-token列表)
        - [创建auth token](#创建auth-token)
        - [更新auth token](#更新auth-token)
        - [获取auth token详情](#获取auth-token详情)
        - [删除auth token](#删除auth-token)
    - [常用工具](#常用工具)
        - [跳板机日志查询](#跳板机日志查询)
        - [CDN刷新](#cdn刷新)
            - [获取CDN刷新任务列表](#获取cdn刷新任务列表)
            - [新建CDN刷新任务](#新建cdn刷新任务)
    - [操作审计](#操作审计)
        - [获取DNS操作记录](#获取dns操作记录)
        - [获取主机操作记录](#获取主机操作记录)
        - [获取应用操作记录](#获取应用操作记录)
        - [获取授权操作记录](#获取授权操作记录)
            - [获取模块授权操作记录](#获取模块授权操作记录)
            - [获取资源授权操作记录](#获取资源授权操作记录)
        - [APItoken操作](#apitoken操作)
- [数据类型](#数据类型)
    - [Production Object](#production-object)
    - [Application Object](#application-object)
        - [avail app actions](#avail-app-actions)
        - [Available prod actions](#available-prod-actions)
        - [Application deploy template](#application-deploy-template)
    - [Deploy Settings](#deploy-settings)
        - [Application Deploy Settings](#application-deploy-settings)
        - [deploy task lifecycle hooks](#deploy-task-lifecycle-hooks)
            - [lifecycle hook](#lifecycle-hook)
        - [Deploy script](#deploy-script)
        - [FTP repository](#ftp-repository)
        - [GIT repository](#git-repository)
        - [Password credential](#password-credential)
        - [SSH private key credential](#ssh-private-key-credential)
    - [Host object](#host-object)
        - [Host init task](#host-init-task)
            - [Host init task options](#host-init-task-options)
        - [Host start task](#host-start-task)
        - [Host stop task](#host-stop-task)
        - [Host restart task](#host-restart-task)
    - [Resource Request](#resource-request)
        - [Domain request](#domain-request)
            - [requested dns record](#requested-dns-record)
        - [Host request](#host-request)
            - [Requested Host](#requested-host)
            - [Shipped package](#shipped-package)
        - [ssl certificate request](#ssl-certificate-request)
    - [DNS](#dns)
        - [dns server](#dns-server)
        - [dns domain](#dns-domain)
            - [available domain actions](#available-domain-actions)
        - [dns domain record](#dns-domain-record)
    - [Ip Address Object](#ip-address-object)
    - [User object](#user-object)
    - [role object](#role-object)
    - [external navigator object](#external-navigator-object)
    - [auth token object](#auth-token-object)
    - [cdn refresh task](#cdn-refresh-task)
    - [jump server log](#jump-server-log)
    - [dns operation](#dns-operation)
    - [host operation](#host-operation)
    - [app operation](#app-operation)
    - [module authorized operation](#module-authorized-operation)
    - [resource authorized operation](#resource-authorized-operation)

<!-- /MarkdownTOC -->


<a id="top"></a>
<a id="全局错误码"></a>
# 全局错误码

<a id="api"></a>
# API
<a id="公共请求参数"></a>
## 公共请求参数

参数名   | 类型   | 必选 | 默认值 | 说明
---------|--------|------|--------|-----
page     | Number | 否   | 1      | 页码
page_size| Number | 否 | 10     | 页面大小

<a id="application"></a>
## Application
- [获取应用列表](#get_app_list)
- [更新应用](#update_app)
- [应用实例](#instances)
- [应用负责人](#responseperson)
- [错误码](#app_error_code)

<a id="get_app_list"></a>
<a id="获取应用列表"></a>
###  获取应用列表
接口描述: &nbsp; 获取应用列表
接口地址: &nbsp; /applications/
请求方法: &nbsp; GET


**请求参数**

参数名          | 类型   | 必须 | 说明
----------------|--------|------|-------
name            | String | 否   | 应用名
full_path       | String | 否   | 绝对路径
response_persons| Array  | 否   | 负责人id列表
has_parent      | Number | 否   | 是否有父应用, 0 - 无， 1 - 有.
user            | String | 否   | 用户名
role            | String | 否   | 角色名
page_number     | Number | 否   | 页码
page_size       | Number | 否   | 页面大小

>name与full_path的区别, name 表示应用在整个应用拓扑结构链中的某个节点的命名, 而full_path则用来表示整个应用拓扑链路. 举个例子<br> 假设应用A有一个子应用B，B又包含子应用C, 则应用C 的name为C, full_path 为A.B.C

**返回内容**

属性            | 类型   | 说明
----------------|--------|---------
prev            | String | 上一页链接
next            | String | 下一页链接
count           | Number | 总条数
results         | Array  | Array of [Application Object](#application-object)


**请求示例**

    
     GET /applications/
     ContentType: 'application/json'

**响应示例**

     {
        'next': '/application/?page=2',
        'prev': null,
        'count': 100,
        'results': [
            {'id': 1, 
            'name': 'applicationA',
            'has_child': true, 
            'parent_app': 1,
            'available_actions': {
                 'view': true,
                 'deploy': true,
                 'check_deploy_task': true,
                 'edit': true,
                 'delete': true,
                 'reboot': true,
                 'view_log': true,
                 'view_monitor': true
               }      
            },
            {'id': 2, 
             'name': 'applicationB',
             'has_child': true, 
             'parent_app': 2,
             'available_actions': {
                 'view': true,
                 'deploy': true,
                 'check_deploy_task': true,
                 'edit': true,
                 'delete': true,
                 'reboot': true,
                 'view_log': true,
                 'view_monitor': true
               } 
            },  
        ]
    }
<a id="更新应用属性"></a>
###  更新应用属性
接口描述: &nbsp; <span id="update_app">更新应用属性</span> 
接口地址: &nbsp; /applications/{id}/
请求方法: &nbsp; PATCH
**请求参数**

属性            | 类型                        | 必选 | 说明
----------------|-----------------------------|------|---------
name            | String                      |  否  | 应用名称
description     | String                      |  否  | 描述
application_type| String                      |  否  | 应用类型
run_users       | String                      |  否  | 运行用户
directory       | String                      |  否  | 部署路径
startup_cmd     | String                      |  否  | 启动命令
stop_cmd        | String                      |  否  | 停止命令
stdout_path     | String                      |  否  | 标准输出路径
stderr_path     | String                      |  否  | 错误输出路径
pid_path        | String                      |  否  | pid文件路径
parent_app      | Number or Null              |  否  | 父应用ID
child_apps      | Array of child app id       |  否  | 子应用id列表 
required_apps   | Array of required app id    |  否  | 依赖应用id列表
response_person | Array of response person id |  否  | 负责人id列表

**返回内容**

属性            | 类型   | 说明
----------------|--------|---------
message         | String | 返回信息                          


**请求示例**

        PATCH /application/{id}/
        ContentType: 'application/json'
        {
            'name': 'newAppName',
            'description': 'some description',
            'application_type': 1,
            'run_user': 'root',
            'directory': '/data/newAppName',
            'startup_cmd': 'service newAppName start',
            'stop_cmd': 'service newAppName stop',
            'stdout_path': '/data/log/newAppName/stdout',
            'stderr_path': '/data/log/newAppName/stderr',
            'pid_path': '/var/run/newAppName.pid',
            'parent_app': 1,
            'child_apps': [4, 5, 6, 7],
            'required_apps': [11, 12],
            'response_person': [1, 2, 3]
        }

**响应示例**

        {
            'message': "success",
        }
<a id="删除应用"></a>
### 删除应用

接口描述: &nbsp; <span id="update_app">更新应用属性</span> 
接口地址: &nbsp; /applications/{id}/
请求方法: &nbsp; DELETE

**请求参数**
无

**返回内容**

属性            | 类型                        | 说明
----------------|-----------------------------|---------
message         | String                      | 返回信息

**请求示例**

        DELETE /applications/{id}/

**响应示例**

        {
            'message': 'success'
        }

<a id="获取用户应用列表"></a>
### 获取用户应用列表
接口描述: &nbsp; <span id="update_app">更新应用属性</span> 
接口地址: &nbsp; /applications/get-by-users/
请求方法: &nbsp; POST

**请求参数**
>Array of [user object](#user object)

**返回内容**


属性         | 类型   | 说明
-------------|--------|------
user_id      | Number |用户id
applications | Array  | Array of [application object](#application-object)

**请求示例**

        POST /applications/get-by-users/
        ContentType: 'application/json'
        [{'id': 1}, ['id': 2]]

**响应示例**

        [
           {'user_id': 1,
           'applications': [
             {
               'name': 'newAppName',
               'description': 'some description',
               'application_type': 1,
               'run_user': 'root',
               'directory': '/data/newAppName',
               'startup_cmd': 'service newAppName start',
               'stop_cmd': 'service newAppName stop',
               'stdout_path': '/data/log/newAppName/stdout',
               'stderr_path': '/data/log/newAppName/stderr',
               'pid_path': '/var/run/newAppName.pid',
               'parent_app': 1,
               'child_apps': [4, 5, 6, 7],
               'required_apps': [11, 12],
               'response_person': [1, 2, 3]，
               'available_actions': {
                 'view_app': true,             
                 'edit_app': false,              
                 'delete_app': true,           
                 'deploy_app': false,          
                 'review_app_deploy_task': true,
                 'restart_app': true,           
                 'view_app_log': true,           
                 'view_app_monitor': true      
               }
             },
             ...
             ],
           }
        ]


<a id="instances"></a>
<a id="应用实例"></a>
### 应用实例
- [获取应用实例列表](#get_app_instances)
- [添加应用实例](#add_app_instances)
- [删除应用实例](#remove_app_instances)

<a id='get_app_instances'></a>
<a id="获取应用实例"></a>
####获取应用实例
接口描述: &nbsp; 获取应用实例列表
接口地址: &nbsp; /application/{id}/instances/
请求方法: &nbsp; GET

**请求参数**

参数名          | 类型           |必选| 说明
----------------|----------------|----|---------
    page        | Number         | 否 | 页码
    page_number | Number         | 否 | 页面大小                

**返回内容**

属性            | 类型   | 说明
----------------|--------|---------
prev            | String | 上一页链接
next            | String | 下一页链接
count           | Number | 总条数
results         | Array  | Array of [App Instance](#app_instance_obj)


**<span id="app_instance_obj">App Instance</span>**

属性            | 类型                        | 说明
----------------|-----------------------------|---------
id              | Number                      | 实例Id
hostname        | String                      | 实例所在主机
status          | String                      | 实例状态, 值为['restarting','running', 'stopped','updating', 'reverting'] 之一
version         | String                      | 实例版本号

**请求示例**

        GET /application/{id}/instances/
        ContentType: 'application/json'
    
**响应示例**

        {
            'next': '/application/{id}/instances/?page=2',
            'prev': null,
            'count': 100,
            'results': [
                {
                    'id': 1,
                    'hostname': 'hostA',
                    'status': 'running',
                    'version': '2018-04-35'
                },
                {
                    'id': 2,
                    'hostname': 'hostB',
                    'status': 'running',
                    'version': '2018-04-35'
                }
            ]
        }

<a id='add_app_instances'></span>
<a id="添加应用实例"></a>
####添加应用实例
接口描述: &nbsp; 添加应用实例
接口地址: &nbsp; /application/{id}/instances/
请求方法: &nbsp; POST

**请求参数**

>Array of bellow

参数名         | 类型   |必选| 说明
---------------|--------|----|---------
hostid         | Number | 是 | 实例所属主机id
hostname       | String | 否 | 实例所属主机名

**返回内容**
Array of  [App Instance obj](#app_instance_obj)     

**请求示例**

        POST /application/{id}/instances/
        ContentType: 'application/json'
        [
            { 'hostid': 1},
            { 'hostid': 2}
        ]

**返回示例**

        [
           
            { 'id': 3, 'hostid': 1, 'hostname': 'hostA', status: 'stopped'},
            { 'id': 4, 'hostid': 2, 'hostname': 'hostB', status: 'stopped'}
            
        ]


<a id='remove_app_instances'></a>
<a id="删除应用实例"></a>
#### 删除应用实例
接口描述: &nbsp; 删除应用实例
接口地址: &nbsp; /application/{id}/instances/
请求方法: &nbsp; DELETE

**请求参数**

>Array of bellow

参数名          | 类型           |必选| 说明
--------------- |----------------|--- |---------
 id             | Number         | 是 | 实例id

**返回内容**

属性            | 类型                        | 说明
--------------- |-----------------------------|---------
message         | String                      | 返回信息

**请求示例**

        DELETE /application/{:id}/instances/
        ContentType: 'application/json'
        [
            { 'id': 1},
            { 'id': 2}
        ]

**返回示例**

        {
            'message': 'sucess',
        }

 
<a id="responseperson"></a>
<a id="应用负责人"></a>
### 应用负责人
- [获取应用负责人信息](#get_app_response_person)
- [添加应用负责人](#add_app_response_person)
- [删除应用负责人](#remove_app_response_person)

<a id='get_app_response_person'></a>
<a id="获取应用负责人信息"></a>
#### 获取应用负责人信息
接口描述: &nbsp; 获取应用负责人信息
接口地址: &nbsp; /application/{id}/response-person/
请求方法: &nbsp; GET

**请求参数**

>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性            | 类型   | 说明
--------------- |--------|---------
prev            | String | 上一页链接
next            | String | 下一页链接
count           | Number | 总条数
results         | Array  | Array of [App response person](#app_response_person)

**<div id='app_response_person'>App response person</div>**

属性            | 类型                        | 说明
--------------- |-----------------------------|---------
id              | Number                      | 负责人id
name            | String                      | 姓名
email           | String                      | 邮箱
type            | String                      | 负责人类型, 可选值为['dev', 'ops', 'qa', 'pm']
mobile          | Number                      | 手机号码


**请求示例**

        GET /application/{id}/response-person/
        ContentType: 'application/json'

**响应示例**

        {
            'next': '/application/{id}/response-person/?page=2',
            'prev': null,
            'count': 100,
            'results': [
                {
                    'id': 1,
                    'name': '张三'
                    'mobile': 18834584567,
                    'email': 'san.zhang@gmail.com'
                    'type': 'pm'
                },
                 {
                    'id': 2,
                    'name': '李四'
                    'mobile': 18834584567,
                    'email': 'si.li@gmail.com'
                    'type': 'dev'
                },
            ]
        }

<a id='add_app_response_person'></a>
<a id="添加应用负责人信息"></a>
#### 添加应用负责人信息
接口描述: &nbsp; 添加应用负责人信息
接口地址: &nbsp; /application/{id}/response-person/
请求方法: &nbsp; POST

**请求参数**

>Array of bellow

参数名      | 类型           |必选| 说明
------------|----------------|--- |---------
id          | Number         | 是 | 负责人ID
type        | String         | 是 | 负责人类型, 可选值为['dev', 'ops', 'qa', 'pm']


**返回内容**

Array of  [App response person](#app_response_person)

**请求示例**

        POST /application/{id}/response-person/
        ContentType: 'application/json'
        [
            {'id': 1, 'type': 'pm'},
            {'id': 2, 'type': 'dev'},
        ]

**响应示例**

        [                             
            {
                'id': 1,
                'name': '张三'
                'mobile': 18834584567,
                'type': 'pm',
                'email': 'san.zhang@gmail.com'
            },
            {
                'id': 2,
                'name': '李四'
                'mobile': 18834584567,
                'type': 'dev',
                'email': 'si.li@gmail.com'
            },
        ]
    


<a id='remove_app_response_person'></a>
<a id="删除应用负责人"></a>
#### 删除应用负责人
接口描述: &nbsp; 删除应用负责人
接口地址: &nbsp; /application/{id}/response-person/
请求方法: &nbsp; DELETE

**请求参数**

>Array of bellow

参数名          | 类型           |必选| 说明
--------------- |----------------|--- |---------
id              | Number         | 是 | 负责人id
 

**返回内容**

属性            | 类型                        | 说明
--------------- |-----------------------------|---------
message         | String                      | 返回信息


**请求示例**

        DELETE /application/{id}/response-person/
        ContentType: 'application/json'
        [
            { 'id': 1 },
            { 'id': 2 },
        ]

**响应示例**

        {
            'message': 'success',
        }

<a id="监控信息"></a>
### 监控信息
<a id="实例日志"></a>
### 实例日志
接口描述: &nbsp; 获取应用日志
接口地址: &nbsp; /application/{:id}/instance/{:id}/log/
请求方法: &nbsp; GET

**请求参数**
>注意日志读取模式

参数名          | 类型      |必选| 默认值 |说明
--------------- |-----------|--- |--------|-----
log_type        | String    | 是 |'stdout'|日志类型, 可选值为['stdout', 'error'].
mode            | String    | 是 |'bytes' |可选值为['lines',' bytes'].
from_position   | Number    | 否 |   0    |从文件开头 from_position 字节位置读取block_size 大小文件内容, <br>不能与from_last_position参数一起使用,<br>只在'bytes'模式下生效.       
from_last_position| Number  | 否 |   0    |从文件结尾 from_last_position字节位置读取 block_size 大小的文件内容, <br>不能与from_position 参数一起使用,<br>只在 bytes 模式下生效
block_size      | Nunber    | 否 | 8192   |每次读取大小, 只在'bytes'模式下生效.
lines           | Number    | 否 | 1000   |从文件开始获取lines行的日志内容, 只在'lines'模式下生效.
from_lines      | Number    | 否 |   无   |从文件开始from_lines行之后的位置读取 lines行的文件内容,只在'lines'模式下生效.
latest_lines    | Number    | 否 | 1000   |获取最近latest_lines行的文件内容,只在'lines'模式下生效.
latest_lines_offset | Number| 否 |    无  |从文件尾部之前latest_lines_offset行的位置向前获取<br>latest_lines行的文件内容, 只在'lines'模式下生效.

**返回内容**

属性            | 类型   | 说明
--------------- |--------|---------
content         | String | 日志内容
length          | Number | 日志内容大小
total_length    | Number | 日志文件大小
position        | Number | 当前位置
lines           | Number | 当前行数， 只在'lines'模式下返回

**请求示例**

        GET /application/{:id}/instance/{:id}/log/?log_type=error

**返回示例**
       
         {
            'content': 'some erro log text'.
            'length': 48,
            'total_length': 1000,
            'position': 48,
         }

<a id="子应用"></a>
### 子应用
- [获取子应用信息](#get_app_child_apps)
- [添加子应用](#add_app_child_apps)
- [删除子应用](#delete_app_child_apps)

<a id='get_app_child_apps'></a>
接口描述: &nbsp; 获取子应用信息
接口地址: &nbsp; /application/{:id}/child-apps/
请求方法: &nbsp; GET

**请求参数**

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|-------
name            | String    | 否 |  无    | 应用名
full_name       | String    | 否 |  无    | 应用绝对路径
user            | String    | 否 |  无    | 用户名
role            | String    | 否 |  无    | 角色名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of  [Application obj](#application-object) 

**请求示例**

         GET /application/{:id}/child-apps/
         ContentType: 'application/json'

**响应示例**

        {
            'next': "/application/{:id}/child-apps/?page=2"
            'prev': null,
            'count': 100,
            'results': [
                {'id': 1, 
                'name': 'applicationA',
                'has_child': true, 
                'parent_app': 1,
                'available_actions': {
                     'view': true,
                     'deploy': true,
                     'check_deploy_task': true,
                     'edit': true,
                     'delete': true,
                     'reboot': true,
                     'view_log': true,
                     'view_monitor': true
                   }      
                },
                {'id': 2, 
                 'name': 'applicationB',
                 'has_child': true, 
                 'parent_app': 2,
                 'available_actions': {
                     'view': true,
                     'deploy': true,
                     'check_deploy_task': true,
                     'edit': true,
                     'delete': true,
                     'reboot': true,
                     'view_log': true,
                     'view_monitor': true
                   } 
                },  
            ]
        }

<a id='add_app_child_apps'></a>
接口描述: &nbsp; 添加子应用
接口地址: &nbsp; /application/{:id}/child-apps/
请求方法: &nbsp; POST
>添加子应用并不会创建新的应用对象，只是新增应用父子依赖映射关系.

**请求参数**
>Array of bellow object

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|-----
id              | String    | 是 |  无    | 子应用id

**返回内容**

Array of  [Application obj] (#application-object)                     

**请求示例**

        POST /application/{:id}/child-apps/
        ContentType: 'application/json'
        [ {'id': 1, 'id': 2}]

**响应示例**

        [            
            {'id': 1, 
            'name': 'applicationA',
            'has_child': true, 
            'parent_app': 0,    
            },
            {'id': 2, 
             'name': 'applicationB',
             'has_child': true, 
             'parent_app': 0, 
            },
            ...
        ]
   

<a id='delete_app_child_apps'></a>
接口描述: &nbsp; 删除子应用
接口地址: &nbsp; /application/{:id}/child-apps/
请求方法: &nbsp; DELETE
>删除子应用并不会删除子应用对象，只是解除子应用与当前应用的父子映射关系
**请求参数**
>以下对象列表

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|-----
id              | String    | 是 |  无    | 子应用id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        DELETE /application/{:id}/child-apps/
        ContentType: 'application/json'
        [ {'id': 1, 'id': 2}]

**响应示例**

        {
            'message': 'success',
        }

<a id="依赖应用"></a>
### 依赖应用
- [获取依赖应用](#get_app_required_apps)
- [添加依赖应用](#add_app_required_apps)
- [删除依赖应用](#delete_app_required_apps)

<a id='get_app_required_apps'></a>
接口描述: &nbsp; 获取依赖应用
接口地址: &nbsp; /application/{:id}/required-apps/
请求方法: &nbsp; GET

**请求参数**

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|--------
name            | String    | 否 |  无    | 应用名
full_name       | String    | 否 |  无    | 应用绝对路径
user            | String    | 否 |  无    | 用户名
role            | String    | 否 |  无    | 角色名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 产品总条数
results     | Array  | Array of [Application object](#application-object)

**请求示例**

        GET /application/{:id}/required-apps/
        ContentType: 'application/json'

**响应示例**

        {
            'next': '/application/{:id}/required-apps/?page=2',
            'prev': null,
            'count': 2,
            'results': [
                {'id': 1, 
                'name': 'applicationA',
                'has_child': true, 
                'parent_app': 1,
                'available_actions': {
                     'view': true,
                     'deploy': true,
                     'check_deploy_task': true,
                     'edit': true,
                     'delete': true,
                     'reboot': true,
                     'view_log': true,
                     'view_monitor': true
                   }      
                },
                {'id': 2, 
                 'name': 'applicationB',
                 'has_child': true, 
                 'parent_app': 2,
                 'available_actions': {
                     'view': true,
                     'deploy': true,
                     'check_deploy_task': true,
                     'edit': true,
                     'delete': true,
                     'reboot': true,
                     'view_log': true,
                     'view_monitor': true
                   } 
                },  
            ]
        }


<a id='add_app_required_apps'></a>
接口描述: &nbsp; 添加依赖应用
接口地址: &nbsp; /application/{:id}/required-apps/
请求方法: &nbsp; POST
>添加依赖应用并不会创建新的应用对象，只是新增应用兄弟依赖映射关系.

**请求参数**
>Array of bellow object

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|-----
id              | String    | 是 |  无    | 依赖应用id

**返回内容**
Array of [Application object](#application-object)


**请求示例**

        POST /application/{:id}/required-apps/
        ContentType: 'application/json'
        [ {'id': 1, 'id': 2}]

**响应示例**

        [
            {'id': 1, 
            'name': 'applicationA',
            'has_child': true, 
            'parent_app': 0,    
            },
            {'id': 2, 
             'name': 'applicationB',
             'has_child': true, 
             'parent_app': 0, 
            }, 
            ... 
        ]
   


<a id='delete_app_child_apps'></a>
接口描述: &nbsp; 删除依赖应用
接口地址: &nbsp; /application/{:id}/required-apps/
请求方法: &nbsp; DELETE
>删除依赖应用并非删除依赖应用对象，只是解除兄弟依赖映射关系.

**请求参数**
> Array of bellow object

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|-----
id              | String    | 是 |  无    | 依赖应用id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        DELETE /application/{:id}/required-apps/
        ContentType: 'application/json'
        [ {'id': 1, 'id': 2}

**响应示例**

        {
           'message': 'success',
        }
<a id="requiredbyapps"></a>
<a id="被依赖应用"></a>
### 被依赖应用
> 应用依赖关系需要通过 [添加依赖应用](#add_app_required_apps) 接口进行操作

<a id='get_app_required_apps'></a>
接口描述: &nbsp; 获取被依赖应用
接口地址: &nbsp; /application/{:id}/required-by-apps/
请求方法: &nbsp; GET

**请求参数**

参数名          | 类型      |必选| 默认值 |说明
----------------|-----------|----|--------|--------
name            | String    | 否 |  无    | 应用名
full_name       | String    | 否 |  无    | 应用绝对路径
user            | String    | 否 |  无    | 用户名
role            | String    | 否 |  无    | 角色名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 产品总条数
results     | Array  | Array of [Application object](#application-object)

**请求示例**

        GET /application/{:id}/required-by-apps/
        ContentType: 'application/json'

**响应示例**

      {
        'next': '/application/{:id}/required-by-apps/?page=2',
        'prev': null,
        'count': 1000,
        'results': [
            {'id': 1, 
             'name': 'applicationA',
             'has_child': true, 
             'parent_app': 1,
             'available_actions': {
                 'view': true,
                 'deploy': true,
                 'check_deploy_task': true,
                 'edit': true,
                 'delete': true,
                 'reboot': true,
                 'view_log': true,
                 'view_monitor': true
               }      
            },
            {'id': 2, 
             'name': 'applicationB',
             'has_child': true, 
             'parent_app': 2,
             'available_actions': {
                 'view': true,
                 'deploy': true,
                 'check_deploy_task': true,
                 'edit': true,
                 'delete': true,
                 'reboot': true,
                 'view_log': true,
                 'view_monitor': true
               } 
            },  
       ]
    }

<a id="发布配置"></a>
### 发布配置
<a id='get_app_deploy-settings'></a>
接口描述: &nbsp; 获取应用发布配置
接口地址: &nbsp; /application/{:id}/deploy-settings/
请求方法: &nbsp; GET

**请求参数**
无

**返回内容**

[Application Deploy Settings](#application-deploy-settings) 


**请求示例**

     GET /application/{:id}/deploy-settings/
     ContentType: 'application/json

**响应示例**

    {
        'enabled': true,
        'application': 1,
        'template': {
            'id': 1,
            'name': 'test-deploy-template'
        },
        'repository': {
            'type': 'GIT'
            'url': 'http://git.example.com/test',
            'branch': 'release',
            'credential': {
                'type': 'PASSWORD',
                'username': 'username',
                'password': 'pasword'
            }
        },
        'deploy_path': '/path/to/deploy/path',
        'script_running_user': 'work',
        'timeout': 120,
        'keep_backups': 5,
        'lifecycle_hooks': {
             'running_user': 'work',
             'global_pre_exec': null,
             'pre_exec': {
                'script':  {
                    'id': 1,
                    'name': 'pre exec script',
                 }
              },
              'post_exec': {
                 'script':  {
                    'id': 2,
                    'name': 'post exec script',
                  }
              },
              'glboal_post_exec': null,
        }
     }

<a id="更新发布配置"></a>
### 更新发布配置
接口描述: &nbsp; 更新发布配置
接口地址: &nbsp; /application/{:id}/deploy-settings/
请求方法: &nbsp; PATCH

**请求参数**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
applications         | Array  | 否   |  无    |关联应用Id列表
repository           | Object | 否   |  无    |应用源码仓库,  可能的类型为<ul><li>[ftp repo arguments](#ftp-repository-arguments) </li><li>[git repo arguments](#git-repository-arguments)</li></ul>
deploy_path          | String | 否   |  无    |发布路径
timeout              | Number | 否   |  120   |发布任务执行超时时间
keep_backups         | Number | 否   |  5     |保留最近备份数
lifecycle_hooks      | Array  | 否   |  无    |[deploy task lifecycle hooks](#deploy-task-lifecycle-hooks)

<a id='ftp-repository-arguments'></a>
**FTP Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 否   |  无    | ftp地址
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 否  | 无  | 登录凭据

<a id='git-repository-arguments'></a>
**GIT Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 否   |  无    | git仓库地址
branch               | String | 否   |  无    | git仓库分支
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 否  | 无  | 登录凭据

**返回内容**
[Application deploy template](#application-deploy-template)

**请求示例**
    
        PATCH /application/{:id}/deploy-settings/
        ContentType: 'application/json'
        {
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': 1,
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                      }
                  },
                  'glboal_post_exec': null,
            }
        }

**响应示例**

        {
            'id': 1
            'enabled': true,
            'creator': 'test_user',
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': {
                    'type': 'PASSWORD'
                    'username': 'username',
                    'password': 'pasword'
                 }
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                        'name': 'pre exec script',
                        'language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja',
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                        'name': 'post exec script',
                        ‘language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja'
                      }
                  },
                  'glboal_post_exec': null,
             }
        }

<a id="链接发布模板"></a>
#### 链接发布模板
<a id='link_app_deploy_template'></a>
接口描述: &nbsp; 链接发布模板
接口地址: &nbsp; /application/{:id}/deploy-settings/template/
请求方法: &nbsp; POST

**请求参数**

参数名 | 类型   | 必选 | 说明
-------|--------|------|------
id     | Number | 是   | 发布模板id


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/{:id}/deploy-settings/template/
        ContentType: 'application/json'
        {'id': 1}

**响应示例**
    
        {
           'message': 'success'
        }

<a id="移除发布模板"></a>
#### 移除发布模板
<a id='unlink_app_deploy_template'></a>
接口描述: &nbsp; 移除发布模板
接口地址: &nbsp; /application/{:id}/deploy-settings/template/
请求方法: &nbsp; DELETE

**请求参数**

参数名 | 类型   | 必选 | 默认值 |说明
-------|--------|------|------- |----
id     | Number | 是   | 无     | 发布模板id
clean  | Bool   | 否   | false  | 是否清理发布配置

>移除模板并清理发布配置时, 将clean设置为true即可


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/{id}/deploy-settings/template/
        ContentType: 'application/json'
        {'id': 1}

**响应示例**
    
        {
           'message': 'success'
        }

<a id="发布任务"></a>
## 发布任务
<a id="获取发布任务"></a>
### 获取发布任务
接口描述: &nbsp; 获取发布任务
接口地址: &nbsp; /application/deploy-tasks/
请求方法: &nbsp; GET

**请求参数**

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------

<a id="新建发布任务"></a>
### 新建发布任务
接口描述: &nbsp; 新建发布任务
接口地址: &nbsp; /application/deploy-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
application_id    | Number | 是   |    无 | 应用id
version           | Number | 是   |    无 | 发布版本号
description       | String | 是   |    无 | 上线描述
level             | String | 是   |    无 | 任务级别 可选值 [ S, A, B, C, I ]
package_source    | String | 是   |　　无 | 发布的文件路径
planned_exec_time | Number | 是   |    无 | 计划发布时间戳
upgrade_checklist | String | 否   |    无 | 上线checklist
upgrade_steps     | String | 否   |    无 | 更新执行步骤
rollback_steps    | String | 否   |    无 | 回滚步骤

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/
        ContentType: 'application/json'
        {
           'application_id': 1,
           'version': '20180408-120000'
           'planned_exec_time': 1523177609,
           'deploy_source': '/data/app/20180408/root.war',
           'level':　'A',
           'upgrade_checklist': '检查日志',
           'upgrade_steps': '直接发布'，
           'rollback_steps': '直接回滚'
        }


**响应示例**
    
        {
           'message': 'success'
        }
<a id="批准任务"></a>
### 批准任务

接口描述: &nbsp; 批准任务
接口地址: &nbsp; /application/deploy-tasks/{id}/actions/approve/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/{id}/actions/approve/
        ContentType: 'application/json'

**响应示例**
    
        {
           'message': 'success'
        }

<a id="拒绝任务"></a>
### 拒绝任务

接口描述: &nbsp; 拒绝任务
接口地址: &nbsp; /application/deploy-tasks/{id}/actions/reject/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/{id}/actions/reject/
        ContentType: 'application/json'

**响应示例**
    
        {
           'message': 'success'
        }

<a id="执行任务"></a>
### 执行任务

接口描述: &nbsp; 开始任务
接口地址: &nbsp; /application/deploy-tasks/{id}/actions/start/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/{id}/actions/start/
        ContentType: 'application/json'

**响应示例**
    
        {
           'message': 'success'
        }
<a id="关闭任务"></a>
### 关闭任务

接口描述: &nbsp; 关闭任务
接口地址: &nbsp; /application/deploy-tasks/{id}/actions/close/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/{id}/actions/close/
        ContentType: 'application/json'

**响应示例**
    
        {
           'message': 'success'
        }

<a id="委托任务"></a>
### 委托任务

接口描述: &nbsp; 委托任务
接口地址: &nbsp; /application/deploy-tasks/{id}/actions/delegate/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
user_id           | Number | 是   |  无   | 被委托人用户ID

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 消息

**请求示例**

        POST /application/deploy-tasks/{id}/actions/delegate/
        ContentType: 'application/json'
        {'user_id': 1}

**响应示例**
    
        {
           'message': 'success'
        }
<a id="子任务"></a>
### 子任务
<a id="新建子发布任务"></a>
#### 新建子发布任务
接口描述: &nbsp; 新建子发布任务
接口地址: &nbsp; /application/deploy-tasks/{id}/sub-upgrade-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
instances         | Object | 是   |  无   |  Array of [instance](#app-deploy-task-sub-task-instance)要更新的应用实例id列表
update_source     | String | 是   |  无   | 更新源文件路径
version           | String | 是   |  无   | 更新版本号
timeout           | Number | 否   |  120  | 子任务超时时间

<span id='app-deploy-task-sub-task-instance'></span>
instance object

属性        | 类型   | 说明
------------|--------|---------
id          | Number | 要更新的应用实例id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
task_id     | String | 子任务ID
task_output | String | 子任务标准输出的 websocket 地址

**请求示例**

        POST /application/deploy-tasks/{id}/sub-upgrade-tasks/
        ContentType: 'application/json'
        {
           'instances': [
               {'id': 1}, {'id': 2}, {'id': 3}
           ],
           'update_source': '/application/{id}/root.war',
           'version': '20180414-121540'
        }

**响应示例**
    
        {
           'task_id': '342443434'
           'task_output': 'ws://ws.example.com/channel/xxx'
        }
<a id="新建子回滚任务"></a>
#### 新建子回滚任务
接口描述: &nbsp; 新建子回滚任务
接口地址: &nbsp; /application/deploy-tasks/{id}/sub-revert-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
instances         | Object | 是   |  无   |  Array of [instance](#app-deploy-task-sub-task-instance)要回滚的应用实例id列表
version           | String | 是   |  无   | 回滚的版本号
timeout           | Number | 否   |  120  | 子任务超时时间

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
task_id     | String | 子任务ID
task_output | String | 子任务标准输出的 websocket 地址

**请求示例**

        POST /application/deploy-tasks/{id}/sub-revert-tasks/
        ContentType: 'application/json'
        {
           'instances': [
               {'id': 1}, {'id': 2}, {'id': 3}
           ],
           'version': '20180414-121540'
        }

**响应示例**
    
        {
           'task_id': '342443434'
           'task_output': 'ws://ws.example.com/channel/xxx'
        }
<a id="产品线"></a>
## 产品线
<a id="获取产品线列表"></a>
### 获取产品线列表
接口描述: &nbsp; 获取产品线列表
接口地址: &nbsp; /productions/
请求方法: &nbsp; GET

**请求参数**
>其他参数请参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
name              |String  | 否   |  无   |  产品线名称

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 产品总条数
results     | Array  | Array of [Production Object](#production-object)

**请求示例**

        GET /productions/

**响应示例**

        {
           'count': 100,
           'prev': null,
           'next': '/productions/?page=2',
           'results': [
                {'id': 1, 'name': 'production A', 'description': 'desc of production A'},
                ...
           ]
        }
<a id="获取产品线应用"></a>
### 获取产品线应用
接口描述: &nbsp; 获取产品线应用
接口地址: &nbsp; /productions/{id}/applications/
请求方法: &nbsp; GET

**请求参数**
>其他参数请参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
name              |String  | 否   |  无   |  产品线名称

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Application Object](#application-object)

**请求示例**

        GET /productions/{id}/applications/

**响应示例**

        {
           'count': 100,
           'prev': null,
           'next': '/productions/{id}/applications/?page=2',
           'results': [
                {'id': 1, 'name': 'app-B', 'full_name': 'appA.app-B', 'has_child': true, 'parent_app': '2'},
                ....
           ]
        }
<a id="添加应用"></a>
### 添加应用
接口描述: &nbsp; 添加产品线应用
接口地址: &nbsp; /productions/{id}/applications/
请求方法: &nbsp; POST

**请求参数**
> 请求参数为以下对象列表

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
id                | Number | 是   |  无   | 应用id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /productions/{id}/applications/
        ContentType: 'application/json'
        [{'id': 1}, {'id': 2}]

**响应示例**

        {
           'message': 'success'
        }
<a id="删除应用-1"></a>
### 删除应用
接口描述: &nbsp; 删除产品线应用
接口地址: &nbsp; /productions/{id}/applications/
请求方法: &nbsp; DELETE

**请求参数**
> 请求参数为以下对象列表

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
id                | Number | 是   |  无   | 应用id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        DELETE /productions/{id}/applications/
        ContentType: 'application/json'
        [{'id': 1}, {'id': 2}]

**响应示例**

        {    
          'message': 'success'
        }

<a id="主机"></a>
## 主机
<a id="获取主机列表"></a>
### 获取主机列表
接口描述: &nbsp; 获取主机列表
接口地址: &nbsp; /hosts/
请求方法: &nbsp; GET

**请求参数**
> 其他参数请参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
name              | String | 否   |  无   | 主机名
host_type         | String | 否   |  无   | 主机类型

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host Object](#host-object)


**请求示例**

        GET /hosts/
        ContentType: 'application/json'


**响应示例**

        {
           'count': 100,
           'prev': null,
           'next': '/hosts/?page=2',
           'results': [{
                'id': 1,
                'name': 'host A',
                'host_type': 'ALI_ECS',
                'location': 'hangzhou',
                'status': 'attached',
                'os_status': 'running',
                'os_type': 'centos-7',
                'description': 'desription of host A',
                'ip_address': [
                    {'address': '10.10.10.2',
                     'netmask': '255.255.0.0',
                     'network': '10.10.0.0',
                     'is_virtual': false,
                     'addr_type': 'PRIVATE'},
                     ...
                     ],
                'cpu': 4,
                'memory': 8192,
            }]
        }
<a id="获取主机初始化任务"></a>
### 获取主机初始化任务
接口描述: &nbsp; 获取主机初始化任务列表
接口地址: &nbsp; /hosts/init-tasks/
请求方法: &nbsp; GET

**请求参数**
> 其他参数请参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |------------
hostname          | String | 否   | 无    | 任务相关主机名
creator           | String | 否   | 无    | 任务创建者

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host init task](#host-init-task)


**请求示例**

        GET /hosts/init-tasks/
        ContentType: 'application/json'


**响应示例**

        {
           'count': 100,
           'prev': null,
           'next': '/hosts/init-tasks/?page=2',
           'results': [
               {'id': 1,
               'creator': 'foo',
               'hosts': [
                    {'id': 1,
                    'name': 'host-A'},
                    {'id': 2,
                    'name': 'host-B'},
                    ...
               ],
               'opts': {
                     'zabbix_groups': ['host_group_A', 'host_group_B'],
                     'zabbix_templates': ['templateA', 'templateB']
                }，
               'created_time': '2018-04-18T15:38:40+08:00', 
               'finished_time': ' 2018-04-18T15:40:40+08:00',
               'status': 'running',},
               ...
               ]
        }

<a id="创建主机初始化任务"></a>
### 创建主机初始化任务
接口描述: &nbsp; 创建主机初始化任务
接口地址: &nbsp; /hosts/init-tasks/
请求方法: &nbsp; POST

**请求参数**
> 其他参数请参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |-----------
hosts             | Array  |   是 | 无    | Array of [Host](#host-object)
opts              | Object |   是 | 无    | [Host init task options](#host-init-task-options)

**返回内容**

[Host init task](#host-init-task)

**请求示例**

        POST /hosts/init-tasks/
        ContentType: 'application/json'
        {'hosts': [
             {'id': 1},
             {'id': 2},
              ...
          ],
         'opts': {
             'zabbix_groups': ['host_group_A', 'host_group_B'],
             'zabbix_templates': ['templateA', 'templateB']
          }，
        }


**响应示例**

    
        {'id': 1,
        'creator': 'foo',
        'hosts': [
             {'id': 1,
             'name': 'host-A'},
             {'id': 2,
             'name': 'host-B'},
             ...
        ],
        'opts': {
              'zabbix_groups': ['host_group_A', 'host_group_B'],
              'zabbix_templates': ['templateA', 'templateB']
         }，
        'created_time': '    2018-04-18T15:38:40+08:00', 
        'finished_time': ' 2018-04-18T15:40:40+08:00',
        'status': 'running',
        }


<a id="获取主机关联应用"></a>
### 获取主机关联应用
接口描述: &nbsp; 获取主机关联应用
接口地址: &nbsp; /hosts/{id}/applications/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Application](#application-object)

**请求示例**

        GET /hosts/{id}/applications/

**响应示例**

        {
            'count': 100,
            'next': '/hosts/{id}/applications/?page=2',
            'prev': null,
            'results': [
                {'id': 1, 
                 'name': 'application-A',
                 'full_name': 'parent.application-A'},
                 ...
            ]
        }

<a id="获取主机启动任务"></a>
### 获取主机启动任务
接口描述: &nbsp; 获取主机启动任务
接口地址: &nbsp; /hosts/start-tasks/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |-----------
creator           | String | 否   |  无   | 创建者
time__gt          | String | 否   |  无   | 大于时间
time__lt          | String | 否   |  无   | 小于时间
status            | String | 否   |  无   | 任务状态, 可选值['running', 'finished', 'failed']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host Start Task](#host-start-task)

**请求示例**
    
        GET /hosts/start-tasks/

**响应示例**

         [
            'count': 100,
            'next': '/hosts/start-tasks/?page=2',
            'prev': null,
            'results': [
                {'id': '13045745',
                 'hosts': [
                     {'id': 1, 'name': 'host-A'},
                     {'id': 2, 'name': 'host-B'}
                  ],
                 'creator': 'test_user',
                 'created_time': '2018-04-18T15:38:40+08:00',
                 'finished_time': '2018-04-18T15:40:40+08:00',
                 'status': 'finished',}
            ]
         ]

<a id="启动主机"></a>
#### 启动主机
接口描述: &nbsp; 启动主机
接口地址: &nbsp; /hosts/{id}/actions/start/
请求方法: &nbsp; POST

**请求参数**
    无

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机启动任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | 主机正在运行中
30003       |   500     | 重启失败
30004       |   500     | 未知错误

**请求示例**

        POST /hosts/{id}/actions/start/
        ContentType: 'application/json'



**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': '主机正在运行中.'}

<a id="批量启动主机"></a>
#### 批量启动主机
接口描述: &nbsp; 批量启动主机
接口地址: &nbsp; /hosts/start-tasks/
请求方法: &nbsp; POST

**请求参数**
>请求参数为下列对象列表

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
host_id           | Number | 是   |  无    | 主机id

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机启动任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | 主机正在运行中
30003       |   500     | 重启失败
30004       |   500     | 未知错误

**请求示例**

        POST /hosts/start-tasks/
        ContentType: 'application/json'
        [{'host_id': 1},
         {'host_id': 2},
         ...]


**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': '主机正在运行中.'}

<a id="获取主机停止任务"></a>
### 获取主机停止任务
接口描述: &nbsp; 获取主机停止任务
接口地址: &nbsp; /hosts/stop-tasks/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |-----------
creator           | String | 否   |  无   | 创建者
time__gt          | String | 否   |  无   | 大于时间
time__lt          | String | 否   |  无   | 小于时间
status            | String | 否   |  无   | 任务状态, 可选值['running', 'finished', 'failed']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host Stop Task](#host-stop-task)

**请求示例**
    
        GET /hosts/stop-tasks/

**响应示例**

         [
            'count': 100,
            'next': '/hosts/stop-tasks/?page=2',
            'prev': null,
            'results': [
                {'id': '13045745',
                 'hosts': [
                     {'id': 1, 'name': 'host-A'},
                     {'id': 2, 'name': 'host-B'}
                  ],
                 'creator': 'test_user',
                 'created_time': '2018-04-18T15:38:40+08:00',
                 'finished_time': '2018-04-18T15:40:40+08:00',
                 'status': 'finished',}
            ]
         ]
<a id="停止主机"></a>
#### 停止主机
接口描述: &nbsp; 停止主机
接口地址: &nbsp; /hosts/{id}/actions/stop/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
force             | Bool   | 否   |  false | 是否强制关闭

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机停止任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | cloudstack API调用失败
30003       |   500     | 腾讯云API调用失败
30004       |   500     | 腾讯云黑石物理机API调用失败

**请求示例**

        POST /hosts/{id}/actions/stop/
        ContentType: 'application/json'
        {'force': true}


**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}

<a id="批量停止主机"></a>
#### 批量停止主机
接口描述: &nbsp; 批量停止主机
接口地址: &nbsp; /hosts/stop-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
host_id           | Number | 是   |  无    | 主机id
force             | Bool   | 否   |  false | 是否强制关闭

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机停止任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | cloudstack API调用失败
30003       |   500     | 腾讯云API调用失败
30004       |   500     | 腾讯云黑石物理机API调用失败

**请求示例**

        POST /hosts/stop-tasks/
        ContentType: 'application/json'
        [{'host_id': 1, 'force': true},
         {'host_id': 2, 'force': false},
         ...]

**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}
<a id="重启主机"></a>
### 重启主机
<a id="获取主机重启任务"></a>
#### 获取主机重启任务
接口描述: &nbsp; 获取主机重启任务
接口地址: &nbsp; /hosts/restart-tasks/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值|说明
------------------|--------|------|------ |-----------
creator           | String | 否   |  无   | 创建者
time__gt          | String | 否   |  无   | 大于时间
time__lt          | String | 否   |  无   | 小于时间
status            | String | 否   |  无   | 任务状态, 可选值['running', 'finished', 'failed']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host Restart Task](#host-restart-task)

**请求示例**
    
        GET /hosts/restart-tasks/

**响应示例**

         [
            'count': 100,
            'next': '/hosts/restart-tasks/?page=2',
            'prev': null,
            'results': [
                {'id': '13045745',
                 'hosts': [
                     {'id': 1, 'name': 'host-A'},
                     {'id': 2, 'name': 'host-B'}
                  ],
                 'creator': 'test_user',
                 'created_time': '2018-04-18T15:38:40+08:00',
                 'finished_time': '2018-04-18T15:40:40+08:00',
                 'status': 'finished',}
            ]
         ]

<a id="重启主机-1"></a>
#### 重启主机
接口描述: &nbsp; 新建重启主机任务
接口地址: &nbsp; /hosts/{id}/actions/restart/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
force             | Bool   | 否   |  false | 是否强制重启

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机停止任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|-------------
30001       |   500     | saltstack 调用失败
30002       |   500     | cloudstack API调用失败
30003       |   500     | 腾讯云API调用失败
30004       |   500     | 腾讯云黑石物理机API调用失败

**请求示例**

        POST /hosts/{id}/actions/restart/
        ContentType: 'application/json'
        {'force': true}


**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}

<a id="批量重启主机"></a>
### 批量重启主机
接口描述: &nbsp; 批量重启主机
接口地址: &nbsp; /hosts/restart-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
host_id           | Number | 是   |  无    | 主机id
force             | Bool   | 否   |  false | 是否强制关闭

**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机停止任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | cloudstack API调用失败
30003       |   500     | 腾讯云API调用失败
30004       |   500     | 腾讯云黑石物理机API调用失败

**请求示例**

        POST /hosts/restart-tasks/
        ContentType: 'application/json'
        [{'host_id': 1, 'force': true},
         {'host_id': 2, 'force': false},
         ...]

**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}
<a id="更改主机状态"></a>
### 更改主机状态
接口描述: &nbsp; 更改主机状态
接口地址: &nbsp; /hosts/{id}/actions/change-status/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
status            | string | 是   |  无    | 可选值 ['attached', 'inited', 'raw', 'offline']


**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
task_id     | String | 主机停止任务Id

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | saltstack 调用失败
30002       |   500     | cloudstack API调用失败
30003       |   500     | 腾讯云API调用失败
30004       |   500     | 腾讯云黑石物理机API调用失败

**请求示例**

        POST /hosts/{id}/actions/change-status/
        ContentType: 'application/json'
        {'status': 'raw'}

**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}
<a id="更改主机状态"></a>
<a id="下架主机"></a>
### 下架主机
>参考 [更改主机状态](#更改主机状态)

**请求示例**

        POST /hosts/{id}/actions/change-status/
        ContentType: 'application/json'
        {'status': 'offline'}

**正确响应示例**

        {'task_id': '310034904'}

**错误响应示例**

        {'error_code': '30002',
         'message': 'cloudstack API 调用失败.'}

<a id="更新主机zbx配置"></a>
### 更新主机zbx配置
接口描述: &nbsp; 更改主机zabbix配置
接口地址: &nbsp; /hosts/{id}/actions/change-zabbix-opts/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
zabbix_groups     | Array  | 否   |  无    |  Array of zabbix group name
zabbix_templates  | Array  | 否   |  无    |  Array of zabbix template name


**正确返回**

属性        | 类型   | 说明
------------|--------|---------------
message     | String | success

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | zabbix API 调用失败
30002       |   500     | 模板不存在
30003       |   500     | zabbix group 不存在

**请求示例**

        POST /hosts/{id}/actions/change-zabbix-opts/
        ContentType: 'application/json'
        {'zabbix_groups': [
               'host_group_A','host_group_B'],        
         'zabbix_templates': [
               'templateA', 'templateB']}

**正确响应示例**
  
         {'message': 'success'}

**错误响应示例**
    
         {'error_code': 30002, 'message': '模板 "templateB" 不存在'}

<a id="资源申请"></a>
## 资源申请
<a id="申请服务器"></a>
### 申请服务器

<a id="获取服务器申请列表"></a>
#### 获取服务器申请列表
接口描述: &nbsp; 获取服务器申请列表
接口地址: &nbsp; /resource-request/hosts/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
creator           | String | 否   |  无    | 申请人
time__gt          | String | 否   |  无    | 大于时间
time__lt          | String | 否   |  无    | 小于时间
status            | String | 否   |  无    | 申请单状态, 可选值['approved', 'wait_review', 'rejected', 'closed', 'finished']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Host request](#host-request)

**请求示例**
    
        GET /resource-request/hosts/

**响应示例**

         {
            'count': 100,
            'next': '/resource-request/hosts/?page=2',
            'prev': null,
            'results': [
                {'id': 1,
                 'creator': 'test_user',
                 'created_time': '2018-04-18T15:38:40+08:00',
                 'purpose': '服务扩容',
                 'expect_delivery_days': '7',
                 'expiration': 'never',
                 'login_users': [
                    {'id': 1}, {'id': 2}
                 ],
                 'shiped_packackages': [
                    {'id': 3}, {'id': 4}
                 ],
                 'required_hosts': [
                    {'name': 'host-a',
                     'specs': {
                        'cpu_core': 4,
                        'mem': 8192,
                        'storage': 100000},
                     'os': 'centos-7.1',
                     'type': 'TECENT_CVM',
                    {'name': 'host-b',
                     'specs': {
                        'cpu_core': 4,
                        'mem': 8192,
                        'storage': 100000}
                     'os': 'centos-7.1',
                     'type': 'TECENT_CVM'},
                    ...
                 ],
                 },
              ...
            ]
         }

<a id="新建服务器申请"></a>
#### 新建服务器申请
接口描述: &nbsp; 新建服务器申请
接口地址: &nbsp; /resource-request/hosts/
请求方法: &nbsp; POST

**请求参数**

参数                | 类型   |必选|默认值 |说明
--------------------|--------|----|-------|----
purpose             | String | 是 | 无    |用途
expect_delivery_days| String | 否 | 7     |期望交付天数
expiration          | String | 否 |'never'|主机是否过期
login_users | Array  | 否 | 无    |Array of [User](#user-object)
shipped_packages    | Array  | 否 | 无    |Array of [Shipped Package](#shipped-package)
required_hosts      | Array  | 否 | 无    |Array of [Requested Host](#requested-host)

**返回内容**
    [Host Request](#host-request)


**请求示例**

        POST /resource-request/hosts/
        ContentType: 'application/json'
        {   
            'purpose': '服务扩容',
            'expect_delivery_days': '7',
            'expiration': 'never',
            'login_users': [
               {'id': 1}, {'id': 2}
            ],
            'shiped_packackages': [
               {'id': 3}, {'id': 4}
            ],
            'required_hosts': [
               {'name': 'host-A',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,               
                   'storage': 100000},
                'os': 'centos-7.1',
                'type': 'TECENT_CVM',
               {'name': 'host-b',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,
                   'storage': 100000}
                'os': 'centos-7.1',
                'type': 'TECENT_CVM'},
               ...
            ],
        }

<a id="获取服务器申请详情"></a>
#### 获取服务器申请详情
接口描述: &nbsp; 获取服务器申请详情
接口地址: &nbsp; /resource-request/hosts/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
    [Host Request](#host-request)

**请求示例**

        GET /resource-request/hosts/{id}/

**响应示例**

        {   
            'id': 1
            'purpose': '服务扩容',
            'expect_delivery_days': '7',
            'created_time': ''2018-04-18T15:38:40+08:00',
            'expiration': 'never',
            'login_users': [
               {'id': 1}, {'id': 2}
            ],
            'shiped_packackages': [
               {'id': 3}, {'id': 4}
            ],
            'required_hosts': [
               {'name': 'host-A',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,               
                   'storage': 100000},
                'os': 'centos-7.1',
                'type': 'TECENT_CVM',
               {'name': 'host-b',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,
                   'storage': 100000}
                'os': 'centos-7.1',
                'type': 'TECENT_CVM'},
               ...
            ],
        }

<a id="更新服务器申请"></a>
#### 更新服务器申请
接口描述: &nbsp; 更新服务器申请
接口地址: &nbsp; /resource-request/hosts/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数                | 类型   |必选|默认值|说明
--------------------|--------|----|------|----
purpose             | String | 否 | 无   |用途
expect_delivery_days| String | 否 | 无   |期望交付天数
expiration          | String | 否 | 无   |主机是否过期
users_with_log_perm | Array  | 否 | 无   |Array of [User](#user-object)
shipped_packages    | Array  | 否 | 无   |Array of [Shipped Package](#shipped-package)
required_hosts      | Array  | 否 | 无   |Array of [Requested Host](#requested-host)

**返回内容**
    [Host Request](#host-request)

**请求示例**

        PATCH /resource-request/hosts/{id}/
        ContentType: 'application/json'
        {   
            'purpose': '服务扩容',
            'expect_delivery_days': '7',
            'expiration': 'never',
            'login_users': [
               {'id': 1}, {'id': 2}
            ],
            'shiped_packackages': [
               {'id': 3}, {'id': 4}
            ],
            'required_hosts': [
               {'name': 'host-A',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,               
                   'storage': 100000},
                'os': 'centos-7.1',
                'type': 'TECENT_CVM',
               {'name': 'host-b',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,
                   'storage': 100000}
                'os': 'centos-7.1',
                'type': 'TECENT_CVM'},
               ...
            ],
        },

**正确响应**

        {   
            'id': 1,
            'creator': 'test_user',
            'created_time': '2018-04-18T15:38:40+08:00',
            'purpose': '服务扩容',
            'expect_delivery_days': '7',
            'expiration': 'never',
            'login_users': [
               {'id': 1}, {'id': 2}
            ],
            'shiped_packackages': [
               {'id': 3}, {'id': 4}
            ],
            'required_hosts': [
               {'name': 'host-A',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,               
                   'storage': 100000},
                'os': 'centos-7.1',
                'type': 'TECENT_CVM',
               {'name': 'host-b',
                'specs': {
                   'cpu_core': 4,
                   'mem': 8192,
                   'storage': 100000}
                'os': 'centos-7.1',
                'type': 'TECENT_CVM'},
               ...
            ],
        }

<a id="同意服务器申请"></a>
#### 同意服务器申请
接口描述: &nbsp; 新建服务器申请
接口地址: &nbsp; /resource-request/hosts/{id}/actions/approve/
请求方法: &nbsp; POST

**请求参数**
   无

**返回内容**

   属性        | 类型   | 说明
---------------|--------|---------
message        | String | success - 成功


**请求示例**

        POST /resource-request/hosts/{id}/actions/approve/

**响应示例**

        {'message': 'success'}

<a id="拒绝服务器申请"></a>
#### 拒绝服务器申请
接口描述: &nbsp; 拒绝服务器申请
接口地址: &nbsp; /resource-request/hosts/{id}/actions/reject/
请求方法: &nbsp; POST

**请求参数**
   无

**返回内容**

   属性        | 类型   | 说明
---------------|--------|---------
message        | String | success - 成功


**请求示例**

        POST /resource-request/hosts/{id}/actions/reject/

**响应示例**

        {'message': 'success'}

<a id="关闭服务器申请"></a>
#### 关闭服务器申请
接口描述: &nbsp; 关闭服务器申请
接口地址: &nbsp; /resource-request/hosts/{id}/actions/close/
请求方法: &nbsp; POST

**请求参数**
   无

**返回内容**

   属性        | 类型   | 说明
---------------|--------|---------
message        | String | success - 成功


**请求示例**

        POST /resource-request/hosts/{id}/actions/close/

**响应示例**

        {'message': 'success'}


<a id="申请域名"></a>
### 申请域名

<a id="获取域名申请列表"></a>
####  获取域名申请列表
接口描述: &nbsp; 获取域名申请列表
接口地址: &nbsp; /resource-request/domains/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
creator           | String | 否   |  无    | 申请人
time__gt          | String | 否   |  无    | 大于时间
time__lt          | String | 否   |  无    | 小于时间
status            | String | 否   |  无    | 任务状态, 可选值['approved', 'wait_review', 'rejected', 'closed', 'finished']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Domain Request](#domain-request)

**请求示例**
    
        GET /resource-request/domains/

**响应示例**

         {
            'count': 100,
            'next': '/resource-request/domains/?page=2',
            'prev': null,
            'results': [
                {
                 'id': '1',
                 'creator': 'test_user',
                 'created_time': ''2018-04-18T15:38:40+08:00',
                 'status': 'wait_review',
                 'records': [
                     {'record': 'record-a.example.com',
                      'value' '10.10.10.10',
                      'type': 'A'},
                     {'record': 'record-b.example.com',
                      'value' '10.10.10.11',
                      'type': 'A'}, 
                ]},
                ...
            ]
         }


<a id="新建域名申请"></a>
####  新建域名申请
接口描述: &nbsp; 新建域名申请
接口地址: &nbsp; /resource-request/domains/
请求方法: &nbsp; POST

**请求参数*

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
associated_app    | Array  | 否   |  无    | Array of appliation id
records           | Array  | 是   |  无    | Array of [Requested Dns Record](#requested-dns-record)

**返回内容**

[Domain request](#domain-request)

**请求示例**

        POST /resource-request/domains/
        ContentType: 'application/json'
        {'records': [
            {'record': 'record-a.example.com',
             'value': '10.10.10.10',
             'type': 'A'},
             {'record': 'record-b.example.com',
             'value': '10.10.10.11',
             'type': 'A'},
        ]}

**响应示例**

        { 
          'id': '1',
          'creator': 'test_user',
          'status': 'wait_review',
          'created_time': ''2018-04-18T15:38:40+08:00',
          'records': [
              {'record': 'record-a.example.com',
               'value' '10.10.10.10',
               'type': 'A'},
              {'record': 'record-b.example.com',
               'value' '10.10.10.11',
               'type': 'A'}, 
           ]
        }


<a id="获取域名申请详情"></a>
####  获取域名申请详情
接口描述: &nbsp; 获取域名申请详情
接口地址: &nbsp; /resource-request/domains/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
   [Domian request](#domain-request)

**请求示例**

        GET /resource-request/domains/{id}/
   

**响应示例**

        { 
          'id': '1',
          'creator': 'test_user',
          'status': 'wait_review',
          'created_time': ''2018-04-18T15:38:40+08:00',
          'records': [
              {'record': 'record-a.example.com',
               'value' '10.10.10.10',
               'type': 'A'},
              {'record': 'record-b.example.com',
               'value' '10.10.10.11',
               'type': 'A'}, 
           ]
        }


<a id="更新域名申请"></a>
####  更新域名申请
接口描述: &nbsp; 更改域名申请
接口地址: &nbsp; /resource-request/domains/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
associated_app    | Array  | 否   |  无    | Array of appliation id
records           | Array  | 是   |  无    | Array of [Requested Dns Record](#requested-dns-record)

**返回内容**

[Domain request](#domain-request)

**请求示例**

        PATCH /resource-request/domains/{id}/
        ContentType: 'application/json'
        {'records': [
            {'record': 'record-a.example.com',
             'value': '10.10.10.10',
             'type': 'A'},
             {'record': 'record-b.example.com',
             'value': '10.10.10.11',
             'type': 'A'},
        ]}

**响应示例**

        { 
          'id': '1',
          'creator': 'test_user',
          'status': 'wait_review',
          'created_time': ''2018-04-18T15:38:40+08:00',
          'records': [
              {'record': 'record-a.example.com',
               'value' '10.10.10.10',
               'type': 'A'},
              {'record': 'record-b.example.com',
               'value' '10.10.10.11',
               'type': 'A'}, 
           ]
        }

<a id="批准域名申请"></a>
####  批准域名申请
接口描述: &nbsp; 批准域名申请
接口地址: &nbsp; /resource-request/domains/{id}/actions/approve/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /resource-request/domains/{id}/actions/approve/

**响应示例**

        {"message": "success"}

<a id="拒绝域名申请"></a>
####  拒绝域名申请
接口描述: &nbsp; 拒绝域名申请
接口地址: &nbsp; /resource-request/domains/{id}/actions/reject/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /resource-request/domains/{id}/actions/reject/

**响应示例**

        {"message": "success"}

<a id="关闭域名申请"></a>
####  关闭域名申请
接口描述: &nbsp; 关闭域名申请
接口地址: &nbsp; /resource-request/domains/{id}/actions/close/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /resource-request/domains/{id}/actions/close/

**响应示例**

        {"message": "success"}

<a id="申请域名ssl证书"></a>
### 申请域名SSL证书

<a id="获取ssl证书申请列表"></a>

<a id="获取ssl证书申请列表"></a>
#### 获取ssl证书申请列表
接口描述: &nbsp; 获取ssl证书申请列表
接口地址: &nbsp; /resource-request/ssl-certificates/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
creator           | String | 否   |  无    | 申请人
time__gt          | String | 否   |  无    | 大于时间
time__lt          | String | 否   |  无    | 小于时间
domain            | String | 否   |  无    | 证书域名
certificate_type  | String | 否   |　无　　| 证书类型，可选值 ['wizard', 'normal'] <br> <ul><li>wizard - 通配符类型</li><li>normal - 普通类型</li></ul>
status            | String | 否   |  无    | 任务状态, 可选值['approved', 'wait_review', 'rejected', 'closed', 'finished']

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [SSL certificate request](#ssl-certificate-request)

**请求示例**
    
        GET /resource-request/ssl-certificates/

**响应示例**

         {
            'count': 100,
            'next': '/resource-request/ssl-certificates/?page=2',
            'prev': null,
            'results': [
                {
                 'id': '1',
                 'creator': 'test_user',
                 'created_time': ''2018-04-18T15:38:40+08:00',
                 'status': 'wait_review',
                 'domain': 'example.com',
                 'certificate_type': 'wizard'
                 'expect_delivery_days': '7',
                 'purpose': 'description of purpose'
                 },
                ...
            ]
         }

<a id="新建ssl证书申请"></a>
#### 新建ssl证书申请
接口描述: &nbsp; 新建ssl证书申请
接口地址: &nbsp; /resource-request/ssl-certificates/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
domain            | String | 是   |  无    | 证书域名
certificate_type  | String | 是   |  无    | 证书类型，可选值 ['wizard', 'normal'] <br> <ul><li>wizard - 通配符类型</li><li>normal - 普通类型</li></ul>
associate_app     | Array  | 否   |  无    | Array of application id, 证书关联应用id列表
purpose           | String | 否   |  无    | 证书用途


**请求示例**

        POST /resource-request/ssl-certificates/
        ContentType: 'application/json'
        {
           'domain': 'example.com',
           'certificate_type': 'wizard'，
           'expect_delivery_days': '7',
           'purpose': 'description of purpose'
    }

**响应示例**

        {
           'id': 1,
           'creator': 'test_user',
           'created_time': ''2018-04-18T15:38:40+08:00',
           'status': 'wait_review',
           'domain': 'example.com',
           'certificate_type': 'wizard'，
           'expect_delivery_days': '7',
           'purpose': 'description of purpose'
        }

<a id="获取ssl证书申请详情"></a>
#### 获取ssl证书申请详情
接口描述: &nbsp; 获取ssl证书申请详情
接口地址: &nbsp; /resource-request/ssl-certificates/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**响应内容**
[SSL certificate request](#ssl-certificate-request)

**请求示例**

        GET /resource-request/ssl-certificates/{id}/

**响应示例**

        {
           'id': 1,
           'creator': 'test_user',
           'created_time': ''2018-04-18T15:38:40+08:00',
           'status': 'wait_review',
           'domain': 'example.com',
           'certificate_type': 'wizard'，
           'expect_delivery_days': '7',
           'purpose': 'description of purpose'
        }



<a id="更新ssl证书申请"></a>
#### 更新ssl证书申请
接口描述: &nbsp; 更新ssl证书申请
接口地址: &nbsp; /resource-request/ssl-certificates/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名               | 类型   | 必选 | 默认值 |说明
---------------------|--------|------|--------|-----------
domain               | String | 否   |  无    | 证书域名
certificate_type     | String | 否   |  无    | 证书类型，可选值 ['wizard', 'normal'] <br> <ul><li>wizard - 通配符类型</li><li>normal - 普通类型</li></ul>
associate_app        | Array  | 否   |  无    | Array of application id, 证书关联应用id列表
purpose              | String | 否   |  无    | 证书用途
expect_delivery_days | String | 否   |  7     | 期望交付天数


**请求示例**

        PATCH /resource-request/ssl-certificates/{id}/
        ContentType: 'application/json'
        {
           'domain': 'example.com',
           'certificate_type': 'wizard'，
           'expect_delivery_days': '7',
           'purpose': 'description of purpose'
        }

**响应示例**

        {
           'id': 1,
           'creator': 'test_user',
           'created_time': '2018-04-18T15:38:40+08:00',
           'status': 'wait_review',
           'domain': 'example.com',
           'certificate_type': 'wizard'，
           'expect_delivery_days': '7',
           'purpose': 'description of purpose'
        }


<a id="同意ssl证书申请"></a>
#### 同意ssl证书申请
接口描述: &nbsp; 同意ssl证书申请
接口地址: &nbsp; /resource-request/ssl-certificates/{id}/actions/approve/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**错误内容**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      | 类型   | 说明
------------|--------|-------------
30001       | Number | 申请单已批准
30002       | String | 申请单已关闭
30003       | String | 申请单已完成


**请求示例**

    POST /resource-request/ssl-certificates/{id}/actions/approve/

**响应示例**

    {"message": "success"}

**错误响应示例**
    
    {"error_code": 30001, "message": "申请单已批准"}

<a id="拒绝ssl证书申请"></a>
#### 拒绝ssl证书申请
接口描述: &nbsp; 拒绝ssl证书申请
接口地址: &nbsp; /resource-request/ssl-certificates/{id}/actions/reject/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**错误内容**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      | 类型   | 说明
------------|--------|-------------
30001       | Number | 申请单已批准
30002       | String | 申请单已关闭
30002       | String | 申请单已完成


**请求示例**

        POST /resource-request/ssl-certificates/{id}/actions/reject/

**响应示例**

        {"message": "success"}

**错误响应示例**
    
        {"error_code": 30001, "message": "申请单已批准"}

<a id="关闭ssl证书申请"></a>
#### 关闭ssl证书申请
接口描述: &nbsp; 关闭ssl证书申请
接口地址: &nbsp; /resource-request/ssl-certificates/{id}/actions/close/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

属性        | 类型   | 说明
------------|--------|-------------
30001       | Number | 申请单已批准
30002       | String | 申请单已关闭
30002       | String | 申请单已完成


**请求示例**

        POST /resource-request/ssl-certificates/{id}/actions/close/

**响应示例**

        {"message": "success"}

**错误响应示例**
    
        {"error_code": 30001, "message": "申请单已批准"}

<a id="dns服务"></a>
## DNS服务

<a id="获取服务器列表"></a>
### 获取服务器列表
接口描述: &nbsp; 获取服务器列表
接口地址: &nbsp; /dns-services/
请求方法: &nbsp; POST

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
creator           | String | 否   |  无    | 申请人
name              | String | 否   |  无    | 名称
description       | String | 否   |  无    | 描述


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [DNS Server](#dns-server)

**请求示例**
    
        GET /dns-services/

**响应示例**

         {
            'count': 100,
            'next': '/dns-services/?page=2',
            'prev': null,
            'results': [
                {
                 'id': '1',
                 'name': 'server A',
                 'creator': 'test user',
                 'created_time': '2018-04-18T15:38:40+08:00'
                 'type': 'bind',
                 'api_endpoint': 'http://127.0.0.1:8053/'
                 },
                ...
            ]
         }

<a id="添加域名服务器"></a>
### 添加域名服务器
接口描述: &nbsp; 添加域名服务器
接口地址: &nbsp; /dns-services/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |  无    | 服务器名称
type              | String | 是   | 'bind' | 可选值 ['bind', 'powerdns']
api_endpoint      | String | 是   | 无     | dns服务器api接口地址
description       | String | 是   | 无     | 描述



**请求示例**

        POST /dns-services/
        ContentType: 'application/json'
        {
           'name': 'server A',
           'type': 'bind',
           'api_endpoint': 'http://127.0.0.1:8053/''
           'description': 'desc of server'
        }

**响应示例**

        {
            'id': '1',
            'name': 'server A',
            'creator': 'test user',
            'created_time': '2018-04-18T15:38:40+08:00'
            'type': 'bind',
            'api_endpoint': 'http://127.0.0.1:8053/'
        }

<a id="获取服务器域名列表"></a>
### 获取服务器域名列表
接口描述: &nbsp; 获取服务器域名列表
接口地址: &nbsp; /dns-services/{id}/domains/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 域名


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [DNS domain](#dns-domain)

**请求示例**
    
        GET /dns-services/{id}/domains/

**响应示例**

         {
            'count': 100,
            'next': '/dns-services/{id}/domains/?page=2',
            'prev': null,
            'results': [
                {
                 'id': '1',
                 'name': 'domain-a.com',
                 },
                {
                 'id': '2',
                 'name': 'domain-b.com',
                 },
                ...
            ]
         }

<a id="添加域名"></a>
### 添加域名
接口描述: &nbsp; 添加域名
接口地址: &nbsp; /dns-services/{id}/domains/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |  无    | 域名


**返回内容**
[DNS domain](#dns-domain)

**请求示例**
    
        POST /dns-services/{id}/domains/
        ContentType: 'application/json'
        {        
            'name': 'domain-a.com',
        }

**响应示例**

        {
            'id': '1',
            'name': 'domain-a.com',
        }
  
<a id="更新域名"></a>
### 更新域名
接口描述: &nbsp; 添加域名
接口地址: &nbsp; /dns-services/{id}/domains/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 域名


**返回内容**
[DNS domain](#dns-domain)

**请求示例**
    
        PATCH /dns-services/{id}/domains/{id}/

**响应示例**

        {
            'id': '1',
            'name': 'domain-a.com',
        }
  
<a id="删除域名"></a>
### 删除域名
接口描述: &nbsp; 删除域名
接口地址: &nbsp; /dns-services/{id}/domains/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        DELETE /dns-services/{id}/domains/{id}
  

**响应示例**

        {
            "message": "success"
        }

<a id="域名记录"></a>
###  域名记录

<a id="获取域名记录列表"></a>
#### 获取域名记录列表
接口描述: &nbsp; 获取域名记录
接口地址: &nbsp; /dns-services/{id}/domains/{id}/records/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 记录名
value             | String | 否   |  无    | 记录值
type              | String | 否   |  无    | 记录类型


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [domain record](#dns-domain-record)

**请求示例**
    
        GET /dns-services/{id}/domains/{id}/records/

**响应示例**

        {
            'count': 100,
            'next': '/dns-services/{id}/domains/{id}/records/?page=2',
            'prev': null,
            'results': [
                {
                 'id': '1',
                 'name': 'record-a.domain-a.com',
                 'value': '10.10.10.10',
                 'type': 'A'
                },
                {
                 'id': '2',
                 'name': 'record-b.domain-a.com',
                 'value': '10.10.10.11',
                 'type': 'A'
                },
                ...
            ]
         }

<a id="添加域名记录"></a>
#### 添加域名记录
接口描述: &nbsp; 添加域名记录
接口地址: &nbsp; /dns-services/{id}/domains/{id}/records/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |  无    | 记录名
value             | String | 是   |  无    | 记录值
type              | String | 是   |  无    | 记录类型

**返回内容**
[domain record](#dns-domain-record)

**请求示例**
    
        POST /dns-services/{id}/domains/{id}/records/
        ContentType: 'application/json'
        {
            'name': 'record-a.domain-a.com',
            'value': '10.10.10.10',
            'type': 'A'
        }

**响应示例**

        {
            'id': '1',
            'name': 'record-a.domain-a.com',
            'value': '10.10.10.10',
            'type': 'A'
        }

<a id="更新域名记录"></a>
#### 更新域名记录
接口描述: &nbsp; 更新域名记录
接口地址: &nbsp; /dns-services/{id}/domains/{id}/records/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 记录名
value             | String | 否   |  无    | 记录值
type              | String | 否   |  无    | 记录类型

**返回内容**
[domain record](#dns-domain-record)

**请求示例**
    
        PATCH /dns-services/{id}/domains/{id}/records/
        ContentType: 'application/json'
        {
            'name': 'record-a.domain-a.com',
            'value': '10.10.10.10',
            'type': 'A'
        }

**响应示例**

        {
            'id': '1',
            'name': 'record-a.domain-a.com',
            'value': '10.10.10.10',
            'type': 'A'
        }

<a id="删除域名记录"></a>
#### 删除域名记录
接口描述: &nbsp; 删除域名记录
接口地址: &nbsp; /dns-services/{id}/domains/{id}/records/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        DELETE /dns-services/{id}/domains/{id}/{records}/{id}/
  

**响应示例**

        {
            "message": "success"
        }

<a id="禁用域名记录"></a>
#### 禁用域名记录
接口描述: &nbsp; 禁用域名记录
接口地址: &nbsp; /dns-services/{id}/domains/{id}/records/actions/disable/
请求方法: &nbsp; POST

**请求参数**
>Array of below

参数名      | 类型   | 必选 | 默认值 | 说明
------------|--------|------|--------|-------------
id          | Number | 是   | 无     | 域名记录ID

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        POST /dns-services/{id}/domains/{id}/records/actions/disable/
        ContentType: 'application/json'
        [{'id': 1}, {'id': 2}, ...]
  

**响应示例**

        {
            "message": "success"
        }


<a id="发布模板"></a>
## 发布模板
<a id="获取发布模板列表"></a>
### 获取发布模板列表
接口描述: &nbsp; 获取发布模板列表
接口地址: &nbsp; /application/deploy-templates/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 模板名
creator           | String | 否   |  无    | 创建人

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Application deploy template](#application-deploy-template)

**请求示例**
    
        GET /application/deploy-templates/

**响应示例**

        {
            'count': 100,
            'next': '/application/deploy-templates/?page=2',
            'prev': null,
            'results': [
                {
                    'id': 1
                    'enabled': true,
                    'applictions': [{'id': 1}, {'id': 2}],
                    'creator': 'test_user',
                    'repository': {
                        'type': 'GIT',
                        'url': 'http://git.example.com/test',
                        'branch': 'release',
                        'credential': {
                            'type': 'PASSWORD'
                            'username': 'username',
                            'password': 'pasword'
                         }
                     },
                    'deploy_path': '/path/to/deploy/path',
                    'timeout': 120,
                    'keep_backups': 5,
                    'lifecycle_hooks': {
                         'running_user': 'work',
                         'global_pre_exec': null,
                         'pre_exec': {
                            'script':  {
                                'id': 1,
                                'name': 'pre exec script',
                                'language': 'bash',
                                'content': 'echo "test"',
                                'template_engine': 'jinja',
                             }
                          },
                          'post_exec': {
                             'script':  {
                                'id': 2,
                                'name': 'post exec script',
                                ‘language': 'bash',
                                'content': 'echo "test"',
                                'template_engine': 'jinja'
                              }
                          },
                          'glboal_post_exec': null,
                     }
                },
                ...
            ]
        }

<a id="新建发布模板"></a>
### 新建发布模板
接口描述: &nbsp; 新建发布模板
接口地址: &nbsp; /application/deploy-templates/
请求方法: &nbsp; POST

**请求参数**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
name                 | String | 是   |  无    |模板名
applications         | Array  | 否   |  无    |关联应用Id列表
repository           | Object | 是   |  无    |应用源码仓库,  可能的类型为<ul><li>[ftp repo arguments](#ftp-repository-arguments) </li><li>[git repo arguments](#git-repository-arguments)</li></ul>
deploy_path          | String | 是   |  无    |发布路径
timeout              | Number | 否   |  120   |发布任务执行超时时间
keep_backups         | Number | 否   |  5     |保留最近备份数
lifecycle_hooks      | Array  | 否   |  无    | [deploy task lifecycle hooks](#deploy-task-lifecycle-hooks)

<a id='ftp-repository-arguments'></a>
**FTP Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 是   |  无    | ftp地址
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 是  | 无  | 登录凭据

<a id='git-repository-arguments'></a>
**GIT Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 是   |  无    | git仓库地址
branch               | String | 是   |  无    | git仓库分支
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 是  | 无  | 登录凭据

**返回内容**
[Application deploy template](#application-deploy-template)

**请求示例**
    
        POST /application/deploy-templates/
        ContentType: 'application/json'
        {
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': 1,
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                      }
                  },
                  'glboal_post_exec': null,
            }
        }

**响应示例**

        {
            'id': 1
            'enabled': true,
            'creator': 'test_user',
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': {
                    'type': 'PASSWORD'
                    'username': 'username',
                    'password': 'pasword'
                 }
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                        'name': 'pre exec script',
                        'language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja',
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                        'name': 'post exec script',
                        ‘language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja'
                      }
                  },
                  'glboal_post_exec': null,
             }
        }



<a id="获取发布模板详情"></a>
### 获取发布模板详情
接口描述: &nbsp; 获取发布模板详情
接口地址: &nbsp; /application/deploy-templates/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
[Application deploy template](#application-deploy-template)

**请求示例**

    GET /application/deploy-templates/{id}/
    
**响应示例**

        {
            'id': 1
            'enabled': true,
            'creator': 'test_user',
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': {
                    'type': 'PASSWORD'
                    'username': 'username',
                    'password': 'pasword'
                 }
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                        'name': 'pre exec script',
                        'language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja',
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                        'name': 'post exec script',
                        ‘language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja'
                      }
                  },
                  'glboal_post_exec': null,
             }
        }

<a id="更新发布模板"></a>
### 更新发布模板
接口描述: &nbsp; 更新发布模板
接口地址: &nbsp; /application/deploy-templates/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
name                 | String | 否   |  无    |模板名
applications         | Array  | 否   |  无    |关联应用Id列表
repository           | Object | 否   |  无    |应用源码仓库,  可能的类型为<ul><li>[ftp repo arguments](#ftp-repository-arguments) </li><li>[git repo arguments](#git-repository-arguments)</li></ul>
deploy_path          | String | 否   |  无    |发布路径
timeout              | Number | 否   |  120   |发布任务执行超时时间
keep_backups         | Number | 否   |  5     |保留最近备份数
lifecycle_hooks      | Array  | 否   |  无    |[deploy task lifecycle hooks](#deploy-task-lifecycle-hooks)

<a id='ftp-repository-arguments'></a>
**FTP Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 否   |  无    | ftp地址
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 否  | 无  | 登录凭据

<a id='git-repository-arguments'></a>
**GIT Repository arguments**

参数名               |  类型  | 必选 | 默认值 | 说明
---------------------|--------|------|--------|-------
url                  | String | 否   |  无    | git仓库地址
branch               | String | 否   |  无    | git仓库分支
credential           | credential id  &vert; [password crendential](#password-credential)  &vert; [ssh private key credential](#ssh-private-key-credential) | 是  | 无  | 登录凭据

**返回内容**
[Application deploy template](#application-deploy-template)

**请求示例**
    
        PATCH /application/deploy-templates/{id}/
        ContentType: 'application/json'
        {
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': 1,
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                      }
                  },
                  'glboal_post_exec': null,
            }
        }

**响应示例**

        {
            'id': 1
            'enabled': true,
            'creator': 'test_user',
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': {
                    'type': 'PASSWORD'
                    'username': 'username',
                    'password': 'pasword'
                 }
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                        'name': 'pre exec script',
                        'language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja',
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                        'name': 'post exec script',
                        ‘language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja'
                      }
                  },
                  'glboal_post_exec': null,
             }
        }

<a id="删除发布模板"></a>
#### 删除发布模板
接口描述: &nbsp; 删除发布模板
接口地址: &nbsp; /application/deploy-templates/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        DELETE /application/deploy-templates/{id}/
  

**响应示例**

        {
            "message": "success"
        }

<a id="发布脚本"></a>
### 发布脚本

<a id="获取发布脚本列表"></a>
####  获取发布脚本列表
接口描述: &nbsp; 获取发布脚本列表
接口地址: &nbsp; /application/deploy-scripts/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 脚本名
creator           | String | 否   |  无    | 创建人
language          | String | 否   |  无    | 语言
content           | String | 否   |  无    | 内容
否
**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [deploy script](#deploy-script)

**请求示例**
    
        GET /application/deploy-scripts/

**响应示例**

        {
            'id': 1
            'enabled': true,
            'creator': 'test_user',
            'repository': {
                'type': 'GIT',
                'url': 'http://git.example.com/test',
                'branch': 'release',
                'credential': {
                    'type': 'PASSWORD'
                    'username': 'username',
                    'password': 'pasword'
                 }
             },
            'deploy_path': '/path/to/deploy/path',
            'timeout': 120,
            'keep_backups': 5,
            'lifecycle_hooks': {
                 'running_user': 'work',
                 'global_pre_exec': null,
                 'pre_exec': {
                    'script':  {
                        'id': 1,
                        'name': 'pre exec script',
                        'language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja',
                     }
                  },
                  'post_exec': {
                     'script':  {
                        'id': 2,
                        'name': 'post exec script',
                        ‘language': 'bash',
                        'content': 'echo "test"',
                        'template_engine': 'jinja'
                      }
                  },
                  'glboal_post_exec': null,
             }
        }

<a id="新建发布脚本"></a>
####  新建发布脚本
接口描述: &nbsp; 新建发布脚本
接口地址: &nbsp; /application/deploy-scripts/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |  无    | 脚本名
creator           | String | 是   |  无    | 创建人
language          | String | 是   |  无    | 语言
content           | String | 是   |  无    | 内容
template_engine   | String | 否   | 'jinja'| 脚本渲染引擎

**正确返回**
    [deploy script](#deploy-script)

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | 脚本名称已存在
30002       |   500     | 语言不支持
30003       |   500     | 脚本引擎不支持

**请求示例**

        POST /application/deploy-scripts/
        ContentType: 'application/json'
        {
            'name': 'script a',
            'language': 'bash',
            'content': 'echo "script a"'
        }

**响应示例***

        {
            'id': 1,
            'name': 'script a',
            'creator': 'admin',
            'language': 'bash',
            'content': 'echo "script a"',
            'template_engine': 'jinja'
        }

<a id="获取发布脚本"></a>
####  获取发布脚本
接口描述: &nbsp; 获取发布脚本
接口地址: &nbsp; /application/deploy-scripts/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容*
    [deploy script](#deploy-script)

**请求示例**
   
        GET /application/deploy-scripts/{id}/

**响应示例**

        {
            'id': 1,
            'name': 'script a',
            'creator': 'admin',
            'language': 'bash',
            'content': 'echo "script a"',
            'template_engine': 'jinja'
        }

<a id="更新发布脚本"></a>
#### 更新发布脚本
接口描述: &nbsp; 更新发布脚本
接口地址: &nbsp; /application/deploy-scripts/{id}/
请求方法: &nbsp; PATCH


**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 记录名
creator           | String | 否   |  无    | 创建人
language          | String | 否   |  无    | 语言
content           | String | 否   |  无    | 内容
template_engine   | String | 否   | 'jinja'| 脚本渲染引擎

**正确返回**
    [deploy script](#deploy-script)

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   500     | 脚本名称已存在
30002       |   500     | 语言不支持
30003       |   500     | 脚本引擎不支持

**请求示例**

        PATCH /application/deploy-scripts/{id}/
        ContentType: 'application/json'
        {
            'name': 'script a',
            'language': 'bash',
            'content': 'echo "script a"'
        }

**响应示例***

        {
            'id': 1,
            'name': 'script a',
            'creator': 'admin',
            'language': 'bash',
            'content': 'echo "script a"',
            'template_engine': 'jinja'
        }


<a id="获取脚本关联应用"></a>
#### 获取脚本关联应用
接口描述: &nbsp; 获取脚本关联应用
接口地址: &nbsp; /application/deploy-scripts/{id}/applications/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [application object](#application-object)

**请求示例**
    
        GET /application/deploy-scripts/{id}/applications/

**响应示例**

        {
            'count': 100,
            'next': '/application/deploy-scripts/{id}/applications/?page=2',
            'prev': null,
            'results': [
                 {'id': 1, 
                  'name': 'application-a',
                  'full_name: 'parent.application-a'},
                 {'id': 2, 
                  'name': 'application-a',
                  'full_name: 'parent.application-a'},
                 ...
             ]
        }

<a id="删除发布脚本"></a>
#### 删除发布脚本
接口描述: &nbsp; 删除发布脚本
接口地址: &nbsp; /application/deploy-scripts/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        DELETE /application/deploy-scripts/{id}/
  

**响应示例**

        {
            "message": "success"
        }

<a id="登录凭据"></a>
### 登录凭据

<a id="获取密码登录凭据列表"></a>
#### 获取密码登录凭据列表
接口描述: &nbsp; 获取密码登录凭据列表
接口地址: &nbsp; /application/repository-credentials/password/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 凭据名称
username          | String | 否   |  无    | 用户名


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [password credential](#password-credential)

**请求示例**
    
        GET /application/repository-credentials/password/

**响应示例**

        {
            'count': 100,
            'next': '/application/repository-credentials/password/?page=2',
            'prev': null,
            'results': [
                 {'id': 1, 
                  'name': 'credential-a',
                  'username': 'username',
                  'password': 'password'},
                 {'id': 1, 
                  'name': 'credential-a',
                  'username': 'username',
                  'password': 'password'},
             ]
        }

<a id="创建密码登录凭据"></a>
#### 创建密码登录凭据
接口描述: &nbsp; 创建密码登录凭据
接口地址: &nbsp; /application/repository-credentials/password/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 凭据名称
username          | String | 否   |  无    | 用户名
password          | String | 否   |  无    | 密码


**返回内容**

[password credential](#password-credential)

**请求示例**
    
        POST /application/repository-credentials/password/
        ContentType: 'application/json'
        {
            'name': 'credential-a',
            'username': 'username',
            'password': 'password'
        }

**响应示例**

        {
             'id': 1, 
             'name': 'credential-a',
             'username': 'username',
             'password': 'password'
        }

<a id="更新密码登录凭据"></a>
#### 更新密码登录凭据
接口描述: &nbsp; 更新密码登录凭据
接口地址: &nbsp; /application/repository-credentials/password/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 凭据名称
username          | String | 否   |  无    | 用户名
password          | String | 否   |  无    | 密码


**返回内容**

[password credential](#password-credential)

**请求示例**
    
        PATCH /application/repository-credentials/password/
        ContentType: 'application/json'
        {
            'name': 'credential-a',
            'username': 'username',
            'password': 'password'
        }

**响应示例**

        {
             'id': 1, 
             'name': 'credential-a',
             'username': 'username',
             'password': 'password'
        }

<a id="删除密码登录凭据"></a>
#### 删除密码登录凭据
接口描述: &nbsp; 删除密码登录凭据
接口地址: &nbsp; /application/repository-credentials/password/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功


**请求示例**
    
        DELETE /application/repository-credentials/password/{id}/
  

**响应示例**

        {
            "message": "success"
        }

<a id="用户"></a>
## 用户
<a id="获取用户列表"></a>
### 获取用户列表
接口描述: &nbsp; 获取用户列表
接口地址: &nbsp; /users/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
username          | String | 否   |  无    | 用户名
email             | String | 否   |  无    | 邮箱
phone             | String | 否   |  无    | 手机号码
status            | String | 否   |  无    | 用户状态, 可选值['enabled', 'disabled']
 

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [User object](#user-object)

**请求示例**
    
        GET /users/
  
**响应示例**


        {
            'count': 100,
            'next': '/users/?page=2',
            'prev': null,
            'results': [
                 {'id': 1, 
                  'username': 'user-a',
                  'email': 'user-a@example.com',
                  'phone': '12345678901'},
                 {'id': 2, 
                  'name': 'user-b',
                  'username': 'user-b@weimob.com',
                  'phone': '12345678902'},
             ]
        }


<a id="获取用户详情"></a>
### 获取用户详情
接口描述: &nbsp; 获取用户配置
接口地址: &nbsp; /users/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
[User object](#user-object)

**请求示例**
    
        GET /users/{id}/
  
**响应示例**

        {
            'id': 1, 
            'username': 'user-a',
            'email': 'user-a@example.com',
            'phone': '12345678901'
        }


<a id="更新用户"></a>
### 更新用户
接口描述: &nbsp; 更新用户配置
接口地址: &nbsp; /users/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
email             | String | 否   |  无    | 邮箱
phone             | String | 否   |  无    | 手机号码

**返回内容**
[User object](#user-object)

**请求示例**
    
    PATCH /users/{id}/
    ContentType: 'application/json'
    {
        'email': 'user-a@example.com',
        'phone': '12345678901'
    }
  
**响应示例**

    {
        'id': 1, 
        'username': 'user-a',
        'status': 'enabled',
        'email': 'user-a@example.com',
        'phone': '12345678901'
    }


<a id="分配用户角色"></a>
### 分配用户角色
接口描述: &nbsp; 分配用户角色
接口地址: &nbsp; /users/{id}/roles/
请求方法: &nbsp; POST

**请求参数**
> Array of bellow object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
id                | Number | 是   |  无    | 角色id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /users/{id}/roles/
        CopntentType: 'application/json'
        [
            {'id': 1},
            {'id': 2},
            ...
        ]

**响应示例**

        {
            "message": "success"
        }

<a id="移除用户角色"></a>
### 移除用户角色
接口描述: &nbsp; 移除用户角色
接口地址: &nbsp; /users/{id}/roles/
请求方法: &nbsp; DELETE

**请求参数**
> Array of bellow object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
id                | Number | 是   |  无    | 角色id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        DELETE /users/{id}/roles/
        CopntentType: 'application/json'
        [
            {'id': 1},
            {'id': 2},
            ...
        ]

**响应示例**

        {
            "message": "success"
        }

<a id="禁用用户"></a>
### 禁用用户
接口描述: &nbsp; 移除用户角色
接口地址: &nbsp; /users/{id}/actions/disable/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /users/{id}/actions/disable/

**响应示例**

        { "message": "success"}

<a id="启用用户"></a>
### 启用用户
接口描述: &nbsp; 移除用户角色
接口地址: &nbsp; /users/{id}/actions/enable/
请求方法: &nbsp; POST

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /users/{id}/actions/disable/

**响应示例**

        { "message": "success"}


<a id="更改密码"></a>
### 更改密码
接口描述: &nbsp; 更改密码
接口地址: &nbsp; /users/{id}/actions/change-password/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
original_password | String | 是   |  无    | 原始密码
new_password      | String | 是   |  无    | 新密码

**正确返回**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误消息

**错误码**

错误码      | http状态码 | 说明
------------|------------|---------
300001      | 400        | 原始密码错误


**请求示例**

        POST /users/{id}/actions/change-password/
        ContentType：'application/json'
        {
            "original_password": 'original_password',
            "new_password": 'new_password'
        }

**响应示例**

        { "message": "success"}

<a id="忘记密码"></a>
### 忘记密码
接口描述: &nbsp; 忘记密码
接口地址: &nbsp; /users/{id}/actions/forget-password/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
email             | String | 是   |  无    | 公司邮箱

**返回内容**

属性        | 类型   | 说明
------------|--------|------------------
message     | String | 'success' - 成功

<a id="角色"></a>
## 角色
<a id="获取角色列表"></a>
### 获取角色列表
接口描述: &nbsp; 获取角色列表
接口地址: &nbsp; /roles/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 角色名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Role object](#role-object)

**请求示例**
    
        GET /roles/
  
**响应示例**

        {
            'count': 100,
            'next': '/roles/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'name': 'role a',
                  'creator': 'admin',
                 },
                 {'id': 2, 
                  'name': 'role-b',
                  'creator': 'admin'
                 },
                  ...
             ]
        }

<a id="更新角色信息"></a>
### 更新角色信息
接口描述: &nbsp; 获取角色列表
接口地址: &nbsp; /roles/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 角色名

**返回内容**
[role object](#role-object)

**请求示例**
    
        GET /roles/{id}/users/
        ContentType: 'application/json'
        {'name': 'role a'}
  
**响应示例**

        {
            'id': 1, 
            'name': 'role a',
            'creator': 'admin',
        }

<a id="获取角色用户列表"></a>
### 获取角色用户列表
接口描述: &nbsp; 获取角色用户列表
接口地址: &nbsp; /roles/{id}/users/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
Array of [role object](#role-object)

        [
             {'id': 1, 
              'username': 'user-a',
              'email': 'user-a@example.com',
              'phone': '12345678901'},
             {'id': 2, 
              'name': 'user-b',
              'username': 'user-b@weimob.com',
              'phone': '12345678902'},
              ...
              
        ]

<a id="添加用户"></a>
### 添加用户
接口描述: &nbsp; 添加用户
接口地址: &nbsp; /roles/{id}/users/
请求方法: &nbsp; POST

**请求参数**
> Array of bellow object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
id                | Number | 是   |  无    | 用户id

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        POST /roles/{id}/users/
        CopntentType: 'application/json'
        [
            {'id': 1},
            {'id': 2},
            ...
        ]

**响应示例**

        {
            "message": "success"
        }

<a id="移除用户"></a>
### 移除用户
接口描述: &nbsp; 移除用户
接口地址: &nbsp; /roles/{id}/users/
请求方法: &nbsp; DELETE

**请求参数**
> Array of bellow object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
id                | Number | 是   |  无    | 用户id

**请求示例**

        DELETE /roles/{id}/users/
        CopntentType: 'application/json'
        [
            {'id': 1},
            {'id': 2},
            ...
        ]

**响应示例**

        {
            "message": "success"
        }

<a id="删除角色"></a>
### 删除角色
接口描述: &nbsp; 删除角色
接口地址: &nbsp; /roles/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**

        DELETE /roles/{id}/
   
**响应示例**

        { "message": "success"}

<a id="系统授权"></a>
## 系统授权
<a id="资源权限"></a>
### 资源权限
<a id="用户应用授权"></a>
####  用户应用授权
接口描述: &nbsp; 用户应用授权
接口地址: &nbsp; /users/{id}/application/perms/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
authorizations    | Array  | 否   |  无    | Array of [Application authorization entry](#application-authorization-entry)

<a id="application-authorization-entry"></a>

**application authorization entry**

属性          | 类型   |   说明
--------------|--------|-----------
id            | Number | 应用ID
app_name      | String | 应用名
permission    | Object | [Application permission object](#application-permission-object)

<a id="application-permission-object"></a>
**application permission object**
>true - 启用权限, false - 取消权限.

属性                   | 类型   |   说明
-----------------------|--------|-----------
view_app               | Bool   | 查看应用
edit_app               | Bool   | 编辑应用
delete_app             | Bool   | 删除应用
deploy_app             | Bool   | 新建,执行发布任务
review_app_deploy_task | Bool   | 审核发布任务
restart_app            | Bool   | 重启应用实例
view_app_log           | Bool   | 查看应用日志
view_app_monitor       | Bool   | 查看应用监控

**返回内容**

属性      | 类型   |   说明
----------|--------|-----------
message   | String | 'success' - 成功

**请求示例**

        POST /users/{id}/application/perms/
        ContentType: 'application/json'
        {
            'authorizations': [
                {
                  'id': 1,
                  'permission': {
                    'view_app': true,
                    'view_app_log': true,
                    'restart_app': true,
                  }
                },
                {
                  'id': 2,
                  'permissions': {
                    'view_app': true,
                    'view_app_log': true,
                    'restart_app': true,
                  }
                },
                ...
            ]
        }

**响应示例**

        {'message': 'success'}

<a id="角色应用授权"></a>
####  角色应用授权
接口描述: &nbsp; 角色应用授权
接口地址: &nbsp; /roles/{id}/application/perms/
请求方法: &nbsp; POST

> 参考 [用户应用授权](#用户应用授权)

<a id="获取用户应用权限"></a>
####  获取用户应用权限
接口描述: &nbsp; 获取用户应用权限
接口地址: &nbsp; /users/{id}/application/perms/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
app_name          | String | 否   |  无    | 应用名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Application authorization entry](#application-authorization-entry)

**请求示例**

        GET /users/{id}/application/perms/

**响应示例**

        {
            'count': 100,
            'next': '/users/{id}/application/perms/',
            'prev': null,
            'results': [{
                  'id': 1,
                  'app_name': 'test.app-a',
                  'permission': {
                    'view_app': true,
                    'view_app_log': true,
                    'restart_app': true,
                  }
                },
                {
                  'id': 2,
                  'app_name': 'test.app-b',
                  'permission': {
                    'view_app': true,
                    'view_app_log': true,
                    'restart_app': true,
                  }
                },
                ...
            ]
        }

<a id="获取角色应用权限"></a>
####  获取角色应用权限
接口描述: &nbsp; 获取角色应用权限
接口地址: &nbsp; /roles/{id}/application/perms/
请求方法: &nbsp; GET 

> 参考 [获取用户应用权限](#获取用户应用权限)

<a id="用户主机授权"></a>
####  用户主机授权
接口描述: &nbsp; 用户主机授权
接口地址: &nbsp; /users/id}/host/perms/
请求方法: &nbsp; POST


**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
authorizations    | Array  | 否   |  无    | Array of [host authorization entry](#host-authorization-entry)

<a id="application-authorization-entry"></a>

**host authorization entry**

属性          | 类型   |   说明
--------------|--------|-----------
id            | Number | 主机id
hostname      | String | 主机名
permission    | Object | [host permission object](#host-permission-object)

<a id="host-permission-object"></a>
**host permission object**
>true - 启用权限, false - 取消权限.

属性                   | 类型   |   说明
-----------------------|--------|-----------
view_host              | Bool   | 查看主机
edit_host              | Bool   | 编辑主机
delete_host            | Bool   | 删除主机
init_host              | Bool   | 初始化主机
restart_host           | Bool   | 重启主机
login_host             | Bool   | 登录主机
deactivate_host        | Bool   | 下架主机


**返回内容**

属性      | 类型   |   说明
----------|--------|-----------
message   | String | 'success' - 成功

**请求示例**

        POST /users/{id}/application/perms/
        ContentType: 'application/json'
        {
            'authorizations': [
                {
                  'id': 1,
                  'permission': {
                    'view_host': true,
                    'edit_host': true,
                    'delete_host': true,
                    'login_host': true,
                  }
                },
                {
                  'id': 2,
                  'permission': {
                    'view_host': true,
                    'edit_host': false,
                    'delete_host': false,
                    'login_host': true,
                  }
                },
                ...
            ]
        }

**响应示例**

        {'message': 'success'}

<a id="角色主机授权"></a>
####  角色主机授权
接口描述: &nbsp; 角色主机授权
接口地址: &nbsp; /roles/id}/host/perms/
请求方法: &nbsp; POST

>参考 [用户主机授权](#用户主机授权)

<a id="获取用户主机权限"></a>
####  获取用户主机权限
接口描述: &nbsp; 获取用户主机权限
接口地址: &nbsp; /users/{id}/host/perms/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
hostname          | String | 否   |  无    | 主机名

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [host authorization entry](#host-authorization-entry)

**请求示例**

        GET /users/{id}/host/perms/

**响应示例**

        {
            'count': 100,
            'next': '/users/{id}/application/perms/',
            'prev': null,
            'results': [
                 {
                  'id': 1,
                  'hostname': 'server-a',
                  'permission': {
                    'view_host': true,
                    'edit_host': true,
                    'delete_host': true,
                    'login_host': true,
                  }
                },
                {
                  'id': 2,
                  'hostname': 'server-b',
                  'permission': {
                    'view_host': true,
                    'edit_host': false,
                    'delete_host': false,
                    'login_host': true,
                  }
                },
                ...
            ]
        }

<a id="获取角色主机权限"></a>
####  获取角色主机权限
接口描述: &nbsp; 获取角色主机权限
接口地址: &nbsp; /roles/{id}/host/perms/
请求方法: &nbsp; GET

>参考 [获取角色主机权限](#获取角色主机权限)

<a id="获取应用用户授权"></a>
#### 获取应用用户授权

接口描述: &nbsp; 获取应用用户授权
接口地址: &nbsp; /applications/{id}/authorization/users/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性        | 类型   |   说明
------------|--------|-----------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Number |　Array of [User app authorization](#user-app-authorization)

<a id='user-app-authorization'></a>
**user app authorization**

属性          | 类型   |   说明
--------------|--------|-----------
user          | String | [User object](#user-object)
permission    | Object | [Application permission object](#application-permission-object)

**请求示例**

        GET /applications/{id}/authorization/users/

**响应示例**

        {
            'next': '/applications/{id}/authorization/users/?page=2'
            'prev': null
            'count': 100,
            'results': [
                 {'user': {'id': 4, 'username': 'user-a'},
                  'permission': {
                        'view_app': true,
                        'view_app_log': true,
                        'restart_app': true,
                        }
                 },
                 {'user': {'id': 5, 'username': 'user-b'},
                  'permission': {
                        'view_app': true,
                        'view_app_log': true,
                        'restart_app': false,
                        }
                 },
                 ...
            ]
        }

<a id="更新应用用户授权"></a>
#### 更新应用用户授权
接口描述: &nbsp; 更新应用用户授权
接口地址: &nbsp; /applications/{id}/authorization/users/
请求方法: &nbsp; PATCH

**请求参数**
> Array of below object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
user              | Object | 是   |  无    | [User object](#user-object)
permission        | Object | 否   |  无    | [Application permission object](#application-permission-object)
action            | String | 是   | update | 可选值['update', 'delete']

**请求示例**
    
         PATCH /applications/{id}/authorization/users/
         ContentType: 'application/json'
         [
            {
                'user': {'id': 1},
                'permission': {
                    'edit_app': false,
                },
                'action': 'update',
            },
            {
                'user': {'id': 2},
                'action': 'delete',
            },
            ...
         ]

**响应示例**

         {'message': 'success'}


<a id="获取应用角色授权"></a>
#### 获取应用角色授权

接口描述: &nbsp; 获取应用用户授权
接口地址: &nbsp; /applications/{id}/authorization/roles/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性        | 类型   |   说明
------------|--------|-----------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Number |　Array of [Role app authorization](#role-app-authorization)

<a id='role-app-authorization'></a>
**role app authorization**

属性          | 类型   |   说明
--------------|--------|-----------
role          | String | [Role object](#role-object)
permission    | Object | [Application permission object](#application-permission-object)

**请求示例**

        GET /applications/{id}/authorization/roles/

**响应示例**

        {
            'next': '/applications/{id}/authorization/roles/?page=2'
            'prev': null
            'count': 100,
            'results': [
                 {'user': {'id': 4, 'username': 'user-a'},
                  'permission': {
                        'view_app': true,
                        'view_app_log': true,
                        'restart_app': true,
                        }
                 },
                 {'user': {'id': 5, 'username': 'user-b'},
                  'permission': {
                        'view_app': true,
                        'view_app_log': true,
                        'restart_app': false,
                        }
                 },
                 ...
            ]
        }

**更新应用角色授权**

接口描述: &nbsp; 更新应用角色授权
接口地址: &nbsp; /applications/{id}/authorization/roles/
请求方法: &nbsp; PATCH

**请求参数**
> Array of below object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
role              | Object | 是   |  无    | [Role object](#role-object)
permission        | Object | 否   |  无    | [Application permission object](#application-permission-object)
action            | String | 是   | update | 可选值['update', 'delete']

**请求示例**
    
         PATCH /applications/{id}/authorization/roles/
         ContentType: 'application/json'
         [
            {
                'role': {'id': 1},
                'permission': {
                    'edit_app': false,
                },
                'action': 'update',
            },
            {
                'role': {'id': 2},
                'action': 'delete',
            },
            ...
         ]

**响应示例**

         {'message': 'success'}

<a id="获取主机用户授权"></a>
#### 获取主机用户授权

接口描述: &nbsp; 获取主机用户授权
接口地址: &nbsp; /hosts/{id}/authorization/users/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性        | 类型   |   说明
------------|--------|-----------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Number |　Array of [User host authorization](#user-host-authorization)

<a id='user-host-authorization'></a>
**user host authorization**

属性          | 类型   |   说明
--------------|--------|-----------
user          | String | [User object](#user-object)
permission    | Object | [Host permission object](#host-permission-object)

**请求示例**

        GET /hosts/{id}/authorization/users/

**响应示例**

        {
            'next': '/hosts/{id}/authorization/users/?page=2'
            'prev': null
            'count': 100,
            'results': [
                 {'user': {'id': 4, 'username': 'user-a'},
                  'permission': {
                        'view_host': true,
                        'edit_host': true,
                        'delete_host': true,
                        'login_host': true,    
                        }
                 },
                 {'user': {'id': 5, 'username': 'user-b'},
                  'permission': {
                        'view_host': true,
                        'edit_host': true,
                        'delete_host': true,
                        'login_host': true,
                        }
                 },
                 ...
            ]
        }

<a id="更新主机用户授权"></a>
#### 更新主机用户授权
接口描述: &nbsp; 更新主机用户授权
接口地址: &nbsp; /applications/{id}/authorization/users/
请求方法: &nbsp; PATCH

**请求参数**
> Array of below object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
user              | Object | 是   |  无    | [User object](#user-object)
permission        | Object | 否   |  无    | [Host permission object](#host-permission-object)
action            | String | 是   | update | 可选值['update', 'delete']

**请求示例**
    
         PATCH /applications/{id}/authorization/users/
         ContentType: 'application/json'
         [
            {
                'user': {'id': 1},
                'permission': {
                    'edit_host': false,
                },
                'action': 'update',
            },
            {
                'user': {'id': 2},
                'action': 'delete',
            },
            ...
         ]

**响应示例**

         {'message': 'success'}

<a id="获取主机角色授权"></a>
#### 获取主机角色授权

接口描述: &nbsp; 获取主机角色授权
接口地址: &nbsp; /host/{id}/authorization/roles/
请求方法: &nbsp; GET

**请求参数**
>参考 [公共请求参数](#公共请求参数)

**返回内容**

属性        | 类型   |   说明
------------|--------|-----------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Number |　Array of [Role host authorization](#role-host-authorization)

<a id='role-host-authorization'></a>
**role host authorization**

属性          | 类型   |   说明
--------------|--------|-----------
role          | String | [Role object](#role-object)
permission    | Object | [Host permission object](#host-permission-object)

**请求示例**

        GET /hosts/{id}/authorization/roles/

**响应示例**

        {
            'next': '/hosts/{id}/authorization/roles/?page=2'
            'prev': null
            'count': 100,
            'results': [
                 {'role': {'id': 4, 'name': 'role-a'},
                  'permission': {
                        'view_host': true,
                        'edit_host': true,
                        'delete_host': true,
                        'login_host': true,    
                        }
                 },
                 {'role': {'id': 5, 'name': 'role-b'},
                  'permission': {
                        'view_host': true,
                        'edit_host': true,
                        'delete_host': true,
                        'login_host': true,
                        }
                 },
                 ...
            ]
    }

<a id="更新主机角色授权"></a>
#### 更新主机角色授权
接口描述: &nbsp; 更新主机角色授权
接口地址: &nbsp; /applications/{id}/authorization/roles/
请求方法: &nbsp; PATCH

**请求参数**
> Array of below object

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
role              | Object | 是   |  无    | [Role object](#role-object)
permission        | Object | 否   |  无    | [Host permission object](#host-permission-object)
action            | String | 是   | update | 可选值['update', 'delete']

**请求示例**
    
         PATCH /applications/{id}/authorization/roles/
         ContentType: 'application/json'
         [
            {
                'role': {'id': 1},
                'permission': {
                    'edit_host': false,
                },
                'action': 'update',
            },
            {
                'role': {'id': 2},
                'action': 'delete',
            },
            ...
         ]

**响应示例**

        {'message': 'success'}
<a id="功能模块权限"></a>
### 功能模块权限                                                                                 
<a id="用户功能授权"></a>
#### 用户功能授权
接口描述: &nbsp; 用户功能授权
接口地址: &nbsp; /users/{id}/system/perms/
请求方法: &nbsp; POST

**请求参数**
> Array of bellow

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
module_name       | String | 是   | 无     |功能模块名称
permissions       | Object | 是   | 无     |[Module permission](#module-permission)

> 由于不同功能模块权限各不相同， module permission 对象将会根据module_name参数变化. 模块权限详情请参考 [模块权限](#模块权限)

<a id="模块权限"></a>
**模块权限**

- [资源申请权限](#mp_资源申请)
- [应用管理权限](#mp_应用管理)
- [DNS管理权限](#mp_DNS管理)
- [资源管理权限](#mp_资源管理)
- [导航管理权限](#mp_导航管理)
- [常用工具权限](#mp_常用工具)
- [发布模板权限](#mp_发布模板)

<a id='mp_资源申请'>资源申请权限</a>

属性                 |  类型  |　说明
---------------------|--------|----------
enable_resource_req  |  Bool  | 启用资源申请模块
approve_host_req     |  Bool  | 主机申请审批
approve_domain_req   |  Bool  | 域名申请审批
approve_ssl_cert_req |  Bool  | ssl证书审批
create_resource_req  |  Bool  | 新建资源申请

<a id='mp_应用管理'>应用管理权限</a>

属性                 |  类型  |　说明
---------------------|--------|----------
enable_app_mgmt      |  Bool  | 启用应用管理模块
view_app             |　Bool  | 查看所有应用
create_app           |  Bool  | 新建应用
delete_app           |  Bool  | 删除所有应用
edit_app             |  Bool  | 编辑所有应用

<a id='mp_DNS管理'>DNS管理权限</a>

属性                 |  类型  |　说明
---------------------|--------|----------
enable_dns_mgmt      |  Bool  | 启用DNS管理模块
manage_dns_server    |  Bool  | 管理DNS服务

<a id='mp_资源管理'>资源管理权限</a>

属性                   |  类型  |　说明
--------------------- -|--------|----------
enable_host_mgmt        |  Bool  | 启用主机管理模块
add_host               |  Bool  | 添加主机
edit_host              |  Bool  | 编辑任意主机配置
delete_host            |  Bool  | 删除任意主机
manage_host            |  Bool  | 管理任意主机
enable_business_mgmt   |  Bool  | 启用业务管理模块
view_business          |  Bool  | 查看任意业务线
add_business           |  Bool  | 新增业务线
delete_business        |  Bool  | 删除任意业务线

<a id='mp_导航管理'>导航管理权限</a>

属性                          |  类型  |　说明
------------------------------|--------|----------
enable_navigator              |  Bool  | 启用第三方导航模块
view_navigator                |  Bool  | 查看第三方导航
manage_navigator              |  Bool  | 管理第三方导航


<a id='mp_常用工具'>常用工具权限</a>

属性                          |  类型  |　说明
------------------------------|--------|----------
enable_common_tools           |  Bool  | 启用常用工具模块
enable_cdn_refresher          |  Bool  | 启用cdn刷新功能
enable_jumpserver_log_mgmt |  Bool  | 启用跳板机日志管理功能

<a id='mp_发布模板'>发布模板权限</a>

属性                          |  类型  |　说明
------------------------------|--------|----------
enable_deploy_template_mgmt   |  Bool  | 启用启用模块
enable_cdn_refresher          |  Bool  | 启用cdn刷新功能
enable_jumpserver_log_mgmt    |  Bool  | 启用跳板机日志管理功能


**正确返回**

属性        | 类型   | 说明
------------|--------|-------------
message     | String | success - 成功

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   400     | 未定义的权限
30002       |   400     | 没有授权权限

**请求示例**

        POST /users/{id}/system/perms/
        ContentType: 'application/json'
        {
            'module_name': 'application',
            'permissions': {
                'enable_app_mgmt': true,
                'add_app': true,
                'delte_app': true,
                'manage_app': true,
            }
        }

**正确响应示例**
   
        {'message': 'success'}

**错误响应示例**

        {'error_code': 30001, 'message': '未定义的权限 restart_app'}


<a id="角色功能授权"></a>
#### 角色功能授权
接口描述: &nbsp; 角色功能授权
接口地址: &nbsp; /roles/{id}/system/perms/
请求方法: &nbsp; POST

>参考 [用户功能授权](#用户功能授权)

<a id="第三方导航管理"></a>
## 第三方导航管理
<a id="获取导航列表"></a>
### 获取导航列表
接口描述: &nbsp; 获取导航列表
接口地址: &nbsp; /external-navigators/
请求方法: &nbsp; GET 

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | 导航名称

**返回内容**

属性        | 类型   | 说明
------------|--------|-------------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [External navigator object](#external-navigator-object)

**请求示例**
  
        GET /external-navigators/

**响应示例**
   
        {
            'count': 100,
            'next': '/external-navigators/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'name': 'external system a',
                  'img': '/imgs/externa-a.jpg'
                  'url': 'http://external-a.example.com/'
                  'creator': 'admin',
                 },
                 {
                  'id': 2, 
                  'name': 'external system b',
                  'img': '/imgs/externa-b.jpg'
                  'url': 'http://external-b.example.com/'
                  'creator': 'admin',
                 },
                  ...
             ]
        }

<a id="新建导航"></a>
### 新建导航
接口描述: &nbsp; 新建导航
接口地址: &nbsp; /external-navigators/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |   无   |导航名称
img               | String | 是   |   无   |导航图片路径
url               | String | 是   |   无   |导航地址

**返回内容**
[External navigator object](#external-navigator-object)

**请求示例**
    
        POST /external-navigators/
        ContentType: 'application/json'
        {
            'name': 'external system a',
            'img': '/imgs/externa-a.jpg'
            'url': 'http://external-a.example.com/'
        }

  
**响应示例**

        {
             'id': 1, 
             'name': 'external system a',
             'img': '/imgs/externa-a.jpg'
             'url': 'http://external-a.example.com/'
             'creator': 'admin',
        }

<a id="更新导航"></a>
### 更新导航
接口描述: &nbsp; 更新导航
接口地址: &nbsp; /external-navigators/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |   无   |导航名称
img               | String | 否   |   无   |导航图片路径
url               | String | 否   |   无   |导航地址

**返回内容**
[External navigator object](#external-navigator-object)

**请求示例**
    
        PATCH /external-navigators/
        ContentType: 'application/json'
        {
            'name': 'external system a',
            'img': '/imgs/externa-a.jpg'
            'url': 'http://external-a.example.com/'
        }

  
**响应示例**

        {
             'id': 1, 
             'name': 'external system a',
             'img': '/imgs/externa-a.jpg'
             'url': 'http://external-a.example.com/'
             'creator': 'admin',
        }

<a id="获取导航详情"></a>
### 获取导航详情
接口描述: &nbsp; 获取导航详情
接口地址: &nbsp; /external-navigators/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
[External navigator object](#external-navigator-object)

**请求示例**
    
        GET /external-navigators/{id}/
   

**响应示例**

        {
             'id': 1, 
             'name': 'external system a',
             'img': '/imgs/externa-a.jpg'
             'url': 'http://external-a.example.com/'
             'creator': 'admin',
        }

a id="获取导航详情"></a>
<a id="删除导航"></a>
### 删除导航
接口描述: &nbsp; 删除导航
接口地址: &nbsp; /external-navigators/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**
    
        DELETE /external-navigators/{id}
   

**响应示例**

        {'message': 'success'}

<a id="apiauthtokens"></a>
## APIAuthTokens

<a id="获取auth-token列表"></a>
### 获取auth token列表
接口描述: &nbsp; 获取auth token列表
接口地址: &nbsp; /auth-tokens/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | token 名
value             | String | 否   |  无    | token 值
description       | String | 否   |  无    | 描述信息

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Auth token](#auth-token-object)

**请求示例**
    
        GET /auth-tokens/

**响应示例**

        {
            'count': 100,
            'next': '/auth-tokens/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'name': 'role a',
                  'creator': 'admin',
                 },
                 {'id': 2, 
                  'name': 'role-b',
                  'creator': 'admin'
                 },
                  ...
             ]
        }

<a id="创建auth-token"></a>
### 创建auth token
接口描述: &nbsp; 创建auth token
接口地址: &nbsp; /auth-tokens/
请求方法: &nbsp; POST

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 是   |  无    | token 名
description       | String | 否   |  无    | 描述信息

**返回内容**
[Auth token](#auth-token-object)

**请求示例**
    
        POST /auth-tokens/
        ContentType: 'application/json'
        {
            'name': 'token a',
            'description': 'description of token'
        }

**响应示例**

        {
            'id':  1,
            'name': 'token a',
            'value': '9944b09199c62bcf9418ad846dd0e4bbdfc6ee4b',
            'description': 'description of token'
        }

<a id="更新auth-token"></a>
### 更新auth token
接口描述: &nbsp; 更新auth token
接口地址: &nbsp; /auth-tokens/{id}/
请求方法: &nbsp; PATCH

**请求参数**

参数名            | 类型   | 必选 | 默认值 |说明
------------------|--------|------|--------|-----------
name              | String | 否   |  无    | token 名
description       | String | 否   |  无    | 描述信息

**返回内容**
[Auth token](#auth-token-object)

**请求示例**
    
        PATCH /auth-tokens/
        ContentType: 'application/json'
        {
            'name': 'token a',
            'description': 'description of token'
        }

**响应示例**

        {
            'id':  1,
            'name': 'token a',
            'value': '9944b09199c62bcf9418ad846dd0e4bbdfc6ee4b',
            'description': 'description of token'
        }

<a id="获取auth-token详情"></a>
### 获取auth token详情
接口描述: &nbsp; 获取auth token详情
接口地址: &nbsp; /auth-tokens/{id}/
请求方法: &nbsp; GET

**请求参数**
    无

**返回内容**
[Auth token](#auth-token-object)

**请求示例**
    
        GET /auth-tokens/{id}/
  

**响应示例**

        {
            'id':  1,
            'name': 'token a',
            'value': '9944b09199c62bcf9418ad846dd0e4bbdfc6ee4b',
            'description': 'description of token'
        }

<a id="删除auth-token"></a>
### 删除auth token
接口描述: &nbsp; 删除auth token
接口地址: &nbsp; /auth-tokens/{id}/
请求方法: &nbsp; DELETE

**请求参数**
    无

**返回内容**

属性        | 类型   | 说明
------------|--------|---------
message     | String | 'success' - 成功

**请求示例**
        
        DELETE /auth-tokens/{id}/
   

**响应示例**

        {'message': 'success'}

<a id="常用工具"></a>
## 常用工具
<a id="跳板机日志查询"></a>
### 跳板机日志查询
接口描述: &nbsp; 跳板机日志查询
接口地址: &nbsp; /common-utils/jump-server-logs/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名     | 类型   | 必选 | 默认值 |说明
-----------|--------|------|--------|-----------
keyword    | String | 否   |  无    | 查询关键字
user       | String | 否   |  无    | 操作用户
host       | String | 否   |  无    | 操作主机
time__gt   | String | 否   |  无    | 操作时间大于等于
time__lt   | String | 否   |  无    | 操作时间小于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [Jump server log ](#jump-server-log)

**请求示例**
        
        GET /common-utils/jump-server-log/

**响应示例**

        {
            'count': 100,
            'next': '/common-utils/jump-server-log/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'user': 'admin',
                  'host': 'host-a',
                  'created_time': '2018-04-18T15:38:40+08:00', 
                  'text': 'some operation text'
                 },
                  ...
             ]
        }
<a id="cdn刷新"></a>
### CDN刷新

<a id="获取cdn刷新任务列表"></a>
#### 获取CDN刷新任务列表
接口描述: &nbsp; 获取CDN刷新任务列表
接口地址: &nbsp; /common-utils/cdn-refresh-tasks/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名               | 类型   | 必选 | 默认值 |说明
---------------------|--------|------|--------|-----------
cdn_service_provider | String | 否   |  无    | cdn厂商
creator              | String | 否   |  无    | 创建人
created_time__gt     | String | 否   |  无    | 创建时间大于等于
created_time__lt     | String | 否   |  无    | 创建时间小于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [cdn refresh task](#cdn-refresh-task)

**请求示例**
    
        GET /common-utils/cdn-refresh-tasks/

**响应示例**

        {
            'count': 100,
            'next': '/common-utils/cdn-refresh-tasks/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'urls': ['http://url-a.example.com', 'http://url-a.example.com'],
                  'cdn_service_provider': 'wangsu',
                  'refresh_mode': 'recursive',
                  'creator': 'admin',
                  'status': 'finished',
                  'created_time': '2018-04-18T15:38:40+08:00', 
                  'finished_time': ' 2018-04-18T15:40:40+08:00',
                 },
                 {
                    'id': 2, 
                    'urls': ['http://url-c.example.com', 'http://url-d.example.com'],
                    'cdn_service_provider': 'tecent',
                    'refresh_mode': 'single_file',
                    'creator': 'admin',
                    'status': 'failed',
                    'error': 'call service api failed',
                    'created_time': '2018-04-18T15:38:40+08:00', 
                    'finished_time': null,
                 },
                  ...
             ]
        }

<a id="新建cdn刷新任务"></a>
#### 新建CDN刷新任务
接口描述: &nbsp; 新建CDN刷新任务
接口地址: &nbsp; /common-utils/cdn-refresh-tasks/
请求方法: &nbsp; POST

**请求参数**

参数名               | 类型   | 必选 | 默认值 |说明
---------------------|--------|------|--------|-----------
cdn_service_provider | String | 是   |  无    | cdn厂商
refresh_mode         | String | 是   |  无    | 刷新模式, recursive - 递归刷新 single_file - 单文件刷新
urls                 | Array  | 是   |  无    | Array of url

**正确返回**

[cdn refresdh task](#cdn-refresh-task)

**错误返回**

属性        | 类型   | 说明
------------|--------|---------
error_code  | Number | 错误码
message     | String | 错误信息

**错误码**

错误码      |http状态码 |说明
------------|-----------|---------
30001       |   400     | url不能为空
30002       |   400     | 非法的url域名
30003       |   400     | 刷新模式不支持
30004       |   400     | CDN厂商不支持

**请求示例**
    
        POST /common-utils/cdn-refresh-tasks/
        ContentType: 'application/json'
        {
          'urls': ['http://url-a.example.com', 'http://url-a.example.com'],
          'cdn_service_provider': 'wangsu',
          'refresh_mode': 'recursive',
        }

**响应示例**


        {
          'id': 1, 
          'urls': ['http://url-a.example.com', 'http://url-a.example.com'],
          'cdn_service_provider': 'wangsu',
          'refresh_mode': 'recursive',
          'creator': 'admin',
          'status': 'processing',
          'created_time': '2018-04-18T15:38:40+08:00', 
        }
             


<a id="操作审计"></a>
## 操作审计
<a id="获取dns操作记录"></a>
### 获取DNS操作记录
接口描述: &nbsp; 获取DNS操作记录
接口地址: &nbsp; /audit/dns-operations/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名                | 类型   | 必选 | 默认值 |说明
--------------------- |--------|------|--------|-----------
operator              | String | 否   |  无    | 操作人
op_type               | String | 否   |  无    | 操作类型，可选值['add', 'update', 'delete', 'disable', 'enable']
op_target             | String | 否   |  无    | 操作对象类型, 可选值['server', ['domain', 'record']]
op_detail             | String | 否   |  无    | 操作消息
op_time__lt           | String | 否   |  无    | 操作时间小于等于
op_time__gt           | String | 否   |  无    | 操作时间大于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [dns operation](#dns-operation)

**请求示例**
    
        GET /audit/dns-operations/

**响应示例**

        {
            'count': 100,
            'next': '/audit/dns-operations/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'op_target': 'domain',
                  'op_type': 'add',
                  'op_detail': '新增域名 example.com',
                  'op_time': '2018-04-18T15:38:40+08:00', 
                  'operator': 'admin',
                 },
                 {
                  'id': 2, 
                  'op_target': 'record',
                  'op_type': 'delete',
                  'op_detail': '删除域名记录 record-a.example.com',
                  'op_time': '2018-04-18T15:38:40+08:00', 
                  'operator': 'admin',
                 },
                ...
             ]
        }
<a id="获取主机操作记录"></a>
### 获取主机操作记录
接口描述: &nbsp; 获取主机操作记录
接口地址: &nbsp; /audit/host-operations/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名               | 类型   | 必选 | 默认值 |说明
---------------------|--------|------|--------|-----------
operator             | String | 否   |  无    | 操作人
op_type              | String | 否   |  无    | 操作类型，可选值['add', 'update', 'delete', 'attach_app', 'deatach_app']
hostname             |  Strig | 否   |  无    | 主机名
op_detail            | String | 否   |  无    | 操作详情
op_time__lt          | String | 否   |  无    | 操作时间小于等于
op_time__gt          | String | 否   |  无    | 操作时间大于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [host operation](#host-operation)

**请求示例**
    
        GET /audit/host-operations/

**响应示例**

        {
            'count': 100,
            'next': '/audit/host-operations/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'hostname': 'server-a',
                  'op_type': 'add',
                  'operator': 'admin',
                  'op_detail': '新增主机 server-a',
                  'op_time': '2018-04-18T15:38:40+08:00', 
                 },
                 {
                  'id': 2, 
                  'hostname: 'server-b'
                  'op_type': 'delete',
                  'operator': 'admin',
                  'op_detail': '删除主机server-b',
                  'op_time': '2018-04-18T15:38:40+08:00', 
                 },
                ...
             ]
        }
<a id="获取应用操作记录"></a>
### 获取应用操作记录

接口描述: &nbsp; 获取应用操作记录
接口地址: &nbsp; /audit/app-operations/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名               | 类型   | 必选 | 默认值 |说明
---------------------|--------|------|--------|-----------
operator             | String | 否   |  无    | 操作人
app_name             | String | 否   |  无    | 应用名
op_type              | String | 否   |  无    | 操作类型，可选值['add', 'update', 'delete', 'attach_host', 'deatach_host', 'change_deploy_setting']
op_detail            | String | 否   |  无    | 操作详情
op_time__lt          | String | 否   |  无    | 操作时间小于等于
op_time__gt          | String | 否   |  无    | 操作时间大于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [app operation](#app-operation)

**请求示例**
    
        GET /audit/app-operations/

**响应示例**

        {
            'count': 100,
            'next': '/audit/app-operations/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'app_name': 'test.app-a',
                  'op_type': 'add',
                  'operator': 'admin',
                  'op_detail': '新增应用 test.app-a',
                  'op_time': '2018-04-18T15:38:40+08:00', 
                 },
                 {
                  'id': 2, 
                  'app_name': 'test.app-a',
                  'op_type': 'change_deploy_settings',
                  'operator': 'admin',
                  'op_detail': "更新应用发布配置 respository url,
                                变更前: http://test.example.com/my-repo/, 
                                变更后: 'http://test.example.com/new-repo'",
                  'op_time': '2018-04-18T15:38:40+08:00', , 
                 },
                ...
             ]
    }
<a id="获取授权操作记录"></a>
### 获取授权操作记录

<a id="获取模块授权操作记录"></a>
#### 获取模块授权操作记录
接口描述: &nbsp; 获取模块授权操作记录
接口地址: &nbsp; /audit/authorize-operations/modules/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名                  | 类型   | 必选 | 默认值 |说明
---------------------   |--------|------|--------|-----------
operator                | String | 否   |  无    | 操作人
module_name             | String | 否   |  无    | 被授权模块名
perm_name               | String | 否   |  无    | 权限名
action                  | String | 否   |  无    | 授权动作类型 ['enable', 'disable'] 
authorized_target_type  | String | 否   |　无　　| 获得授权的目标类型，可选值 ['role', 'user']
authorized_target_name  | String | 否   |  无    | 获得授权的用户或角色名
op_time__lt             | String | 否   |  无    | 操作时间小于等于
op_time__gt             | String | 否   |  无    | 操作时间大于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [module authorized operation](#module-authorized-operation)

**请求示例**
    
        GET /audit/authorize-operations/modules/

**响应示例**

        {
            'count': 100,
            'next': '/audit/authorize-operations/modules/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1, 
                  'operator': 'admin',
                  'module_name': '应用管理',
                  'perm_name': 'add_app',
                  'action': 'enable',
                  'authorized_target_type': 'role',
                  'authorized_target_name': '运维人员',
                  'op_time': '2018-04-18T15:38:40+08:00', ,
                 },
                 {
                  'id': 2, 
                  'operator': 'admin',
                  'module_name': '应用管理',
                  'perm_name': 'add_app',
                  'action': 'disable',
                  'authorized_target_type': 'role',
                  'authorized_target_name': '开发人员',
                  'op_time': '2018-04-18T15:38:40+08:00', , 
                 },
                ...
             ]
        }

<a id="获取资源授权操作记录"></a>
#### 获取资源授权操作记录
接口描述: &nbsp; 获取资源授权操作记录
接口地址: &nbsp; /audit/authorize-operations/resources/
请求方法: &nbsp; GET

**请求参数**
>其他参数参考 [公共请求参数](#公共请求参数)

参数名                  | 类型   | 必选 | 默认值 |说明
---------------------   |--------|------|--------|-----------
operator                | String | 否   |  无    | 操作人
resource_type           | String | 否   |  无    | 被授权资源类型, 可选值['host', 'application', 'business']
resource_id             | Number | 否   |  无    | 被授权资源id
perm_name               | String | 否   |  无    | 权限名
action                  | String | 否   |  无    | 授权动作类型 ['enable', 'disable'] 
authorized_target_type  | String | 否   |　无　　| 获得授权的目标类型，可选值 ['role', 'user']
authorized_target_name  | String | 否   |  无    | 获得授权的用户或角色名
op_time__lt             | String | 否   |  无    | 操作时间小于等于
op_time__gt             | String | 否   |  无    | 操作时间大于等于


**返回内容**

属性        | 类型   | 说明
------------|--------|---------
prev        | String | 上一页链接
next        | String | 下一页链接
count       | Number | 总条数
results     | Array  | Array of [resource authorized operation](#resource-authorized-operation)

**请求示例**
    
        GET /audit/authorize-operations/resources/

**响应示例**

        {
            'count': 100,
            'next': '/audit/authorize-operations/resources/?page=2',
            'prev': null,
            'results': [
                 {
                  'id': 1,
                  'operator': 'admin',
                  'resource_type': 'host',
                  'resource': {'id': 1, 'host': 'server-a'},
                  'perm_name': 'login',
                  'action': 'enable',
                  'authorized_target_type': 'role',
                  'authorized_target_name': '运维人员',
                  'op_time': '2018-04-18T15:38:40+08:00',
                 },
                 {
                  'id': 1,
                  'operator': 'admin',
                  'resource_type': 'host',
                  'resource': {'id': 2, 'host': 'server-b'},
                  'perm_name': 'login',
                  'action': 'enable',
                  'authorized_target_type': 'role',
                  'authorized_target_name': '运维人员',
                  'op_time': '2018-04-18T15:38:40+08:00',
                 },
                ...
             ]
    }
<a id="apitoken操作"></a>
### APItoken操作


<a id="数据类型"></a>
# 数据类型

<a id="production-object"></a>
##Production Object

属性       | 类型   | 说明
-----------|--------|-------
id         | Number | 产品线id
name       | String | 产品线名称
description| String | 描述
available_actions | [Available production actions](#available-prod-actions) object | 可用操作

<a id="application-object"></a>
##Application Object

属性       | 类型   | 说明
-----------|--------|-------
id         | Number | 应用id
name       | String | 应用名
full_name  | String | 绝对名称(包含路径信息)
has_child  | String | 是否含有子应用
production | Number | 产品id
parent_app | Number &#124; Null | 父应用ID，若为NULL则没有父应用
available_actions | [Available app actions](#avail-app-actions) object | 可用操作

<a id="avail-app-actions"></a>
###  avail app actions

属性                   | 类型   |   说明
-----------------------|--------|-----------
view_app               | Bool   | 查看应用
edit_app               | Bool   | 编辑应用
delete_app             | Bool   | 删除应用
deploy_app             | Bool   | 新建,执行发布任务
review_app_deploy_task | Bool   | 审核发布任务
restart_app            | Bool   | 重启应用实例
view_app_log           | Bool   | 查看应用日志
view_app_monitor       | Bool   | 查看应用监控

<a id="available-prod-actions"></a>
###Available prod actions

属性              | 类型  | 说明
------------------|-------|------
view              | Bool  | 查看
delete            | Bool  | 删除
reboot            | Bool  | 编辑

<a id="application-deploy-template"></a>
### Application deploy template

属性          | 类型   | 说明
--------------|--------|---------
id            | Number | 模板id
enabled       | Bool   | 是否启用
applications  | Number | 关联应用id列表
repository    | Object | 应用源码仓库,  可能的类型为<ul><li>[ftp repo](#ftp-repository) </li><li>[git repo](#git-repository)</li></ul>
deploy_path   | String | 发布路径
timeout       | Number | 发布任务执行超时时间
keep_backups  | Number | 保留最近备份数
lifecyle_hooks| Array  | Array of [deploy task lifecyle hooks](#deploy-task-lifecycle-hooks)

<a id="deploy-settings"></a>
##Deploy Settings

<a id="application-deploy-settings"></a>
### Application Deploy Settings

属性          | 类型   | 说明
------------  |--------|---------
enabled       | Bool   | 是否启用
creator       | String | 创建人
application   | Number | 应用Id
repository    | Object | 应用源码仓库, 可能的类型为<ul><li>[ftp repo](#ftp-repository) </li><li>[git repo](#git-repository)</li></ul>
deploy_path   | String | 发布路径
timeout       | Number | 发布任务执行超时时间
keep_backups  | Number | 保留最近备份数
lifecyle_hooks| Array  | Array of [deploy task lifecyle hooks](#deploy-task-lifecycle-hooks)
template      | Object | 发布配置链接模板id

<a id="deploy-task-lifecycle-hooks"></a>
### deploy task lifecycle hooks

属性            | 类型   | 说明
----------------|--------|---------
running_user    | String | 脚本默认执行用户，在lifecye hook 里配置的running_  user将会覆盖此配置.
global_pre_exec | Object | [lifecycle-hook](#lifecycle-hook)
pre_exec        | Object | [lifecycle-hook](#lifecycle-hook)
post_exec       | Object | [lifecycle-hook](#lifecycle-hook)
global_post_exec| Object | [lifecycle-hook](#lifecycle-hook)

<a id="lifecycle-hook"></a>
#### lifecycle hook

属性          | 类型   | 说明
------------  |--------|---------
running_user  | String | 脚本执行用户
script        | Object | [deploy script](#deploy-script)

<a id="deploy-script"></a>
###Deploy script 

属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | String | Script Template Id
name                    | String | 脚本名称
language                | String | 脚本语言, 可选值['python', 'bash']
content                 | String | 脚本内容
template_engine         | String | 脚本渲染引擎


<a id="ftp-repository"></a>
###FTP repository

属性                    | 类型   | 说明
----------------------- |--------|---------
type                    | String | 仓库类型 值为 'FTP'
url                     | String | ftp url
credential              | Object | [Password Credential](#app_deploy_password_credential)
 
<a id="git-repository"></a>
###GIT repository

属性                    | 类型   | 说明
----------------------- |--------|---------
type                    | String | 仓库类型 值为 'GIT'
url                     | String | git url
branch                  | String | git 仓库分支
credential              | Object | [Password Credential](#app_deploy_password_credential)

<div id="app_deploy_password_credential"></div>
<a id="password-credential"></a>
###Password credential

属性                    | 类型   | 说明
----------------------- |--------|---------
type                    | String | 凭据类型，值为'PASSWORD'
username                | String | 用户名
password                | String | 密码

<a id="ssh-private-key-credential"></a>
###SSH private key credential

属性                    | 类型   | 说明
----------------------- |--------|---------
type                    | String | 凭据类型，值为'SSH_PRIVATE_KEY'
username                | String | 用户名
private_key             | String | 私钥内容

<div id="app_deploy_ssh_private_key_credential"></div>

<a id="host-object"></a>
## Host object
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 主机id
name                    | String | 主机名
host_type               | String | 主机类型,可选值:<br>   &nbsp;ALI_ECS - 阿里云<br> &nbsp;PHY_HOST - 物理机<br> &nbsp;TECENT_CVM - 腾讯云主机<br>&nbsp;TECENT_CPM - 腾讯云黑石物理机 <br> &nbsp;CLOUDSTACK - 线上cloudstack集群 <br> &nbsp;CLOUDSTACK_OFFICE - 线下CLOUDSTACK集群
status                  | String | 主机状态, 可选值: &nbsp; ['attached', 'inited', 'raw', 'offline']
os_status               | String | 操作系统状态，可选值: &nbsp; ['stopped', 'running', 'restarting']
os_type                 | String | 操作系统版本
cpu                     | Number | cpu 核心数
memory                  | Number | 内存大小， 单位MB
location                | String | 地理位置
ip_adress               | Array  | Arrary of [Ip Address Object](#ip-address-object)
description             | String | 描述信息

<a id="host-init-task"></a>
### Host init task
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 初始化任务id
hosts                   | Array  | Array of [Host](#host-object)
created_time            | String | 创建时间
opts                    | Object | [Host init task options](#host-init-task-options)
finished_time           | String | 结束时间
status                  | String | 当前状态， 可选值: ['running', 'failed', 'finished']
creator                 | String | 任务发起人

<a id="host-init-task-options"></a>
#### Host init task options
属性                    | 类型   | 说明
----------------------- |--------|---------
zabbix_groups           | Array  | zabbix监控主机组
zabbix_temlates         | Array  | zabbix监控模板

<a id="host-start-task"></a>
### Host start task
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 任务id
hosts                   | Array  | Array of [Host](#host-object)
creator                 | String | 发起人
created_time            | String | 创建时间
finished_time           | String | 完成时间
status                  | String | 状态， 可选值['running', 'failed', 'finished']

<a id="host-stop-task"></a>
### Host stop task
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 任务id
hosts                   | Array  | Array of [Host](#host-object)
creator                 | String | 发起人
created_time            | String | 创建时间
finished_time           | String | 完成时间
status                  | String | 状态， 可选值['running', 'failed', 'finished']

<a id="host-restart-task"></a>
### Host restart task
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 任务id
hosts                   | Array  | Array of [Host](#host-object)
creator                 | String | 发起人
created_time            | String | 创建时间
finished_time           | String | 完成时间
status                  | String | 状态， 可选值['running', 'failed', 'finished']


<a id="resource-request"></a>
## Resource Request

<a id="domain-request"></a>
### Domain request

属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 申请单ID
creator                 | String | 创建人
status                  | String | 申请单状态，可能值为['approved', 'wait_review', 'rejected', 'closed', 'finished']
created_time            | String | 创建时间
associated_app          | Number | 域名相关application id
records                 | Array  | Array of [dns record](#requested-dns-record)

<a id="requested-dns-record"></a>
#### requested dns record
属性                    | 类型   | 说明
----------------------- |--------|---------
name                    | String | 记录名
value                   | String | 记录值 
type                    | String | 记录类型, 可能值为['A', 'MX', 'CNAME'，'NS']

<a id="host-request"></a>
### Host request

属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 申请单ID
creator                 | String | 创建人
status                  | String | 申请单状态，可能值为['approved', 'wait_review', 'rejected', 'closed', 'finished']
created_time            | String | 创建时间
purpose                 | String | 用途
expect_delivery_days    | String | 期望交付天数
expiration_type         | String | 可选值['INFINITE', 'FINITE']
expiration_days         | String | 使用天数
users_with_log_perm     | Array  | Array of [User](#user-object)
shipped_packages        | Array  | Array of [Shipped Package](#shipped-package)
requested_hosts         | Array  | Array of [Requested Host](#requested-host)

<a id="requested-host"></a>
#### Requested Host
属性                    | 类型   | 说明
----------------------- |--------|---------
name                    | String | 主机名
cpu_cores               | Number | cpu 核心数
mem                     | Number | 内存大小，单位MB.
storage                 | Number | 存储大小，单位MB

<a id="shipped-package"></a>
####Shipped package
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | package id
name                    | String | package 名称
type                    | String | 包类型 - ['zip', 'tar.gz', 'rpm']
maintainer              | String | 维护人
craeted_time            | String | 创建时间
update_time             | String | 更新时间
description             | String | 描述

<a id="ssl-certificate-request"></a>
### ssl certificate request
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | 申请单ID
creator                 | String | 创建人
status                  | String | 申请单状态，可能值为['approved', 'wait_review', 'rejected', 'closed', 'finished']
created_time            | String | 创建时间
purpose                 | String | 用途
expect_delivery_days    | String | 期望交付天数
domian                  | String | 证书域名z
certificate_type        | String | 证书类型，可选值 ['wizard', 'normal'] <br> <ul><li>wizard - 通配符类型</li><li>normal - 普通类型</li></ul>

<a id="dns"></a>
## DNS
<a id="dns-server"></a>
###  dns server
属性              | 类型   |说明
------------------|--------|-----------
id                | Number | 服务器id
creator           | String | 创建人
created_time      | String | 创建时间
name              | String | 服务器名称
type              | String | 可选值 ['bind', 'powerdns']
api_endpoint      | String | dns服务器api接口地址
description       | String | 描述

<a id="dns-domain"></a>
### dns domain
属性              | 类型   |说明
------------------|--------|-----------
id                | Number | id
creator           | String | 创建人
created_time      | String | 创建时间
name              | String | 域名
available_actions | String | [available domain actions](#available-domain-actions)

<a id="available-domain-actions"></a>
#### available domain actions
属性              | 类型   |说明
------------------|--------|-----------
edit              | Bool   |  编辑
delete            | Bool   |  删除

<a id="dns-domain-record"></a>
### dns domain record
属性              | 类型   |说明
------------------|--------|-----------
id                | Number | id
creator           | String | 创建人
created_time      | String | 创建时间
name              | String | 记录名
value             | String | 记录值
type              | String | 记录类型， 可选值['A', 'MX', 'CNAME', 'NS']

<a id="ip-address-object"></a>
## Ip Address Object
属性                    | 类型   | 说明
----------------------- |--------|---------
id                      | Number | ID
owner                   | String | IP地址绑定对象类型, 默认为HOST, 可选值: ['HOST', 'LB', null]
is_virtual              | Bool   | 是否为虚拟地址
addr_type               | String | IP地址类型，可选值:['PRIVATE','PUBLIC']
network                 | String | 网络ID
netmask                 | String | 子网掩码
address                 | String | IP地址

<a id="user-object"></a>
## User object

属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | 用户id
username                | String  | 用户名
email                   | String  | 邮箱
phone                   | String  | 手机号码
status                  | String  | 用户状态, 可选值['enabled', 'disabled']

<a id="role-object"></a>
## role object

属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | 用户id
name                    | String  | 用户名

<a id="external-navigator-object"></a>
## external navigator object

属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | id
name                    | String  | 导航名称
img                     | String  | 导航图片路径
url                     | String  | 导航地址

<a id="auth-token-object"></a>
## auth token object

属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | id
name                    | String  | token名
value                   | String  | token值
description             | String  | token描述

<a id="cdn-refresh-task"></a>
## cdn refresh task

属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | id
urls                    | Array   | Array of url
cdn_service_provider    | String  | cdn厂商， 可选值['ALI_CDN', 'TECENT_CDN', 'WANGSU']
refresh_mode            | String  | 刷新模式, recursive - 递归刷新 ， single_file - 单文件刷新
status                  | String  | 任务状态, 可选值 ['RUNNING', 'FINISHED', 'FAILED'，'TIMEOUT']
error                   | String &vert; null | 错误信息， 当任务为'FAILED 时候'，该字段包含详细错误信息， 其他状态时 为空.
created_time            | String  | 创建时间
finished_time           | String &vert; null | 完成时间

<a id="jump-server-log"></a>
##  jump server log
属性                    | 类型    | 说明
----------------------- |---------|---------
id                      | Number  | id
user                    | String  | 操作用户    
host                    | String  | 操作主机
text                    | String  | 操作日志内容
created_time            | String  | 操作时间

<a id="dns-operation"></a>
## dns operation

属性             | 类型    | 说明
-----------------|---------|---------
id               | Number  | id
op_target        | String  | 操作对象类型, 可选值['server', 'domain', 'record']op_type          | String  | 操作类型，可选值['add', 'delete', 'update']
op_detail        | String  | 操作详情
op_time          | String  | 操作时间
operator         | String  | 操作人

<a id="host-operation"></a>
## host operation

属性             | 类型    | 说明
-----------------|---------|---------
id               | Number  | id
hostname         | String  | 主机名
op_type          | String  | 操作类型, 可选值['add', 'delete', 'update', 'deatach_app', 'attach_app']
op_detail        | String  | 操作详情
op_time          | String  | 操作时间
operator         | String  | 操作人

<a id="app-operation"></a>
## app operation

属性             | 类型    | 说明
-----------------|---------|---------
id               | Number  | id
app_name         | String  | 应用名
op_type          | String  | 操作类型, 可选值['add', 'update', 'delete', 'attach_host', 'deatach_host', 'change_deploy_setting']
op_detail        | String  | 操作详情
op_time          | String  | 操作时间
operator         | String  | 操作人

<a id="module-authorized-operation"></a>
## module authorized operation

属性                    | 类型   | 说明
------------------------|--------|---------
id                      | Number | id
operator                | String | 操作人
module_name             | String | 被授权模块名
perm_name               | String | 权限名
action                  | String | 授权动作类型 ['enable', 'disable'] 
authorized_target_type  | String | 获得授权的目标类型，可选值 ['role', 'user']
authorized_target_name  | String | 获得授权的用户或角色名
op_time                 | String | 操作时间


<a id="resource-authorized-operation"></a>
## resource authorized operation

属性                    | 类型   | 说明
------------------------|--------|---------
id                      | Number | id
operator                | String | 操作人
resource_type           | String | 被授权资源类型, 可选值['host', 'application', 'business']
resource_id             | Number | 被授权资源id
perm_name               | String | 权限名
action                  | String | 授权动作类型 ['enable', 'disable'] 
authorized_target_type  | String | 获得授权的目标类型，可选值 ['role', 'user']
authorized_target_name  | String | 获得授权的用户或角色名
op_time                 | String | 操作时间



