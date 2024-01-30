## 七牛云文件快速上传

- **chenxuan**

## 作用

- 方便的七牛云客户端实现上传方便

## 获取方法

1. 直接通过release版本下载

2. 下载源码编译

3. 使用docker

## 使用方法

1. 修改config文件夹内的demo.json(主要是添加七牛云参数)并重新命名为config.json

2. 运行qiniuserver

## 参数说明
```
{
	"host":{
		"ip":"127.0.0.1", // 绑定ip
		"port":"5200" // 绑定端口
	},
	"qiniu":{
		"domain":"demo", // cdn的域名
		"access_key":"demo", // qiniu云的accesskey
		"secret_key":"demo", // qiniu云的secretkey
		"bucket":"demo", // qiniu云的bucket
		"upload_path":"demo", // qiniu云的上传路径
		"file_name":"", // 自定义上传文件名,为空就是保持原文件名,%d表示日期,%f表示原文件名,%r表示6位随机字符串,目前只支持这几个
		"zone":"Huadong" // qiniu云的地区
	}
}
```
