# mip-xiaomi-router

mip-xiaomi-router 组件说明

标题|内容
----|----
类型|通用
支持布局|responsive,fixed-height,fill,container,fixed
所需脚本|https://mipcache.bdstatic.com/extensions/platform/v1/mip-xiaomi-router/mip-xiaomi-router.js

## 示例

### 基本用法

```html
<!-- 默认不启动服务 -->
<mip-xiaomi-router packageName="xxx.xxx.xxx"></mip-xiaomi-router>
```

```html
<!-- 直接启动服务 -->
<mip-xiaomi-router packageName="xxx.xxx.xxx" appRouter="true"></mip-xiaomi-router>
```

```html
<!-- 启动服务前提示确认 -->
<mip-xiaomi-router packageName="xxx.xxx.xxx" page="home" appRouter="true" confirm="true"></mip-xiaomi-router>
```

```html
<!-- 安装快捷方式时应用名称 -->
<mip-xiaomi-router packageName="xxx.xxx.xxx" appName="应用名称"></mip-xiaomi-router>
```

## 属性

### packageName

说明：manifest.json中声明的包名
必选项：是
类型：string

### confirm

说明：确认提示是否打开服务；不填不做提示确认
必选项：否
类型：{true|false}

### appRouter

说明：是否直接启动服务；不填默认不直接启动
必选项：否
类型：{true|false}

### page

说明：要打开的页面
必选项：否
类型：string

### appName

说明：安装桌面快捷方式的名称
必选项：否
类型：string

### params

说明：请求附带的参数，通过：a1=v1&a2=v2的方式书写
必选项：否
类型：string


## 事件

### evtAppRouter

说明：调用服务

### evtInstallShortcut

说明：安装桌面快捷方式

### evtCallNative

说明: 直接调用底层服务

## 注意事项

