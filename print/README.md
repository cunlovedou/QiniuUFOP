## PHP UFOP DEMO

*  功能：

1. 安装一个PHP的环境.
2. 启动一个server监听 9100 端口.
3. 接收`POST`请求数据，并将接收到的`POST`请求数据返回出来.

比如一个图片调用该ufop： http://rwxf.qiniudn.com/1.png?print
会得到如下返回：

```
{
	cmd: "print",
	src: {
		url: "http://183.136.139.10:24000/get/N9Bc0nNjhyhvRtP7nqf8rg==",
		mimetype: "image/png",
		fsize: 760935,
		bucket: "rwxf",
		key: "1.png"
	}
}
```


* qufopctl 使用说明：

1. ` qufopctl build <Ufop> [-dir <BuildDir>]                                         - Build image with resources contained in <dir>`
将本地的资源打包上传，并在线上进行build。

2. `qufopctl imageinfo <Ufop> [-v <Version>]                                        - Retrieve image info` 查看镜像的build信息

3. `qufopctl state <Ufop> [-index <Index> | -range <IndexStart:IndexEnd>]           - Check state(s) of one or several ufop instance(s)`
查看当前实例的运行信息

4. ` qufopctl ufopver <Ufop> [-c <Version>]                                          - Switch ufop version`
将当前的ufop切换版本， ps: `切换后需要配合 qufopctl upgrade 新版本才能生效`



