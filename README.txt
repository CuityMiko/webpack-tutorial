����Webpack��ѧϰ

һ����װ

1.Node.js����һ����������npm,webpack��ͨ��npm��װ��
$ npm install webpack -g(ȫ�ְ�װ)

2.���ذ�װ  
��1��Ϊnpm���һ��package.json�����ļ���$ npm init
//package.json�ļ������ֹ���д��Ҳ����ʹ��npm init�����Զ�����
��2�����webpack�� package.json��
$ npm install webpack --save
//��ʱpackage.json�ļ��л�������´��룺  "dependencies": {
    "webpack": "^1.14.0"
  }
ע��ÿ����Ŀ�ĸ�Ŀ¼���棬һ�㶼��һ��package.json�ļ��������������Ŀ����Ҫ�ĸ���ģ�飬�Լ���Ŀ��������Ϣ���������ơ��汾�����֤��Ԫ���ݣ���npm install���������������ļ����Զ����������ģ�飬Ҳ����������Ŀ��������кͿ�������������package.json���http://javascript.ruanyifeng.com/nodejs/packagejson.html

��������

1�����һ�������ļ�webpack.config.js��һ�����js�ļ�main.js��һ����̬ҳ�� index.html

2���������� $ webpack-dev-server �������ʹ�� http://localhost:8080 ��Ԥ��

����ʹ��

1��Babel���� ����Ԥ���������ɽ� JSX/ES6 ת���� js �ļ���
��װ����  npm install babel-loader babel-preset-es2015 babel-preset-react react react-dom --save
��demo02

2��css���� Webpack��������js�ļ�������CSS�ļ���Ȼ���� CSS-loader ��CSS�ļ�����Ԥ�����������demo03����CSS-loader �� style-loader�� ��װ����
 npm install css-loader style-loader --save
��demo03
3��ͼƬ������Ҫ���� file-loader �� url-loader ����װ����
npm install url-loader file-loader --save
��demo05

4��css-loader?modules (��ѯģ��Ĳ���) ʹ��CSSģ��Ĺ�񡣼���CSSģ��Ĭ���Ǳ��������������Ҫ��CSS������ȫ�֣���ý�ѡ��������global����:global(.h2) ��demo05

5��UglifyJs��� Webpack �в��ϵͳ����չ�书�ܡ����磺UglifyJs Plugin�� main.js ���ѹ���汾�� bundle.js��demo06

6��HTML Webpack��� html-webpack-plugin �ܴ���index.html �ļ�����demo07

7��open-browser-webpack-plugin�����Զ���http://localhost:8080/
```js
plugins: [
    new HtmlwebpackPlugin({
      title: 'Webpack-demos'
    }),
    new OpenBrowserPlugin({
      url: 'http://localhost:8080'
    })
]
8��jQuery/jslite����
jQuery��һ�����١�����JavaScript���,��װJavaScript���õĹ��ܴ��룬�ṩһ�ּ���JavaScript���ģʽ���Ż�HTML

��װ����$ npm install jquery --save

��Ӧ��main.jsд��

var $ = require('jslite');
$('h1').text('Hello World');//�൱��<h1>hello world<h2>
��demo13