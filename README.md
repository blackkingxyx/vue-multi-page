# vue2.*  (多页面跳转)

 @[vue2.3.3|webpack2.6.1|scss|axios]

>- 以前看过有相关朋友share了空的多页面脚手架. 不过down了几个都是webpack1.0或者vue1.0的.
>- 刚好项目需要用到vue. 就在vue-cli的基础上进行了修改
>- 已经有babel直接用es6即可,如果需要修改配置的请到 .babelrc里面修改
>- **并且全局引了JQ(如果不需要或者不喜欢 请到base.conf.js里面修改)**

## 命令
>国际惯例

- **npm install (or cnpm 其他)** 装依赖包
- **npm run dev** 起服务
- **npm run build** 打上线包
- 跑起来服务后,需要在url输入 /module/*.html (*为对应文件夹名字)
- 添加了新文件夹后,需要重新 npm run dev一下

---

##目录结构
1. build/config: 一系列配置文件
2. src: 页面文件
3. (src)assets: 
- js公用的方法/配置方法
- scss公用的样式和base.scss
- lib.js页面引用的入口
4. (src)components: 复用的组件
5. (src)module: **相关的页面** (每个文件夹表示一个页面)
- app.vue (页面)
- *.html (页面的入口,需要和文件夹名称一致)
- *.js (页面的js入口,需要和文件夹名称一致)
- **在static文件夹中的tpl有模板直接复制就ok**

---

