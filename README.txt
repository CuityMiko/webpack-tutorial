Webpack
һ����װ
1.Node.js����һ����������npm,webpack��ͨ��npm��װ��
$ npm install webpack -g(ȫ�ְ�װ)

2.���ذ�װ  Ϊnpm���һ��package.json�����ļ���$ npm init
��װ�����webpack�� package.json��
$ npm install webpack --save-dev
��������
1�����һ�������ļ�webpack.config.js��һ�����js�ļ�main.js��һ����̬ҳ�� index.html

2���������� $ webpack-dev-server �������ʹ�� http://localhost:8080 ��Ԥ��

����ʹ��
1��css���� Webpack��������js�ļ�������CSS�ļ���Ȼ���� CSS-loader ��CSS�ļ�����Ԥ�����������demo03����CSS-loader �� style-loader�� ��װ����
 npm install css-loader style-loader --save

2��ͼƬ������Ҫ���� file-loader �� url-loader ����װ����
npm install url-loader file-loader --save