# React项目生成
## GitHub
在github上创建一个代码仓库,git clone 拉下来;
## 安装插件
1. yo
```
npm install -g yo
```

查看版本:
```
yo --version
```
2. generator-react-webpack (自动化项目生成工具)
```
npm install -g generator-react-webpack
```
查看版本:
```
npm ls -g --depth=1 2>/dev/null | grep generator-
```
显示:
```
+-- generator-react-webpack@3.3.4
```
解析:
```
    npm ls -g    列出我们全局安装的所有的npm包
    --depth=1       限制树状展示仅限一层

    > 重定向
    在bash里:     1: 标准输出     2: 错误输出
    /dev/null       空设备文件
    2>/dev/null     如果执行 npm -g 的过程中有错误消息,把错误消息重定向到空设备文件上(就是不显示错误消息)

    |               管道 ,上一次的输出,是下一次的输入
    grep generator-   过滤出generator-

```

3. 自动生成项目
在项目根目录reactExample文件夹中
```
yo react-webpack reactExample
```
返回:
```

Out of the box I include Webpack and some default React components.

? Please choose your application name (reactExample)
(选择项目名)
```
等等,根据提示进行选择
最后会自动生成