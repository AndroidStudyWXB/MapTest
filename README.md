1. 在android studio中使用百度地图SDK详细流程
   1.1 注册成为百度开发者，网址为 http://developer.baidu.com/user/reg
   1.2 申请百度地图API秘钥，网址为 http://lbsyun.baidu.com/apiconsole/key/create
   1.3 获取数字签名(SHA1), 在cmd中进入.android文件夹，执行 keytool -list -keystore debug.keystore, 如果需要输入密码，
	   直接忽略即可，之后便可看到秘钥。填写完毕后，提交即可，之后便可看到API_KEY
   1.4 下载SDK， 网址为 http://developer.baidu.com/map/sdkandev-download.htm， 选择一键下载即可
   1.5 在项目中添加.jar文件， 切换到project视图下，将xxx.jar复制到app/libs/目录下，在xxx.jar文件上点击鼠标右键，选择
       “Add as Libary...”, 如此即完成添加
   1.6 在项目中添加.so文件，切换到project视图下，在app/src/main下新建jniLibs/armeabi/目录，将.so文件复制到armeabi目录
       下即可。
	   
2. 在使用过程遇到过的坑
   2.1 在AndroidManifest.xml文件中添加 
		<meta-data
            android:name="com.baidu.lbsapi.API_KEY"
            android:value="4Li8i6GnxWGF7AE1UX7tZ4CO"
            />
		注意：name="com.baidu.lbsapi.API_KEY",必须是这个
		      value为刚才申请的API_KEY，不能包含任何空格
   2.2 使用LocationManger获取位置失败，原因仍未确定