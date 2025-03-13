# 启动流程
> 入口地址：frontend/src/index.jsx

1. 使用 `appService.getConfig` 获取到基本配置之后进入初始化流程。
2. 使用 `i18n`库结合`i18next-http-backend`获取语言文件，`react-i18next`绑定 react 实现来实现i18n，与`react-intl`比较来说，`i18n`更加强大，支持动态加载语言文件，而且`react-intl`只支持加载静态的语言文件。
3. 使用`@sentry/react`来实现应用的性能监控 APM 和错误跟踪。
4. 渲染到app 元素中。