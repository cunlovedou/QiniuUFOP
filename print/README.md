## PHP UFOP DEMO

*  功能：

1. 安装一个PHP的环境.
2. 启动一个server监听 9100 端口.
3. 接收`POST`请求数据，并将接收到的`POST`请求数据返回出来.


* qufopctl 使用说明：

* ` qufopctl build <Ufop> [-dir <BuildDir>]                                         - Build image with resources contained in <dir>`
将本地的资源打包上传，并在线上进行build。

* `qufopctl imageinfo <Ufop> [-v <Version>]                                        - Retrieve image info` 查看镜像的build信息

* `qufopctl state <Ufop> [-index <Index> | -range <IndexStart:IndexEnd>]           - Check state(s) of one or several ufop instance(s)`
查看当前实例的运行信息

* ` qufopctl ufopver <Ufop> [-c <Version>]                                          - Switch ufop version`
将当前的ufop切换版本， ps: `切换后需要配合 qufopctl upgrade 新版本才能生效`

