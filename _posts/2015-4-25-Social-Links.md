---
layout: post
title: ��ô��Jekyll�Զ��������罻ý���ͼ��
---

  ��Github���˲��ͣ����˺ö�����⣬�������Ǵ�����ˬ��Jekyll Now��ʼ������������İ����ݷḻ������
  
  ��һ��ֻ����������΢����ͼ�����Ӽӵ���ע����ͼ���Google Analytics�Ķ���������Google Analytics���Ѿ�֧�ֵģ���Ҫ���Ľ����ǵ�Google����վ��ȥע����Ӧ��һ����Ŀ���Ϳ��Լ�ر���վ�ķ��������ˡ�

  ������Ҫ��¼һ����ô��ӵ�����΢����ͼ�����ӣ���Ϊ��Google��Ҳû����������Ӧ����Ϣ�������о�Դ������ã��Ѿ��ɹ�������ˡ��������罻��վ��ͼ��Ҳ���ơ�
  
  1. ׼��ͼ��
  ![_config.yml]({{ site.baseurl }}/images/weibo.png)
  ���ͼ�����Ѿ��޸ĺ��ˣ�ע��ͼ���Сһ����40*40�ģ����߻���ѿ��������֧��͸�������ģ�Ҫ��Ҳ���ÿ���
  
  2. ����ͼ���base64��data
  ��������һЩ����������������վ��
  [b64.io](http://b64.io/)
  [AskApache's Base64 encoder/decoder](http://www.askapache.com/online-tools/base64-image-converter/)
  [duri.me](http://duri.me/)
  
  3. �޸�_sass/_svg-icons.scss �ļ�
  ��������&�Ų����µ�ͼƬ��base64������ճ����ȥ�Ϳ�����
  
  4. �޸�_config.yml �ļ�
  ��footer-links�������һ�� weibo����Ӧ��ֵ��������΢����������
  
  5. �޸�_includes/svg-icons.html �ļ�
  ��������һ��{% if site.footer-links.weibo %}<a href="http://weibo.com/{{ site.footer-links.weibo }}"><i class="svg-icon weibo"></i></a>{% endif %}
 