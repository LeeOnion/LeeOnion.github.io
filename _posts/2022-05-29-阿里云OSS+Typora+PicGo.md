# 阿里云OSS+Typora+PicGO

### 0 前言

本篇文章主要介绍利用阿里云OSS+PicGO，实现Typora图片的上云。

### 1 阿里云OSS

购买完阿里云OSS服务后，在界面右边选择创建新的bucket。

![image-20220529142229558](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291422578.png)

其中Bucket名称自己想一个即可；地域选择离你较近的城市；读写权限改为公共读。

![image-20220529142338783](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291423819.png)

打开新创建的bucket的概览，复制下图红色部分。

![image-20220529142615817](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291426844.png)

在OSS界面的右下角，点击Access Key，获取KeyId和KeySecret。

![image-20220529142804808](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291428827.png)

### PicGo

在Github上下载PicGo的可执行文件。

```
https://github.com/Molunerfinn/PicGo/releases
```

打开PicGo的图床选项，找到阿里云，进行配置。

其中KeyId和KeySecret为阿里云上获取得到；存储空间名为你创建bucket时的名称；存储区域为上述获取的地址；存储路径可自定义。

![image-20220529143119914](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291431935.png)



### Typora

打开Typora左上角的文件->偏好设置->图像，进行如下设置即可。

![image-20220529143314928](https://typorabucket.oss-cn-hangzhou.aliyuncs.com/typoraImage/202205291433950.png)
