# 主组件
> frontend/src/App/App.jsx

1. 使用`react-router-dom`实现路由
2. 通过自定义`white-label`实现浏览器的标题与 icon 的自定义，路径为: `frontend/ce/white-label/whiteLabelling.js`
3. 路由`/:workspaceId/apps/:slug/:pageHandle?/*`导航到`AppsRoute`中，加载`AppLoader`组件
4. 使用`AppsRoute`来验证用户登录情况
    - 4.1 `useSessionManagement` get the info of session
    - 4.2 if the session is invalid, render target component without extra props
    - 4.3 if the session is valid, invoke `onValidSession` to validate session in the server.
    - 4.4 get url params via `handleAppAccess`
5. load `AppLoader` component `frontend/src/AppLoader/AppLoader.jsx`
6. 使用`Y.js`实现多人开发

    


# 使用到的库
1. `classnames`: 条件组合多个 classname
2. `shadcn/ui`: 组件库
3. `tailwind/css`: css库