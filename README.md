<!--
 * @Description: What's this for
 * @Autor: WangYuan
 * @Date: 2021-12-20 14:20:57
 * @LastEditors: WangYuan
 * @LastEditTime: 2021-12-21 16:55:00
-->
<!-- [English](./README.md) | 简体中文  -->

<h2 align="center">Mall-Cook - 商城可视化搭建平台</h2>

> 基于vue开发可视化商城搭建平台

> 我前端基建梦想的一小步

## 介绍
Mall-Cook是一个基于vue开发的可视化商城搭建平台，包括多页面可视化构建、Json Schema生成器（可视化搭建物料控制面板），实现组件流水线式标准接入平台。

<p data-tool="mdnice编辑器" style="font-size: 16px; padding-top: 8px; padding-bottom: 8px; margin: 0; line-height: 26px; color: black;">掘金文章具体介绍平台：<a href="https://juejin.cn/post/7040993073437868063" style="text-decoration: none; color: #1e6bb8; word-wrap: break-word; font-weight: bold; border-bottom: 1px solid #1e6bb8;">传送门</a></p>

## 体验
<p data-tool="mdnice编辑器" style="font-size: 16px; padding-top: 8px; padding-bottom: 8px; margin: 0; line-height: 26px; color: black;">预览地址：<a href="http://110.42.184.128:8000/#/login" style="text-decoration: none; color: #1e6bb8; word-wrap: break-word; font-weight: bold; border-bottom: 1px solid #1e6bb8;">传送门</a></p>

<figcaption style="margin-top: 10px;margin-bottom: 10px; text-align: center; color: #888; font-size: 14px;">拖拽构建页面</figcaption>
<img src="https://files.mdnice.com/user/2544/f5f46fc7-38cf-4221-ae81-98274080f832.gif" alt style="display: block; margin: 0 auto; max-width: 100%;">

<figcaption style="margin-top: 30px;margin-bottom: 10px; text-align: center; color: #888; font-size: 14px;">Json-Schema生成器</figcaption>
<img src="https://files.mdnice.com/user/2544/4e087cef-f13a-4b35-8bbf-1b8156740ba0.gif" alt style="display: block; margin: 0 auto; max-width: 100%;">


## 特别插入
项目从被阮一峰老师推荐到技术周刊，到一天得到200个star深深的激励了我，感谢大佬们的抬爱。

本着授人以鱼不如授人以渔思想，我决定在项目新建shelf分支，正常迭代Mall-Cook情况下，从零重构一套"干净"的可视化架构（很多现成的思路和组件是能复用的，并不是重新写一个），同时会在掘金同步出教程文章详细讲述关键功能点，带大家一览此类平台从零到架构搭建的整个过程，谢谢大家的支持

<figcaption style="margin-top: 10px;margin-bottom: 10px; text-align: center; color: #888; font-size: 14px;">Mall-Cook平台架构</figcaption>
<img src="https://files.mdnice.com/user/2544/75704807-4c6d-47a1-b982-b973f99fea09.png" alt style="display: block; margin: 0 auto; max-width: 100%;">

关键功能点：
- 可视化拖拽面板搭建
- Json Schema 生成器构建
- 组件嵌套开发
- json配置属性面板实现
- 多页面功能开发
- 生成uni-app程序，实现多端复用
## 特性

- 项目基于VUE语言开发
- 暂支持生成H5商城，后续提供生成小程序商城
- 生成商城支持屏幕适配
- 提供物料Json Schema 生成器，根据Json自动生成配置栏
- 提供多页面搭建
- 提供模板商城，可直接套用模板构建商城
- 自定义底部tab菜单



## 安装

```bash
$ npm istall          # install cli
$ npm run dev         # 开发
$ npm run build:dev   # 编译发布 (包括平台与h5商城项目)
```

## 结构

```javascript
├─ h5                                   // h5项目
│  ├─ api                       
│  ├─ assets                     
│  ├─ components                 
│  ├─ pages                      
│  ├─ router                     
│  ├─ store                      
│  ├─ utils                      
│  ├─ App.vue                    
│  └─ main.js                    
├─ src                                  // admin项目  
│  ├─ api   
│  ├─ assets                         
│  ├─ components              
│  ├─ config                            // 初始配置文件     
│  ├─ custom-components                 // 物料库
│  ├─ custom-schema-template            // 属性组件库
│  ├─ custom-schema-template-set        // 属性面板生成器
│  ├─ mixin                              
│  ├─ pages        
│  ├─ router  
│  ├─ scss  
│  ├─ store  
│  ├─ utils  
│  ├─ App.vue  
│  └─ main.js              
├─ package.json   
└─ webpack.config.js    
```

## to do list
- 持续业务组件开发
- 开发小程序版商城（uni-app）
- 开发物料库（uni-app版），可在现有小程序中引入物料库，传入Mall-Cook配置Json，即可生成页面
- 探索平台接入NPM组件

