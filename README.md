# Antdv工作流组件 smart-flow-design

<p align="center">
  <a href="https://github.com/vuejs/vue">
    <img src="https://img.shields.io/badge/vue-2.6.14-brightgreen.svg" alt="vue">
  </a>
  <a href="https://github.com/vueComponent/ant-design-vue">
    <img src="https://img.shields.io/badge/Ant%20Design%20Vue-1.7.8-blue" alt="ant-design-vue">
  </a>
  <a href="https://github.com/Kchengz/k-form-design/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/mashape/apistatus.svg" alt="license">
  </a>
</p>

![图片](https://gitee.com/crowncloud/smart-flow-design/blob/master/demo.png)

## 简介

基于vue、ant-design-vue的自定义组件

注：该项目不兼容vue3.0项目，暂无后续兼容vue3.0的计划

- [码云](https://gitee.com/crowncloud/smart-flow-design)

## 特性
  - 支持在线流程设计器，钉钉审批模式，中国式工作流
  - 支持流程办理、退回、自由流、会签、并行、串行、服务任务等
  - 支持退回任务，退回到指定环节，退回到上一步，退回到发起人
  - 支持转办任务，将任务交接给他人办理，办理完成后继续下一步骤
  - 支持委托任务，将任务委托给他人，他人办理完成后再回到委托人
  - 支持智能提交，相同处理人自动跳过，支持自由指定下一步处理人
  - 支持作废流程，允许发起人快速终止流程，管理员维护终止流程
  - 支持自由流程，根据环节选择，自由跳转到指定环节，特事特办
  - 支持流程撤回，下一步未办理的任务，可进行取回撤销重做任务
  - 支持流程跟踪图，流程状态展现，流转信息，任务历史，任务分配信息
  - 支持一个流程模型挂接多个业务单据，如某公司8种费用审批流程，表单不一样，但流程相同
  - 支持一个表单挂接多个流程环节，以表单角度去管理流程，方便业务理解
  - 流程事件脚本在线编写，包括：流程启动、完成、取消；任务分配、创建、结束等
  - 流程脚本管理（Groovy、Beetl），在线编辑、自动完成、脚本测试、多语言脚本模板维护
  - 我的待办任务处理，我的已办任务、我创建的任务查询、流程跟踪、审批记录查询
  - 流程管控，在无关联表单情况下流程调试，如流程发起、挂起；流程定义、实例、任务等查询；任务办理,重定位等
  - 支持流程组件标签定义（流程按钮、意见审批、下一步流程信息等）快速与自定义的业务表单建立关系。
  - 支持版本化管理流程，新调整的流程业务不影响正在运行，未结束的流程继续流转。
  - 支持任务加签、催办任务、传阅任务、流程委托设置、流水号管理、常用语管理

## 术语

 - **或签：** 一名负责人通过即可通过审批节点
 - **会签：** 需所有负责人通过才能通过审批节点
 - **委托：** 将任务委托给他人，他人办理完成后再回到委托人
 - **转交：** 将审批单转交给指定人处理

#模块安装

## 组件

- FlowDesign 流程设计

## 发布
``` cmd
npm login

npm publish
```

## 本地运行
```cmd
# 使用yarn 
yarn install

yarn run dev

# 使用npm 
npm install

npm run dev
```

## 插件安装
```cmd
# 使用yarn 
yarn add smart-flow-design

# 使用npm 
npm i smart-flow-design --save
```

## 引入组件
``` javascript
// 在main.js引入
import SmartFlowDesign from 'smart-flow-design';
import 'smart-flow-design/styles/flow-design.less';
Vue.use(SmartFlowDesign)
```

## 使用组件
``` html
<template>
  <div>
   <FlowDesign ref="FlowDesign" />
  </div>
</template>
```

## 交流
点击链接加入qq群聊，可以直接提问及反馈bug


License
---
[MIT](https://gitee.com/crowncloud/smart-flow-design/blob/master/LICENSE)
Copyright (c) 2022 luocheng

