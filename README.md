1. ��android studio��ʹ�ðٶȵ�ͼSDK��ϸ����
   1.1 ע���Ϊ�ٶȿ����ߣ���ַΪ http://developer.baidu.com/user/reg
   1.2 ����ٶȵ�ͼAPI��Կ����ַΪ http://lbsyun.baidu.com/apiconsole/key/create
   1.3 ��ȡ����ǩ��(SHA1), ��cmd�н���.android�ļ��У�ִ�� keytool -list -keystore debug.keystore, �����Ҫ�������룬
	   ֱ�Ӻ��Լ��ɣ�֮���ɿ�����Կ����д��Ϻ��ύ���ɣ�֮���ɿ���API_KEY
   1.4 ����SDK�� ��ַΪ http://developer.baidu.com/map/sdkandev-download.htm�� ѡ��һ�����ؼ���
   1.5 ����Ŀ�����.jar�ļ��� �л���project��ͼ�£���xxx.jar���Ƶ�app/libs/Ŀ¼�£���xxx.jar�ļ��ϵ������Ҽ���ѡ��
       ��Add as Libary...��, ��˼�������
   1.6 ����Ŀ�����.so�ļ����л���project��ͼ�£���app/src/main���½�jniLibs/armeabi/Ŀ¼����.so�ļ����Ƶ�armeabiĿ¼
       �¼��ɡ�
	   
2. ��ʹ�ù����������Ŀ�
   2.1 ��AndroidManifest.xml�ļ������ 
		<meta-data
            android:name="com.baidu.lbsapi.API_KEY"
            android:value="4Li8i6GnxWGF7AE1UX7tZ4CO"
            />
		ע�⣺name="com.baidu.lbsapi.API_KEY",���������
		      valueΪ�ղ������API_KEY�����ܰ����κοո�
   2.2 ʹ��LocationManger��ȡλ��ʧ�ܣ�ԭ����δȷ��