# React学习

## 目录

- [一、react概述](#%E4%B8%80react%E6%A6%82%E8%BF%B0)
  - [1.1 react是什么](#11-react%E6%98%AF%E4%BB%80%E4%B9%88)
  - [1.2 react的特点](#12-react%E7%9A%84%E7%89%B9%E7%82%B9)
  - [1.3 react的基本使用](#13-react%E7%9A%84%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8)
    - [1.3.1 react的安装](#131-react%E7%9A%84%E5%AE%89%E8%A3%85)
    - [1.3.2 react的使用](#132-react%E7%9A%84%E4%BD%BF%E7%94%A8)
  - [1.4 能够使用react脚手架](#14-%E8%83%BD%E5%A4%9F%E4%BD%BF%E7%94%A8react%E8%84%9A%E6%89%8B%E6%9E%B6)
    - [1.4.1 脚手架的意义](#141-%E8%84%9A%E6%89%8B%E6%9E%B6%E7%9A%84%E6%84%8F%E4%B9%89)
    - [1.4.2 使用脚手架初始化项目](#142-%E4%BD%BF%E7%94%A8%E8%84%9A%E6%89%8B%E6%9E%B6%E5%88%9D%E5%A7%8B%E5%8C%96%E9%A1%B9%E7%9B%AE)
    - [1.4.3 在脚手架中使用react](#143-%E5%9C%A8%E8%84%9A%E6%89%8B%E6%9E%B6%E4%B8%AD%E4%BD%BF%E7%94%A8react)
  - [1.5 总结](#15-%E6%80%BB%E7%BB%93)
- [二、JSX](#%E4%BA%8Cjsx)
  - [2.1 JSX的基本使用](#21-jsx%E7%9A%84%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8)
    - [2.1.1 createElement()的问题](#211-createelement%E7%9A%84%E9%97%AE%E9%A2%98)
    - [2.1.2 JSX简介](#212-jsx%E7%AE%80%E4%BB%8B)
    - [2.1.3 JSX中使用JavaScript表达式](#213-jsx%E4%B8%AD%E4%BD%BF%E7%94%A8javascript%E8%A1%A8%E8%BE%BE%E5%BC%8F)
  - [2.2 JSX渲染](#22-jsx%E6%B8%B2%E6%9F%93)
    - [2.2.1 条件渲染](#221-%E6%9D%A1%E4%BB%B6%E6%B8%B2%E6%9F%93)
    - [2.2.2 列表渲染](#222-%E5%88%97%E8%A1%A8%E6%B8%B2%E6%9F%93)
    - [2.2.3 样式处理](#223-%E6%A0%B7%E5%BC%8F%E5%A4%84%E7%90%86)
  - [2.3 JSX总结](#23-jsx%E6%80%BB%E7%BB%93)
- [三、React组件基础](#%E4%B8%89react%E7%BB%84%E4%BB%B6%E5%9F%BA%E7%A1%80)
  - [3.1 组件介绍](#31-%E7%BB%84%E4%BB%B6%E4%BB%8B%E7%BB%8D)
  - [3.2 组件的创建方式](#32-%E7%BB%84%E4%BB%B6%E7%9A%84%E5%88%9B%E5%BB%BA%E6%96%B9%E5%BC%8F)
    - [3.2.1 使用函数创建组件](#321-%E4%BD%BF%E7%94%A8%E5%87%BD%E6%95%B0%E5%88%9B%E5%BB%BA%E7%BB%84%E4%BB%B6)
    - [3.2.2 使用类创建组件](#322-%E4%BD%BF%E7%94%A8%E7%B1%BB%E5%88%9B%E5%BB%BA%E7%BB%84%E4%BB%B6)
    - [3.2.3 把组件抽离为独立的JS文件](#323-%E6%8A%8A%E7%BB%84%E4%BB%B6%E6%8A%BD%E7%A6%BB%E4%B8%BA%E7%8B%AC%E7%AB%8B%E7%9A%84js%E6%96%87%E4%BB%B6)
  - [3.3 事件处理](#33-%E4%BA%8B%E4%BB%B6%E5%A4%84%E7%90%86)
    - [3.3.1 事件绑定](#331-%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A)
    - [3.3.2 事件对象](#332-%E4%BA%8B%E4%BB%B6%E5%AF%B9%E8%B1%A1)
  - [3.4 有状态组件和无状态组件](#34-%E6%9C%89%E7%8A%B6%E6%80%81%E7%BB%84%E4%BB%B6%E5%92%8C%E6%97%A0%E7%8A%B6%E6%80%81%E7%BB%84%E4%BB%B6)
  - [3.5 组件中的state和setState](#35-%E7%BB%84%E4%BB%B6%E4%B8%AD%E7%9A%84state%E5%92%8Csetstate)
    - [3.5.1 state的基本使用](#351-state%E7%9A%84%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8)
    - [3.5.2 setState()修改状态](#352-setstate%E4%BF%AE%E6%94%B9%E7%8A%B6%E6%80%81)
    - [3.5.3 从jsx中抽离事件处理程序](#353-%E4%BB%8Ejsx%E4%B8%AD%E6%8A%BD%E7%A6%BB%E4%BA%8B%E4%BB%B6%E5%A4%84%E7%90%86%E7%A8%8B%E5%BA%8F)
    - [3.5.4 事件绑定this指向](#354-%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9Athis%E6%8C%87%E5%90%91)
    - [3.5.6 事件绑定总结](#356-%E4%BA%8B%E4%BB%B6%E7%BB%91%E5%AE%9A%E6%80%BB%E7%BB%93)
  - [3.6 表单处理](#36-%E8%A1%A8%E5%8D%95%E5%A4%84%E7%90%86)
    - [3.6.1 受控组件](#361-%E5%8F%97%E6%8E%A7%E7%BB%84%E4%BB%B6)
    - [3.6.2 受控组件的多表单元素优化](#362-%E5%8F%97%E6%8E%A7%E7%BB%84%E4%BB%B6%E7%9A%84%E5%A4%9A%E8%A1%A8%E5%8D%95%E5%85%83%E7%B4%A0%E4%BC%98%E5%8C%96)
    - [3.6.3 非受控组件（不推荐使用）](#363-%E9%9D%9E%E5%8F%97%E6%8E%A7%E7%BB%84%E4%BB%B6%E4%B8%8D%E6%8E%A8%E8%8D%90%E4%BD%BF%E7%94%A8)
  - [3.7 组件总结](#37-%E7%BB%84%E4%BB%B6%E6%80%BB%E7%BB%93)
  - [3.8 React组件案例](#38-react%E7%BB%84%E4%BB%B6%E6%A1%88%E4%BE%8B)
    - [3.8.1 案例：评论列表](#381-%E6%A1%88%E4%BE%8B%E8%AF%84%E8%AE%BA%E5%88%97%E8%A1%A8)
- [四、React组件进阶](#%E5%9B%9Breact%E7%BB%84%E4%BB%B6%E8%BF%9B%E9%98%B6)
  - [4.1 组件的props](#41-%E7%BB%84%E4%BB%B6%E7%9A%84props)
  - [4.2 组件通讯的三种方式](#42-%E7%BB%84%E4%BB%B6%E9%80%9A%E8%AE%AF%E7%9A%84%E4%B8%89%E7%A7%8D%E6%96%B9%E5%BC%8F)
    - [4.2.1 父组件传递数据给子组件](#421-%E7%88%B6%E7%BB%84%E4%BB%B6%E4%BC%A0%E9%80%92%E6%95%B0%E6%8D%AE%E7%BB%99%E5%AD%90%E7%BB%84%E4%BB%B6)
    - [4.2.2 子组件传数据给父组件](#422-%E5%AD%90%E7%BB%84%E4%BB%B6%E4%BC%A0%E6%95%B0%E6%8D%AE%E7%BB%99%E7%88%B6%E7%BB%84%E4%BB%B6)
    - [4.2.3 兄弟组件之间的通讯](#423-%E5%85%84%E5%BC%9F%E7%BB%84%E4%BB%B6%E4%B9%8B%E9%97%B4%E7%9A%84%E9%80%9A%E8%AE%AF)
  - [4.3 Context](#43-context)
  - [4.3 props深入](#43-props%E6%B7%B1%E5%85%A5)
    - [4.3.1 children属性](#431-children%E5%B1%9E%E6%80%A7)
    - [4.3.2 props校验](#432-props%E6%A0%A1%E9%AA%8C)
    - [4.3.3 props的默认值](#433-props%E7%9A%84%E9%BB%98%E8%AE%A4%E5%80%BC)
  - [4.4 组件的生命周期](#44-%E7%BB%84%E4%BB%B6%E7%9A%84%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F)
    - [4.4.1 组件的生命周期概述：](#441-%E7%BB%84%E4%BB%B6%E7%9A%84%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F%E6%A6%82%E8%BF%B0)
    - [4.4.2 生命周期的三个阶段](#442-%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F%E7%9A%84%E4%B8%89%E4%B8%AA%E9%98%B6%E6%AE%B5)
  - [4.5 render-props](#45-render-props)
    - [4.5.1 render props模式](#451-render-props%E6%A8%A1%E5%BC%8F)
    - [4.5.2 演示Mouse组件的复用](#452-%E6%BC%94%E7%A4%BAmouse%E7%BB%84%E4%BB%B6%E7%9A%84%E5%A4%8D%E7%94%A8)
    - [4.5.3 childern代替render属性](#453-childern%E4%BB%A3%E6%9B%BFrender%E5%B1%9E%E6%80%A7)
  - [4.6 高阶组件](#46-%E9%AB%98%E9%98%B6%E7%BB%84%E4%BB%B6)
    - [4.6.1 概述](#461-%E6%A6%82%E8%BF%B0)
    - [4.6.2 设置displayName](#462-%E8%AE%BE%E7%BD%AEdisplayname)
    - [4.6.3 传递props](#463-%E4%BC%A0%E9%80%92props)
  - [4.7 React组件进阶总结](#47-react%E7%BB%84%E4%BB%B6%E8%BF%9B%E9%98%B6%E6%80%BB%E7%BB%93)
- [五、React原理](#%E4%BA%94react%E5%8E%9F%E7%90%86)
  - [5.1 学习目标](#51-%E5%AD%A6%E4%B9%A0%E7%9B%AE%E6%A0%87)
  - [5.2 setState()说明](#52-setstate%E8%AF%B4%E6%98%8E)
    - [5.2.1 更新数据与推荐语法](#521-%E6%9B%B4%E6%96%B0%E6%95%B0%E6%8D%AE%E4%B8%8E%E6%8E%A8%E8%8D%90%E8%AF%AD%E6%B3%95)
    - [5.2.2 setState的第二个参数](#522-setstate%E7%9A%84%E7%AC%AC%E4%BA%8C%E4%B8%AA%E5%8F%82%E6%95%B0)
  - [5.3 JSX语法的转化过程](#53-jsx%E8%AF%AD%E6%B3%95%E7%9A%84%E8%BD%AC%E5%8C%96%E8%BF%87%E7%A8%8B)
  - [5.4 组件更新机制](#54-%E7%BB%84%E4%BB%B6%E6%9B%B4%E6%96%B0%E6%9C%BA%E5%88%B6)
  - [5.5 组件性能优化](#55-%E7%BB%84%E4%BB%B6%E6%80%A7%E8%83%BD%E4%BC%98%E5%8C%96)
    - [5.5.1 减轻state](#551-%E5%87%8F%E8%BD%BBstate)
    - [5.5.2 避免不必要的重新渲染](#552-%E9%81%BF%E5%85%8D%E4%B8%8D%E5%BF%85%E8%A6%81%E7%9A%84%E9%87%8D%E6%96%B0%E6%B8%B2%E6%9F%93)
    - [5.5.3 纯组件](#553-%E7%BA%AF%E7%BB%84%E4%BB%B6)
  - [5.6 虚拟DOM和Diff算法](#56-%E8%99%9A%E6%8B%9Fdom%E5%92%8Cdiff%E7%AE%97%E6%B3%95)
  - [5.7 React原理总结](#57-react%E5%8E%9F%E7%90%86%E6%80%BB%E7%BB%93)
- [六、React路由](#%E5%85%ADreact%E8%B7%AF%E7%94%B1)
  - [6.1 React路由介绍](#61-react%E8%B7%AF%E7%94%B1%E4%BB%8B%E7%BB%8D)
  - [6.2 路由的基本使用](#62-%E8%B7%AF%E7%94%B1%E7%9A%84%E5%9F%BA%E6%9C%AC%E4%BD%BF%E7%94%A8)
  - [6.3 常用组件说明](#63-%E5%B8%B8%E7%94%A8%E7%BB%84%E4%BB%B6%E8%AF%B4%E6%98%8E)
  - [6.4 路由的执行过程](#64-%E8%B7%AF%E7%94%B1%E7%9A%84%E6%89%A7%E8%A1%8C%E8%BF%87%E7%A8%8B)
  - [6.5 编程式导航](#65-%E7%BC%96%E7%A8%8B%E5%BC%8F%E5%AF%BC%E8%88%AA)
  - [6.6 默认路由](#66-%E9%BB%98%E8%AE%A4%E8%B7%AF%E7%94%B1)
  - [6.7 匹配模式](#67-%E5%8C%B9%E9%85%8D%E6%A8%A1%E5%BC%8F)
    - [6.7.1 模糊匹配模式](#671-%E6%A8%A1%E7%B3%8A%E5%8C%B9%E9%85%8D%E6%A8%A1%E5%BC%8F)
    - [6.7.2 精确匹配模式](#672-%E7%B2%BE%E7%A1%AE%E5%8C%B9%E9%85%8D%E6%A8%A1%E5%BC%8F)
  - [6.8 React路由基础总结](#68-react%E8%B7%AF%E7%94%B1%E5%9F%BA%E7%A1%80%E6%80%BB%E7%BB%93)

# react学习

## 一、react概述

### 1.1 react是什么

- react是一个用于构建用户界面的JavaScript库
- 用户界面：HTML界面（前端）
- react主要用来写HTML界面，或构建web应用
- 从MVC角度看，react仅仅是视图层（V），负责视图的渲染


### 1.2 react的特点

1. 声明式
   - 只需要描述UI，跟写HTML一样
   - react负责渲染UI，并在数据变化时更新UI

2. 基于组件
	- 组件是react最重要的内容
	- 组件表示内容的部分内容
	- 组合、复用多个组件，可以实现完整的页面功能

3. 学习一次，随处使用
	- react可以开发web应用
	- react开发移动端原生应用
	- react开发VR应用

### 1.3 react的基本使用

#### 1.3.1 react的安装

安装命令：npm i react react-dom

react包是核心，提供创建元素，组件等功能

react-dom包提供DOM相关功能

#### 1.3.2 react的使用

1. 引入react和react-dom两个js文件
2. 创建react元素
3. 渲染react元素到页面中

react的使用：

	 //创建react元素
	 //参数一：元素名称
	 //参数二：元素属性
	 //参数三及其以后的参数：元素的子节点
	 const title=React.createElement(
	 'p',
	 {titie:'标题'},
	 'Hello',
	 React.createElement('span',null,'我是span标签')
	 )
	
	 //渲染react元素
	 //参数一：要渲染的react元素
	 //参数二：挂载点
	 ReactDOM.render(title,document.getElementById('root'))
	

*渲染后的效果：*

    <div id="root">
    	<p titie="标题">
    	   Hello
		<span>我是span标签</span>
       </p>
    </div>

### 1.4 能够使用react脚手架

#### 1.4.1 脚手架的意义

1. 脚手架是开发现代web应用的必备
2. 充分利用webpack、Babel、ESLint等工具辅助项目开发
3. 零配置，无需手动配置繁琐的工具即可使用
4. 关注业务，而不是工具配置


#### 1.4.2 使用脚手架初始化项目

1. 初始化项目：命令：`npm create-react-app my-app`
2. 启动项目，在项目根目录执行命令：`npm start`

#### 1.4.3 在脚手架中使用react

1. 导入react和react-dom两个包 `import React from 'react'``import ReactDOM from 'react-dom'`
2. 调用React-createElement()方法创建react元素
3. 调用ReactDOM.render()方法渲染react元素到页面中

### 1.5 总结

**React基础**

1. React是构建用户界面的JavaScript库
2. 使用react时，推荐使用脚手架方式
3. 初始化命令：`npm create-react-app my-app`
4. 启动项目命令：	`yarn start` 或者`npm start`
5. React.createElement()方法用于创建react元素到页面中
6. ReactDOM.render()方法负责渲染react元素到页面中

## 二、JSX

### 2.1 JSX的基本使用

#### 2.1.1 createElement()的问题

1. 繁琐不简洁
2. 不直观，无法一眼看出所描述的结构
3. 不优雅，用户体验不爽

#### 2.1.2 JSX简介

- JSX是JavaScript XML的简写，表示JavaScript代码中写XML(HTML)格式的代码

- 优势：声明式语法更加直观，与HTML结构相同，降低了学习成本，提升开发效率

- JSX是React的核心内容

**使用步骤**

1. 使用JSX语法创建react元素
2. 使用ReactDOM.render()方法创建react元素到页面中

JSX:

    //使用jsx创建react元素
     const title=<h1>hello jsx</h1>
    //渲染react元素
    ReactDOM.render(title,document.getElementById('root'))

**为什么脚手架中可以使用JSX语法？**

1. JSX不是标准的ECMAScropt语法，它是ECMAScript的语法扩展
2. 需要babel编译处理后，才能在浏览器环境中使用
3. create-react-app脚手架中已经默认有该配置，无需手动配置
4. 编译JSX语法包为：@babel/preset-react


**注意点**

1. React元素的属性名使用驼峰命名法
2. 特殊属性名：class->className, for->htmlFor, tabindex->tablndex
3. 没有子节点的React元素可以用/>结束
4. 推荐：使用小括号包裹JSX，从而避免js中的自动插入分号陷阱

#### 2.1.3 JSX中使用JavaScript表达式

1. 数据存储在JS中
2. 语法：{JavaScript表达式}

### 2.2 JSX渲染

#### 2.2.1 条件渲染

1. 场景：loading效果
2. 条件渲染：根据条件渲染的特定JSX结构
3. 可以使用if/else或三元运算符或逻辑运算符来实现

条件渲染：
    
    const isloading=true
    const loadData=()=>{
      if (isloading){
    return <div>loading</div>
      }
      return <div>数据加载完成</div>
    }
    const title=(
      <h1>
    条件渲染：
    {loadData()}
      </h1>
    )
    ReactDOM.render(title,document.getElementById('root'))


#### 2.2.2 列表渲染

1. 如果要渲染一组数据，应该使用数组的map()方法
2. 注意：渲染列表时应该添加key属性，key属性值要保证唯一
3. 原则：map()遍历谁，就给谁添加key属性
4. 注意：避免使用索引号作为key

列表渲染：

    const songs=[
      { id:1,name:'致未来的我'},
      {id:2,name:'我是你的'},
      {id:3,name:'拜托了世界'}
    ]
    const list=(
      <ul>
    {songs.map(item=><li key={item.id}>{item.name}</li>)}
      </ul>
    )
    ReactDOM.render(list,document.getElementById('root'))

#### 2.2.3 样式处理

1. 行内样式-style
2. 类名-className

jsx的样式处理：

    const list=(
      <h1 className="title" style={{color:'red',background:'skyblue'}}>
    JSX样式处理
      </h1>
    )
    //渲染react元素
    ReactDOM.render(list,document.getElementById('root'))

### 2.3 JSX总结

1. JSX是React的核心内容
2. JSX表示在JS代码中写HTML结构，是React声明式的体现
3. 使用JSX配合嵌入JS表达式，条件渲染，列表渲染，可以描述任意UI结构
4. 推荐使用className的方式结合JSX添加样式
5. React完全利用JS语言自身的能力编写UI，而不是造轮子增强HTML功能

## 三、React组件基础

### 3.1 组件介绍

1. 组件是React的一等公民，使用React就是在组件
2. 组件表示页面中的部分功能
3. 组合多个组件实现完整的页面功能
4. 特点：可复用，独立，可组合

### 3.2 组件的创建方式

#### 3.2.1 使用函数创建组件

1. 函数组件：使用JS的函数或（箭头函数）创建的组件
2. 规则1：函数名必须以大写字母开头(为了区分组件和普通的React元素）
3. 规则2：函数组件必须有返回值，表示该组件的结构
4. 如果返回值为null，表示不渲染任何内容
5. 渲染函数组件：用函数名作为组件标签名
6. 组件标签可以是单标签也可以是双标签

函数组件：

    function Hello(){
      return (
    <div>
      函数组件
    </div>
      )
    }
    // 或箭头函数
    const Hello=()=>(<div>
    函数组件
    </div>
    )
    //渲染组件
    ReactDOM.render(<Hello />,document.getElementById('root'))

#### 3.2.2 使用类创建组件

1. 类组件：使用ES6的class创建的组件
2. 规则1：类名必须要大写字母开头
3. 规则2：类组件应该继承React.Component父类，从而可以使用父类中提供的方法或属性
4. 规则3：类组件必须提供render()方法
5. 规则4：render()方法必须有返回值，表示该组件的结构

类组件：

    class Hello extends React.Component{
      render(){
    return (
      <div>
    类组件
      </div>
    )
      }
    }
    //渲染组件
    ReactDOM.render(<Hello/>,document.getElementById('root'))

#### 3.2.3 把组件抽离为独立的JS文件

**思考：项目中的组件多了之后，该如何组织这些组件？**

组件作为一个独立的个体，一般都会放到一个独立的JS文件中

1. 创建Hello.js
2. 在Hello.js中导入React
3. 创建组件（函数或类）
4. 在Hello.js中导出该组件
5. 在index.js中导入Hello组件
6. 渲染组件

*Hello.js文件*

    import React from 'react'
    
    //创建类组件
    class Hello extends React.Component{
    render(){
    return(
    <div>
    抽离到js文件的组件
    </div>
    )
    }
    }
    //导出组件
    export default Hello

*index.js文件*
    
    //导入Hello组件
    import Hello from './Hello'
    //渲染组件
    ReactDOM.render(<Hello></Hello>,document.getElementById('root'))

### 3.3 事件处理

#### 3.3.1 事件绑定

1. React事件绑定语法与DOM事件语法相似
2. 语法：on+事件名称={事件处理程序}，比如：onClick={()=>{}}
3. 注意：React事件采用驼峰命名法，比如：onMouseEnter,onFocus

类组件：

    class App extends React.Component{
      handleclick(){
    alert('事件触发了')
      }
      render(){
    return (
      <button onClick={this.handleclick}>点我</button>
    )
      }
    }
    //渲染组件
    ReactDOM.render(<App/>,document.getElementById('root'))
    
函数组件：

    function App(){
      function handleclick(){
    alert('事件触发了')
      }
      return (
    <button onClick={handleclick}>点我</button>
      )
    }
    ReactDOM.render(<App/>,document.getElementById('root'))

#### 3.3.2 事件对象

1. 可以通过事件处理程序的参数获取到事件对象
2. React中的事件对象叫做：合成事件（对象）
3. 合成事件：兼容所有浏览器，无需担心跨浏览器兼容性问题

事件对象：

    class App extends React.Component{
      handleclick(e){
   		 alert('事件触发了,但是页面不发生跳转')
    //阻止浏览器的默认行为（不让页面发生跳转）
         e.preventDefault()
        }
      render(){
         return (
           <a href="https://cn.bing.com/?scope=web&FORM=ANNTH1" onClick={this.handleclick}>必应</	a>
       )
      }
    }
    // 渲染组件
    ReactDOM.render(<App />,document.getElementById('root'))

### 3.4 有状态组件和无状态组件

1. 函数组件又叫无状态组件，类组件又叫有状态组件
2. 状态state即数据
3. 函数组件没有自己的状态，只负责数据的展示（静）
4. 类组件有自己的状态，负责更新UI，让页面“动”起来

### 3.5 组件中的state和setState

#### 3.5.1 state的基本使用

1. 状态state即数据，是组件内部的私有数据，只能在组件内部使用
2. state的值是对象，表示一个组件中可以有多个数据
3. 获取状态：this.state

state的初始化：
    
    class App extends React.Component{
      constructor(){
        super()
    // 初始化state
     this.state={
       count:0
     }
      }
      render(){
       return (
      <div>
        <h1>
         计数器:{this.state.count}
   	    </h1>
      </div>
    )
      }
    }
    // 渲染组件
    ReactDOM.render(<App/>,document.getElementById('root'))

#### 3.5.2 setState()修改状态

1. 状态是可变的
2. 语法：this.setState({要修改的数据})
3. 注意：不要直接修改state中的值，这是错误的！
4. setState()作用：1.修改state 2.更新UI
5. 思想：数据驱动视图

正确：

    this.setState({
       count:this.state.count+1
    })

错误：

    this.state.count+=1

setState()修改状态：

	class App extends React.Component{
	  constructor(){
	    super()
	    // 初始化state
	     this.state={
	       count:0
	     }
	  }
	  // 事件处理程序
	  onIncrement(){
	    this.setState({
	      count:this.state.count+1
	    })
	  }
	  render(){
	    return (
	      <div>
	        <h1>
	          计数器:{this.state.count}
	        </h1>
	        <button onClick={()=>{
	          this.setState({
	            count:this.state.count+1
	          })
	        }}>+1</button>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App/>,document.getElementById('root'))

#### 3.5.3 从jsx中抽离事件处理程序

1. jsx中参加过多js逻辑代码，会显得非常混乱
2. 推荐：将逻辑抽离到单独的方法中，保证jsx结构清晰
3. 报错：× TypeError: Cannot read property 'setState' of undefined
4. 原因：事件处理程序中this的值为undefined
5. 希望：this指向组件实例（render方法中的this即为组件实例）


#### 3.5.4 事件绑定this指向

1. 箭头函数
	- 利用箭头函数自身不绑定this的特点
    - render()方法中的this为组件实例，可以获取到setState()
2. Function.prototype.bind()
    - 利用ES5中的bind方法，将事件处理程序中的this与组件实例绑定到一起
3. class的实例方法
    - 利用箭头函数形式的class实例方法
    - 注意：该语法是实验性语法，但是babel的存在可以直接使用

箭头函数：

	class App extends React.Component{
	  constructor(){
	    super()
	    // 初始化state
	     this.state={
	       count:0
	     }
	  }
	  // 事件处理程序
	  onIncrement(){
	    this.setState({
	      count:this.state.count+1
	    })
	  }
	  render(){
	    return (
	      <div>
	        <h1>
	          计数器:{this.state.count}
	        </h1>
	        <button onClick={()=>this.onIncrement()}>+1</button>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App/>,document.getElementById('root'))

Function.prototype.bind():

	class App extends React.Component{
	  constructor(){
	    super()
	    this.state={
	      count:0
	    }
	    this.onIncrement=this.onIncrement.bind(this)
	  }
	    // 事件处理程序
	    onIncrement(){
	      this.setState({
	        count:this.state.count+1
	      })
	    }
	  render(){
	    return(
	      <div>
	      <h1>计时器:{this.state.count}</h1>
	      <button onClick={this.onIncrement}>+1</button>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App/>,document.getElementById('root'))

class的实例方法:

	class App extends React.Component{
	  constructor(){
	    super()
	    this.state={
	      count:0
	    }
	  }
	    // 事件处理程序
	    onIncrement=()=>{
	      this.setState({
	        count:this.state.count+1
	      })
	    }
	  render(){
	    return(
	      <div>
	      <h1>计时器:{this.state.count}</h1>
	      <button onClick={this.onIncrement}>+1</button>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App/>,document.getElementById('root'))

#### 3.5.6 事件绑定总结

1. 推荐:使用class的实例方法
2. 箭头函数
3. bind方法

### 3.6 表单处理

#### 3.6.1 受控组件

1. HTML中的表单元素时可输入的，也就是有自己的可变状态
2. 在React中可变状态通常保存在state中，并且只能通过setState()方法来修改
3. React将state与表单元素值value绑定到一起，由state的值来控制表单元素的值
4. 受控组件：其值受到React控制的表单元素

**步骤**

1. 在state中添加一个状态，作为表单元素的value值（控制表单元素值的来源）
2. 给表单元素绑定change事件，将表单元素的值设置为state的值（控制表单元素值的变化）

代码：

	state={txt:''}
	<input type="text" value={this.state.txt} onChange={e=>this.setState({
	txt:e.target.value
	})}/>

举例代码：

	class App extends React.Component{
	  state={
	    txt:''
	  }
	  handleChange=e=>{
	    this.setState({
	      txt:e.target.value
	    })
	  }
	  render(){
	    return(
	      <div>
	        <input type="text" value={this.state.txt} onChange={this.handleChange}/>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App></App>,document.getElementById('root'))

**示例总结**

1. 文本框，富文本框，下拉框操作value属性
2. 复选框操作checked属性

示例代码：

	class App extends React.Component{
	  state={
	    txt:'',
	    content:'',
	    city:'bj',
	    isChecked:false
	  }
	  handleChange=e=>{
	    this.setState({
	      txt:e.target.value
	    })
	  }
	  handleContent=e=>{
	    this.setState({
	      content:e.target.value
	    })
	  }
	  handleCity=e=>{
	    this.setState({
	      city:e.target.value
	    })
	  }
	  handelChecked=e=>{
	    this.setState({
	      isChecked:e.target.checked
	    })
	  }
	  render(){
	    return(
	      <div>
	        {/* 文本框 */}
	        <input type="text"  value={this.state.txt} onChange={this.handleChange}/>
	        <br/>
	        {/* 富文本框 */}
	        <textarea value={this.state.content} onChange={this.handleContent}></textarea>
	        <br/>
	        {/* 下拉框 */}
	        <select value={this.state.city} onChange={this.handleCity}>
	          <option value="sh">上海</option>
	          <option value="bj">北京</option>
	          <option value="gz">广州</option>
	        </select>
	        <br/>
	        {/* 复选框 */}
	        <input type="checkbox" checked={this.state.isChecked} onChange={this.handelChecked}/>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 3.6.2 受控组件的多表单元素优化

问题：

1. 每个表单元素都有一个单独的事件处理程序，处理太繁琐
2. 优化：使用一个事件处理程序同时处理多个表单元素

优化步骤：

1. 给表单元素添加name属性，名称与state相同
2. 根据表单元素类型获取对应值
3. 在change事件处理程序中通过[name]来修改对应的state

优化后的代码：

	class App extends React.Component{
	  state={
	    txt:'',
	    content:'',
	    city:'bj',
	    isChecked:false
	  }
	  handleForm=e=>{
	    // 获取当前DOM对象
	    const target=e.target
	    // 根据类型获取值
	    const value=target.type=='checkbox'?target.checked:target.value
	    //获取name
	    const name=target.name
	    this.setState({
	      [name]:e.target.value
	    })
	  }
	
	  render(){
	    return(
	      <div>
	        {/* 文本框 */}
	        <input type="text"  name="txt" value={this.state.txt} onChange={this.handleForm}/>
	        <br/>
	        {/* 富文本框 */}
	        <textarea name="content" value={this.state.content} onChange={this.handleForm}></textarea>
	        <br/>
	        {/* 下拉框 */}
	        <select name="city" value={this.state.city} onChange={this.handleForm}>
	          <option value="sh">上海</option>
	          <option value="bj">北京</option>
	          <option value="gz">广州</option>
	        </select>
	        <br/>
	        {/* 复选框 */}
	        <input name="isChecked" type="checkbox" checked={this.state.isChecked} onChange={this.handleForm}/>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 3.6.3 非受控组件（不推荐使用）

1. 说明：借助与ref，使用原生DOM方式来获取表单元素值
2. ref的作用：获取DOM或组件

使用步骤：

1. 调用React.createRef()方法创建一个ref对象
2. 将创建好的ref对象添加到文本框中
3. 通过ref对象获取到文本框的值

代码：

	constructor(){
	  suoer()
	  this.txtRef=React.createRef()
	}
	<input type="text" ref={this.txtRef} />
	Console.log(this.txtRef.current.value)

示例代码：

	class App extends React.Component{
	  constructor(){
	    super()
	    // 创建Ref
	    this.txtRef=React.createRef()
	  }
	      // 获取文本框的值
	      getTxt=()=>{
	        alert('文本框的值为：'+this.txtRef.current.value)
	      }
	  render(){
	    return(
	      <div>
	        <input type="text" ref={this.txtRef}></input>
	        < button onClick={this.getTxt}>获取文本框的值</button>
	      </div>
	    )
	  }
	}
	// 渲染组件
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 3.7 组件总结

1. 组件的两种创建方式：
     - 函数组件
     - 类组件
2. 无状态组件（函数组件），负责静态结构展示
3. 有状态组件（类组件），负责更新UI，让页面动起来
4. 绑定事件注意this指向问题
5. 推荐使用受控组件来处理表单
6. 完全利用JS语言的能力创建组件，这是React的思想

### 3.8 React组件案例

#### 3.8.1 案例：评论列表

需求分析：

- 渲染评论列表（列表渲染）
- 没有评论数据时渲染：暂无评论（条件渲染）
- 获取评论信息，包括评论人和评论内容
- 发表评论，更新评论列表

**步骤**

1. 渲染评论列表
    - 在state中初始化评论列表数据
    - 使用数组的map方法遍历state中的列表数据
    - 给每个被遍历的li元素添加key属性
2. 渲染暂无评论
	- 判断列表数据的长度是否为0
	- 如果为0，则渲染暂无评论
3. 获取评论信息
	- 使用受控组件方式处理表单元素
4. 发表评论
	- 给按钮绑定单击事件
	- 在事件处理程序中，通过state获取评论信息
	- 将评论信息添加到state中，并调用setState()方法更新state
	- 边界情况：清空文本框
	- 边界情况：非空判断

代码：

	class App extends React.Component{
	    state={
	        comments:[
	            {id:1,name:'a',content:'aa'},
	            {id:2,name:'b',content:'bb'},
	            {id:3,name:'c',content:'cc'}
	        ],
	        // 评论人
	        userName:'',
	        // 评论内容
	        userContent:''
	    }
	    // 渲染评论内容
	    renderList(){
	        if(this.state.comments.length===0){
	            return <div className="no-comment">暂无评论，快去评论吧！</div>
	        }else{
	            return <ul>
	            {this.state.comments.map(item=>(
	            <li key={item.id}>
	            <h3>评论人：{item.name}</h3>
	            <p>评论内容：{item.content}</p>
	            </li>
	            ))}
	        </ul>
	        } 
	    }
	    // 处理表单元素值
	    handleForm=(e)=>{
	        const{name,value}=e.target 
	        this.setState({
	            [name]:value
	        })
	    }
	    // 发表评论事件
	    addComment=()=>{
	        const{comments,userContent,userName}=this.state
	        // 非空校验(去除掉空格后等于空)
	        if(userName.trim()===''||userContent.trim()===''){
	         alert('请输入评论人和评论内容')
	         return 
	        }
	        const newComments=[{
	            id:Math.random(),
	            name:userName,
	            content:userContent
	        },
	        ...comments]
	    // 清空文本框的值，只需要将对应的state清空
	        this.setState({
	            comments:newComments,
	            userName:'',
	            userContent:''
	        })
	    }
	    render(){
	        const {userContent,userName}=this.state
	        return(
	            <div className="app"> 
	              <div>
	                <input className="user" placeholder="请输入评论人" value={userName} name="userName" onChange={this.handleForm}/>
	                <br/>
	                <textarea className="content" rows="10" cols="30" placeholder="请输入评论内容" value={userContent} name="userContent" onChange={this.handleForm}></textarea>
	                <br/>
	                <button onClick={this.addComment}>发表评论</button>
	                </div>
	                {this.renderList()}
	            </div>
	        )
	    }
	}
	// 渲染组件
	ReactDOM.render(<App></App>,document.getElementById('root'))

## 四、React组件进阶

### 4.1 组件的props

1. 组件是封闭的，要接收外部数据应该通过props来实现
2. props的作用：接收传递给组件的数据
3. 传递数据：给组件标签添加属性
4. 接收数据：函数组件通过参数props接收数据，类组件通过this.props接收数据

函数组件接收数据：

	function Hello(props){
	    return(
	        <div>
	            接收的数据：{props.name}
	        </div>
	    )
	}
	ReactDOM.render(<Hello name="jack" age={19}></Hello>,document.getElementById('root'))

类组件接收数据：

	class Hello extends React.Component{
	    render(){
	        return(
	            <div>
	                接收到的数据：{this.props.age}
	            </div>
	        )
	    }
	}
	ReactDOM.render(<Hello name="jack" age={19}></Hello>,document.getElementById('root'))

**特点**

1. 可以给组件传递任意类型的数据
2. props是只读的对象，只能读取属性的值，无法修改对象
3. 注意：使用类组件时，如果写了构造函数，应该将props传递给super()，否则无法在构造函数中获取到props

代码：

	class Hello extends React.Component{
        constructor(props){
          super(props)
     }
	    render(){
	        return(
	            <div>
	                接收到的数据：{this.props.age}
	            </div>
	        )
	    }
	}
	ReactDOM.render(<Hello name="jack" age={19}></Hello>,document.getElementById('root'))

### 4.2 组件通讯的三种方式

**组件之间的通讯分为3种：**

1. 父组件 -> 子组件
2. 子组件 -> 父组件
3. 兄弟组件

#### 4.2.1 父组件传递数据给子组件

1. 父组件提供要传递的state数据
2. 给子组件标签添加属性，值为state中的数据
3. 子组件中通过props接收父组件中传递的数据

代码：

	class Parent extends React.Component{
	    state={lastName:'王'}
	    render(){
	        return(
	            <div className="parent">
	            父组件传递数据给子组件:<Child name={this.state.lastName}></Child>
	        </div>
	        )
	    }
	}
	// 子组件
	function Child(props){
	    return <div className="child">子组件接收到的数据:{props.name}</div>
	}
	ReactDOM.render(<Parent></Parent>,document.getElementById('root'))

#### 4.2.2 子组件传数据给父组件

思路：利用回调函数，父组件提供回调，子组件调用，将要传递的数据作为回调函数的参数

1. 父组件提供一个回调函数（用于接收数据）
2. 将函数作为属性的值，传递给子组件
3. 子组件通过props调用回调函数
4. 将子组件的数据作为参数值传递给回调函数

代码：

	// 父组件
	class Parent extends React.Component{
	    state={
	        parentMsg:''
	    }
	    // 提供回调函数，用来接收数据
	    getChildMsg=(data)=>{
	        alert('接收子组件中传递过来的数据'+data)
	        this.setState({
	            parentMsg:data
	        })
	    }
	    render(){
	        return(
	            <div className="parent">
	            父组件:{this.state.parentMsg}
	            <Child getMsg={this.getChildMsg}></Child>
	            </div>
	        )
	    }
	}
	// 子组件
	class Child extends React.Component{
	    state={ChildMsg:'React'}
	    handleClick=()=>{
	        this.props.getMsg(this.state.ChildMsg)
	    }
	    render(){
	        return(
	            <div>
	            <button onClick={this.handleClick}>点我给父组件传递数据</button>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<Parent></Parent>,document.getElementById('root'))

#### 4.2.3 兄弟组件之间的通讯

1. 将共享状态提升到最近的公共父组件中，由这个公共父组件管理这个状态
2. 思想：状态提升
3. 公共父组件职责：1.提供共享状态 2.提供操作共享的方法
4. 要通讯的子组件只需要通过props接收状态或操作状态的方法

代码：

	// 父组件
	class Counter extends React.Component{
	    // 提供共享状态
	    state={
	        count:0
	    }
	    // 更新修改状态的方法
	    onIncrement=()=>{
	        this.setState({
	            count:this.state.count+1
	        })
	    }
	    render(){
	        return <div>
	            <Child1 count={this.state.count}></Child1>
	            <Child2 onIncrement={this.onIncrement}></Child2>
	        </div>
	    }
	}
	const Child1=(props)=>{
	    return <h1>计数器：{props.count}</h1>
	}
	const Child2=(props)=>{
	    return <button onClick={props.onIncrement}>+1</button>
	}
	ReactDOM.render(<Counter></Counter>,document.getElementById('root'))

### 4.3 Context

**思考：**

App组件（第一层）要传递给Child组件（第四层），该如何处理？

- 处理方式：使用props一层层往下传递（繁琐）

- 更好的方式：
	- 使用Context
	- 作用：跨组件传递数据（比如：主题，语言等）

**使用步骤**

1. 调用React.createContext()创建Provider(提供数据)和Consumer(消费数据)两个组件
`const {Provider,Consumer}=React.createContext()`
2. 使用Provider组件作为父节点
          
	        <Provider>
            <div className="app">
               <Node></Node>
            </div>
            </Provider>
3. 设置value属性，表示要传递的数据
`<Provider value="pick"> </Provider>`
4. 使用Consumer组件接收数据（data为value值）

	      <Consumer>
	          {data=><span>我是子节点--{data}</span>}
	     </Consumer>  

**总结**

1. 如果两个组件是远方亲戚（比如：嵌套多层）可以使用Context实现组件通讯
2. Context提供两个组件：Provider和Consumer
3. Provider组件：用来提供数据
4. Consumer组件：用来消费数据

### 4.3 props深入

#### 4.3.1 children属性

- children属性：表示组件标签的子节点，当组件标签有子节点时，props就会有该属性
- childen属性与普通的props一样，值可以是任意值（文本，React元素，组件，甚至是函数）

代码：(props.children即为Test组件)

	const Test=()=> <button>我是button组件</button>
	const App=(props)=>{
	    return (
	        <div>
	           <h1>
	               组件标签的子节点{props.children}
	           </h1>
	        </div>
	    )
	}
	ReactDOM.render(
	    <App>
	        <Test/>
	    </App>,
	    document.getElementById('root')
	)
代码：(props.children即为函数)

	const App=(props)=>{
	    return (
	        <div>
	           <h1>
	               组件标签的子节点
	              <button onClick={()=>props.children()}>点击</button>
	           </h1>
	        </div>
	    )
	}
	ReactDOM.render(
	    <App>
	        {()=>alert('这是一个函数子节点')}
	    </App>,
	    document.getElementById('root')
	)

#### 4.3.2 props校验

[https://zh-hans.reactjs.org/docs/typechecking-with-proptypes.html](https://zh-hans.reactjs.org/docs/typechecking-with-proptypes.html "使用 PropTypes 进行类型检查")

**问题：**

- 对于组件来说，props是外来的，无法保证组件使用者传入什么格式的数据
- 如果传入的数据格式不对，可能会导致组件内部报错
- 关键问题：组件使用者不知道明确的错误原因

**解决方法：**

- props校验：运行在创建组件的时候，就指定props的类型，格式等
`App.propTypes={colors:PropTypes.array}`
- 作用：捕获使用组件时因为props导致的错误，给出明确的错误提示，增加组件的健壮性

**使用步骤**

1. 安装包props-types(npm i props-types)
2. 导入props-types包
3. 使用组件名.propsTypes={}来给组件的props添加校验规则
4. 校验规则：通过propsTypes对象来指定

props校验：(约定colors属性为array类型，若类型不对则报出明确错误，便于分析错误原因)

	import PropTypes from 'prop-types'
	const App=(props)=>{
	    const arr = props.colors
	    const lis=arr.map((item,index)=> <li key={index}>{item}</li>)
	    return <ul>{lis}</ul>
	}
	// 添加props检验
	App.propTypes={
	    colors:PropTypes.array
	}
	ReactDOM.render(<App colors={['red','blue']}></App>,document.getElementById('root'))

**约束规则**

1. 常见类型：array,bool,func,numder,object,string
2. React元素类型：element
3. 必填项：isRequired
4. 特定结构的对象：shape({})

校验案例：

    //属性a:数值number ，属性fn：函数func并为必填项，
    //属性tag：React元素（element），属性filter：对象({area:'上海',price:1999})
	import PropTypes from 'prop-types'
	const App=(props)=>{
	    return(<div>
	        <h1>
	            props校验：
	        </h1>
	    </div>)
	}
	App.propTypes={
	    a:PropTypes.number,
	    fn:PropTypes.func.isRequired,
	    tag:PropTypes.element,
	    filter:PropTypes.shape({
	        area:PropTypes.string,
	        price:PropTypes.number
	    })
	}
	ReactDOM.render(<App fn={()=>{}}></App>,document.getElementById('root'))

#### 4.3.3 props的默认值

1. 场景：分页组件->每页显示条数
2. 作用：给props设置默认值，在未传入props时生效

代码：

	const App=(props)=>{
	    return(
	    <div>
	        <h1>此处显示props的默认值：{props.pageSize}</h1>
	    </div>
	    )
	}
	// 添加props默认值
	App.defaultProps={
	    pageSize:10
	}
	// 组件中不传入pageSize时则为默认值，传入则为传入值
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 4.4 组件的生命周期

#### 4.4.1 组件的生命周期概述：

- 意义：组件的生命周期有助于理解组件的运动方式、完成更复杂的组件功能、分析组件错误原因等
- 组件生命周期：组件从被创建到挂在到页面中运行，再到组件不用时卸载的过程
- 钩子函数：生命周期的每个阶段总是伴随着一些方法调用，这些方法就是生命周期的钩子函数
- 钩子函数的作用：为开发人员在不同阶段操作组件提供了时机

#### 4.4.2 生命周期的三个阶段

- 创建时（挂在阶段）
	- 执行时机：组件创建时（页面加载时）
	- 执行顺序：constructor()->render()->componentDidMount
	- |钩子函数| 触发时机|作用|
	- |constructor | 创建组件时最先执行 | 1.初始化state 2.为事件处理程序绑定this|
	- |render | 每次组件渲染都会触发 | 渲染UI（注意：不能调用setState()）|
	- |componentDidMount |组件挂载(完成DOM渲染)后 | 1.发送网络请求 2.DOM操作|

代码：

	class App extends React.Component{
	    constructor(props){
	        super(props)
	        // 初始化state
	        this.state={
	            count:0
	        }
	    }
	    // 1. 进行DOM操作 2.发送请求获取数据
	    componentDidMount(){
	      const title=document.getElementById('title')
	      console.log(title)
	    }
	    render(){
	        return (
	            <div>
	                <h1 id="title">统计豆豆被打的次数：</h1>
	                <button id="btn"></button>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

- 更新时（更新阶段）
	- 执行时机：1.setState() 2.forceUpdate() 3.组件接收到的心的props
	- 说明：以上三者任意一种变化，组件就会重新渲染
	- 执行顺序：render()->componentDidUpdate()
	- |钩子函数| 触发时机|作用|
	- |render|每次组件渲染都会触发|渲染UI(与挂载阶段是同一个render())|
	- |componentDidUpdate|组件更新(完成DOM渲染)后|1.发送网络请求 2.DOM操作 注意：如果要setState()必须放在一个if条件中

代码1：

	class App extends React.Component{
	    constructor(props){
	        super(props)
	        // 初始化state
	        this.state={
	            count:0
	        }
	    }
	    //打豆豆
	    handleClick=()=>{
	        // this.setState({
	        //     count:this.state.count+1
	        // })
	
	        // 演示强制更新
	        this.forceUpdate()
	    }
	    render(){
	        return (
	            <div>
	               <Counter count={this.state.count}></Counter>
	                <button onClick={this.handleClick}>打豆豆</button>
	            </div>
	        )
	    }
	}
	class Counter extends React.Component{
	    render(){
	        return <h1>统计豆豆被打的次数：{this.props.count}</h1>
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

代码2：

	class App extends React.Component{
	    constructor(props){
	        super(props)
	        // 初始化state
	        this.state={
	            count:0
	        }
	    }
	    //打豆豆
	    handleClick=()=>{
	     this.setState({
	         count:this.state.count+1
	     })
	    }
	    render(){
	        return (
	            <div>
	               <Counter count={this.state.count}></Counter>
	                <button onClick={this.handleClick}>打豆豆</button>
	            </div>
	        )
	    }
	}
	class Counter extends React.Component{
	    render(){
	        return <h1 id="title">统计豆豆被打的次数：{this.props.count}</h1>
	    }
	    //注意：如果要setState()必须放在一个if条件中
	    // 所以：直接调用setState()更新状态，会导致递归更新
	    componentDidUpdate(prevProps){
	    // 正确做法：比较前后更新的props是否相同，来决定是否重新渲染组件
	    console.log('上一次的props：',prevProps,'，当前props：',this.props)
	    if(prevProps.count!==this.props.count){
	        // this.setState({})
	        //发送ajax请求的代码
	    }
	}
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

- 卸载时（卸载阶段）
	- 执行时机：组件从页面中消失
	- |钩子函数| 触发时机|作用|
	- |componentWillUnmount|组件卸载(从页面消失)|执行清理工作(比如:清理定时器等)|

代码：

	class App extends React.Component{
	        constructor(props){
	        super(props)
	        // 初始化state
	        this.state={
	            count:0
	        }
	    }
	    // 打豆豆
	    handleClick=()=>{
	        this.setState({
	            count:this.state.count+1
	        })
	    }
	    render(){
	        return(
	            <div>
	               {
	                this.state.count>3
	                ? <p>豆豆被打死了</p>
	                :<Counter count={this.state.count}></Counter>
	               }
	                <button onClick={this.handleClick}>打豆豆</button>
	            </div>
	        )
	    }
	}
	class Counter extends React.Component{
	    render(){
	        return <h1>统计豆豆被打次数：{this.props.count}</h1>
	    }
	    componentDidMount(){
	        // 开启定时器
	        this.timeID=setInterval(()=>{
	           console.warn("定时器")
	        },1000)
	    }
	    // 组件卸载的钩子函数
	    componentWillUnmount(){
	        console.warn("生命周期钩子函数：omponentWillUnmoun")
	        // 清理计时器
	        clearInterval(this.timeID)
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 4.5 render-props

#### 4.5.1 render props模式

- 思考：如果两个组件中的部分功能相似或相同，该如何处理
- 处理方式：复用相似的功能（联想函数封装）
- 复用什么：1.state 2.操作state的方法(组件状态逻辑)
- 两种方式：1.render props模式 2.高阶组件(HOC)
- 注意：这两种方式不是鑫的API，而是利用React自身特点的编码技巧，演化而成的固定写法

**思路分析**

- 思路：将复用的state和操作的state的方法封装到一个组件中
- 问题1：如何拿到该组件中复用的state
- 在使用组件时，添加一个值为函数的prop，通过参数来获取（需要组件内部实现）
- 问题2：如何渲染任意的UI？
- 使用该函数的返回值作为要渲染的UI内容（需要组件内部实现）

代码：

	<Mouse render={(mouse)=>(
	  <p>鼠标当前位置{mouse.x},{mouse.y}</p>
	)}/>

**使用步骤**

1. 创建Mouse组件，在组件中提供复用的状态逻辑代码(1.状态 2.操作状态的方法)
2. 将要复用的状态作为props.render(state)方法的参数，暴露到组件外部
3. 使用props.render()的返回值作为要渲染的内容

代码：(获取鼠标位置并打印出)

	class Mouse extends React.Component{
	    // 鼠标位置state
	      state={
	            x:0,
	            y:0
	        }
	    // 鼠标移动事件处理程序
	    handleMouseMove=e=>{
	        this.setState({
	            x:e.clientX,
	            y:e.clientY
	        })
	    }
	    // 监听鼠标移动事件
	    componentDidMount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    render(){
	        return this.props.render(this.state)
	    }
	}
	class App extends React.Component{
	    render(){
	        return (
	            <div>
	                <h1>
	                    render props模式
	                    <Mouse render={(mouse)=>{
	                        return <p>鼠标位置：{mouse.x},{mouse.y}</p>
	                    }}></Mouse>
	                </h1>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 4.5.2 演示Mouse组件的复用

- Mouse组件负责：封装复用的状态逻辑代码(1.状态 2.操作方法—)
- 状态：鼠标坐标(x,y)
- 操作状态的方法:鼠标移动事件
- 传入的render prop负责:使用复用的状态来渲染UI结构

代码：

	import img from './/source//logo192.png'
	class Mouse extends React.Component{
	    // 鼠标位置state
	      state={
	            x:0,
	            y:0
	        }
	    // 鼠标移动事件处理程序
	    handleMouseMove=e=>{
	        this.setState({
	            x:e.clientX,
	            y:e.clientY
	        })
	    }
	    // 监听鼠标移动事件
	    componentDidMount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    render(){
	        return this.props.render(this.state)
	    }
	}
	class App extends React.Component{
	    render(){
	        return (
	            <div>
	                <h1>
	                    render props模式
	                    <Mouse render={(mouse)=>{
	                        return <p>鼠标位置：{mouse.x},{mouse.y}</p>
	                    }}></Mouse>
	                </h1>
	                <Mouse render={mouse=>{
	                    return (
	                        <img
	                        src={img} alt="图标"
	                        style={{
	                            position:'absolute',
	                            top:mouse.y-90,
	                            left:mouse.x-90
	                        }}></img>
	                    )
	                }}>
	
	                </Mouse>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 4.5.3 childern代替render属性

- 注意:并不是该模式叫render props就必须使用名为render的prop，实际上可以使用任意名称的prop
- 把prop是一个函数并告诉组件要渲染什么内容的技术叫:render props模式
- 推荐：使用children代替render属性

代码：

	class Mouse extends React.Component{
	    // 鼠标位置state
	      state={
	            x:0,
	            y:0
	        }
	    // 鼠标移动事件处理程序
	    handleMouseMove=e=>{
	        this.setState({
	            x:e.clientX,
	            y:e.clientY
	        })
	    }
	    // 监听鼠标移动事件
	    componentDidMount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    render(){
	        return this.props.children(this.state)
	    }
	}
	class App extends React.Component{
	    render(){
	        return (
	            <div>
	                <h1>
	                    render props模式
	                    <Mouse>
	                    {mouse=>{
	                        return <p>鼠标位置：{mouse.x},{mouse.y}</p>
	                    }}</Mouse>
	                </h1>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

**代码优化**

1. 推荐：给render props模式添加props校验
   `Mouse.propsTypes={children:PropTypes.func.isRequired}`
2. 应该在组件卸载时解除mousemove事件绑定
   `componentWillUnmount(){window.removeEventListener('mousemove',thishandleMouseMove)}`

代码:

	import PropTypes from 'prop-types'
	class Mouse extends React.Component{
	    // 鼠标位置state
	      state={
	            x:0,
	            y:0
	        }
	    // 鼠标移动事件处理程序
	    handleMouseMove=e=>{
	        this.setState({
	            x:e.clientX,
	            y:e.clientY
	        })
	    }
	    // 监听鼠标移动事件
	    componentDidMount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    // 组件卸载时移除事件绑定
	    componentWillUnmount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    render(){
	        return this.props.children(this.state)
	    }
	}
	// 添加props校验
	Mouse.propTypes={
	    children:PropTypes.func.isRequired
	}
	class App extends React.Component{
	    render(){
	        return (
	            <div>
	                <h1>
	                    render props模式
	                    <Mouse>
	                    {mouse=>{
	                        return <p>鼠标位置：{mouse.x},{mouse.y}</p>
	                    }}</Mouse>
	                </h1>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 4.6 高阶组件

#### 4.6.1 概述

- 目的：实现状态逻辑复用
- 采用包装模式,比如：手机壳
- 手机：获取保护功能
- 手机壳：提供保护功能
- 高阶组件就相当于手机壳，通过包装组件，增强组件功能

**思路分析**

- 高阶组件(HOC)是一个函数，接收要包装的组件，返回增强后的组件
`const EnhancedComponent=withHOC(WrappedComponent)`
- 高阶组件内部创建一个类组件，在这个类组件中提供复用的状态逻辑代码，通过prop将复用的状态传递给
- 被包装组件WrappedComponent

**使用步骤** 

1. 创建一个函数，名称以with开头
2. 指定函数参数，参数应该以大写字母开头(作为要渲染的组件)
3. 在函数内部创建一个类组件，提供复用的状态逻辑代码，并返回
4. 在该组件中，渲染参数组件，同时将状态通过prop传递给参数组件
5. 调用该高阶组件，传入要增强的组件，通过返回值拿到增强后的组件，并将其渲染到页面中

示例代码：

	fucntion withMouse(WrappedComponent){
	    class Mouse extends React.Component{
	        render(){
	            return <WrappedComponent {...this.state}></WrappedComponent>
	        }
	    }
	    return Mouse
	}

代码：

	import img from './/source//logo192.png'
	function withMouse(WrappedComponent){
	    // 该组件提供复用状态逻辑
	    class Mouse extends React.Component{
	    //    鼠标状态
	    state={
	        x:0,
	        y:0
	    }
	    handleMouseMove=e=>{
	        this.setState({
	            x:e.clientX,
	            y:e.clientY
	        })
	    }
	    // 控制鼠标状态的逻辑
	    componentDidMount(){
	        window.addEventListener('mousemove',this.handleMouseMove)
	    }
	    // 组件卸载时解绑事件
	    componentWillUnmount(){
	        window.removeEventListener('mousemove',this.handleMouseMove)
	    }
	    render(){
	        return <WrappedComponent {...this.state}></WrappedComponent>
	    }
	 }
	 return Mouse
	}
	const Mouse = props =>(
	   <p>
	        鼠标位置: ({props.x},{props.y})
	  </p>
	)
	const Logo=props=>(
	     <img
	        src={img} alt="图标"
	        style={{
	            position:'absolute',
	            top:props.y-90,
	            left:props.x-90
	        }}></img>
	)
	// 获取增强后的组件,调用高阶组件函数
	const MousePosition=withMouse(Mouse)
	const LogoPosition=withMouse(Logo)
	class App extends React.Component{
	    render(){
	        return (
	            <div>
	                <h1>高阶组件</h1>
	                <MousePosition></MousePosition>
	                <LogoPosition></LogoPosition>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 4.6.2 设置displayName

高阶组件的displayName

- 使用高阶组件存在的问题：得到的两个组件名称相同
- 原因：默认情况下，React使用组件名称作为displayName
- 解决方式：为高阶组件设置displayName便于调试时区分不同的组件
- displayName的作用：用于设置调试信息(React Developer Tools信息)

设置方式：(在高阶函数中编写)

	Mouse.displayName=`WithMouse${getDisplayName(WrappedComponent)}`
	 return Mouse
	}

单独编写：

	function getDisplayName(WrappedComponent){
	    return WrappedComponent.displayName||WrappedComponent.name||'Component'
	}

#### 4.6.3 传递props

- 问题：props丢失
- 原因：高阶组件没有往下传递props
- 解决方式：渲染WrappedComponent时，将state和this.props一起传递给组件
- 传递方式：
`<WrappedComponent {...this.state}{...this.props}></WrappedComponent>`

### 4.7 React组件进阶总结

1. 组件通讯是构建React应用必不可少的一环
2. props的灵活性让组件变得更加强大
3. 状态提升是React组件的常用模式
4. 组件生命周期有助于理解组件的运行过程
5. 钩子函数让开发者可以在特定的实际执行某种功能
6. render props模式和高阶组件可以实现组件状态逻辑复用
7. 组件的极简模型：`(state,props)=>UI`

## 五、React原理

### 5.1 学习目标

- 知道setState()更新数据是异步的
- 知道JSX语法的转化过程
- 能说出React组件的更新机制
- 能够对组件进行性能优化
- 能够说出虚拟DOM和Diff算法

### 5.2 setState()说明

#### 5.2.1 更新数据与推荐语法

- setState()是异步更新数据的(更新数据后不立即改变)
- 注意：一个函数中多次使用setState(),后面setState不依赖于前面的setState
- 可以调用多次setState，合并后，只会触发一次渲染(render)

**推荐语法**

- 推荐： 使用`setState((state,props)=>{})`语法
- 参数state：表示最新的state
- 参数props：表示最新的props

#### 5.2.2 setState的第二个参数

- 场景：在状态更新(页面完成重新渲染)后立即执行某个操作
- 语法：setState(updater[,callback])

示例代码：

	this.setState(
          (state,props)=>{
              return {
                  count:state.count+1
              }
          },
        //  状态更新后并且重新渲染后立即执行： 
          ()=>{ 
            console.log('状态更新完成',this.state.count)
        })

### 5.3 JSX语法的转化过程

- JSX仅仅是createElement()方法的简化语
- JSX语法被@bable/preset-react插件编译为createElement()方法
- 转化过程：JSX语法->createElement()->React元素
- React元素：是一个对象，用来描述你希望在屏幕上看到的内容

### 5.4 组件更新机制

- setState()两个作用：1.修改state 2.更新组件(UI)
- 过程：父组件重新渲染时，也会重新渲染子组件，但是只会渲染当前组件子树(当前组件及其所有子组件和后代组件)

### 5.5 组件性能优化

#### 5.5.1 减轻state

- 减轻state：只存储组件渲染相关的数据(比如:count/列表数据/loading等)
- 注意：不用做渲染的数据不要放在state中，比如定时器的id等
- 更渲染无关的数据，需要在多个方法中用到的数据，应该放在this中

#### 5.5.2 避免不必要的重新渲染

- 组件更新机制：父组件更新会引起子组件也被更新，这种思路很清晰
- 问题：子组件没有任何变化时也会重新渲染
- 如何避免不必要的更新渲染呢？
- 解决问题：使用钩子函数
`shouldComponentUpdate(nextProps,nextState)`
- 作用：通过返回值决定该组件是否重新渲染，返回true表示重新渲染，false表示不重新渲染
- 触发时机：更新阶段的钩子函数，组件重新渲染前执行(shouldComponentUpdate->render),若返回false，则render不执行
- nextState为最新的状态，this.state为更新前的状态

钩子函数：

shouldComponentUpdate(nextProps,nextState){
   //最新的状态
   console.log('最新的state',nextState)
   //更新前的状态
   console.log('this.state',this.state)
   return true
}

**案例**

随机数案例代码(通过state阻止相同值的更新)：

	class App extends React.Component{
	    state={
	       number:0
	    }
	    handleClick=()=>{
	        this.setState(()=>{
	            return {
	                number:Math.floor(Math.random()*3)
	            }
	        })
	    }
	    // 因为两次生成的随机数相同，如果相同则不需要重新渲染
	    shouldComponentUpdate(nextProps,nextState){
	        console.log('最新状态：',nextState,'当前状态：',this.state)
	            return nextState.number!==this.state.number
	    }
	    render(){
	        console.log('render')
	        return (
	            <div>
	                <h1>随机数：{this.state.number}</h1>
	                <button onClick={this.handleClick}>生成随机数</button>
	            </div>
	        )
	    }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

随机数案例代码(通过props阻止相同值的更新)： 

	class App extends React.Component{
	    state={
	       number:0
	    }
	    handleClick=()=>{
	        this.setState(()=>{
	            return {
	                number:Math.floor(Math.random()*3)
	            }
	        })
	    }
	    // 因为两次生成的随机数相同，如果相同则不需要重新渲染
	    // shouldComponentUpdate(nextProps,nextState){
	    //     console.log('最新状态：',nextState,'当前状态：',this.state)
	    //         return nextState.number!==this.state.number
	    // }
	    render(){
	        return (
	            <div>
	               <NumberBox number={this.state.number}></NumberBox>
	                <button onClick={this.handleClick}>生成随机数</button>
	            </div>
	        )
	    }
	}
	class NumberBox extends React.Component{
	    shouldComponentUpdate(nextProps){
	        console.log('最新props：',nextProps,'更新的前props：',this.props)
	        return nextProps.number!==this.props.number
	    }
	   render(){
	    console.log('子组件的render')
	    return <h1>随机数：{this.props.number}</h1>
	   }
	}
	ReactDOM.render(<App></App>,document.getElementById('root'))

#### 5.5.3 纯组件

- 说明：纯组件内部的对比是shallow compare(浅层对比)
- 对比值类型来说：比较两个值是否相同(直接赋值即可，没有坑)
- 对于引用类型：只比较对象的引用(地址)是否相同
- 主要：state或props中属性值为引用类型时，一应该创建新数据，不要直接修改原数据！

示例代码：

    //创建新数据，newObj为obj的副本，并更改number的值
	const newObj={...this.state.obj,number:1}
    //把新数据赋值给obj
	this.setState(()=>{
	    return {
	        obj:newObj
	    }
	})

**创建新数据的方法**

- 不要使用数组的push/unshift直接修改当前数组的方法
- 应该使用concat或slice这些返回新数组的方法

代码：

	this.setState({
		list:[...this.state.list,{新数据}]
	})

### 5.6 虚拟DOM和Diff算法

- React更新视图的思想是：只要state变化就重新渲染视图
- 特点：思路非常清晰
- 问题：组件只有一个DOM元素需要更新时，也得把整个组件的内容重新渲染到页面中吗？ （不是）
- 理想状态：部分更新，只更新变化的地方
- 问题：React是如何做到部分更新的？ 使用虚拟DOM配合Diff算法

虚拟DOM：本质上就是一个JS对象，用来描述你希望在屏幕上看到的内容(UI)

**执行过程**

1. 初始渲染时，React会根据初始state，创建一个虚拟DOM对象
2. 根据虚拟DOM生成真正的DOM,渲染到页面中
3. 当前数据变化后(setState())，重新根据新的数据，创建新的虚拟DOM对象
4. 与上次得到的虚拟DOM对象，使用Diff算法对比，得到需要更新的内容
5. 最终，React只需将变化的内容更新(patch)到DOM中，重新渲染到页面
6. 组件render()调用后，并不意味着浏览器中的重新渲染！仅仅说明要进行diff，根据状态和JSX结构生成虚拟DOM对象

### 5.7 React原理总结

1. 工作角度：应用第一，原理第二
2. 原理有助于更好理解React的自身运行机制
3. setState()异步更新数据
4. 父组件更新导致子组件更新，纯组件提升性能
5. 思路清晰简单为前提，虚拟DOM和Diff保效率
6. 虚拟DOM->state+JSX
7. 虚拟DOM的真正价值从来都不是性能，最大价值让浏览器脱离了React环境的束缚

## 六、React路由

### 6.1 React路由介绍

现代的前端应用大多都是SPA(单页面应用程序)，也就是只有一个HTML页面的应用程序，因为它的用户体验更好，对服务器的压力更小，所以更受欢迎，为了有效的使用单个页面来管理原来多页面的功能，前端路由应运而生。

-前端路由的功能：让用户从一个视图(页面)导航到另一个视图(页面)
- 前端路由是一套隐射规则，在React中，是URL路径与组件的对应关系
- 使用React路由简单来说，就是配置路径和组件(配对)

### 6.2 路由的基本使用

**使用步骤** 

1. 安装：`yarn add react-router-dom`
2. 导入路由的三个核心组件：Router/Route/Link
`import {BrowserRouter as Router,Route,Link} from 'react-router-dom'`
3. 使用Router组件包裹整个应用(重要)
4. 使用Link组件作为导航菜单(路由入口)
`<Link to="/first">页面一</Link>`
5. 使用Router组件配置路由规则和要展示的组件(路由出口)

代码：(点击路由入口，则显示出路由出口)

	import {BrowserRouter as Router,Route,Link} from 'react-router-dom'
	const First=()=>(
	    <p>页面一的内容</p>
	)
	const App=()=>(
	    // 使用Router组件包裹整个应用
	    <Router>
	        <div>
	            <h1>React路由基础</h1>
	            {/* 指定路由入口 */}
	            <Link to="/first">页面一</Link>
	            {/* 指定路由出口 */}
	            <Route path="/first" component={First}></Route>
	        </div>
	    </Router>
	)
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 6.3 常用组件说明

- Router组件:包裹整个应用，一个React应用只需要使用一次
- 两种常用的Router:HashRouter和BrowserRouter
- HashRouter:使用URL的哈希值实现(localhost:3000/#/first)
- (推荐)BrowserRouter:使用H5的history API实现(localhost:3000/first)
- Link组件：用于指定导航链接(a标签)，to属性为浏览器地址栏中的pathname(location.pathname)
`<Link to="/first">页面一</Link>`
- Route组件:指定路由展示组件相关信息，path属性为路由规则，component属性为展示的组件，Route组件写在哪里渲染出来的组件就展示在哪
`<Route path="/first" component={First}></Route>`

### 6.4 路由的执行过程

1. 点击Link组件(a标签)，修改了浏览器地址栏中的url
2. React路由监听到地址栏url的变化
3. React路由内部遍历所有Route组件，使用路由规则(path)与pathname进行匹配
4. 当路由规则(path)能够匹配地址栏中的pathname时，就展示该Route组件的内容

### 6.5 编程式导航

- 场景：点击登入按钮，登入成功后，通过代码跳转到后台首页，如何实现？
- 编程式导航：通过JS代码来实现页面跳转
- history是React路由提供，用于获取浏览器记录的相关信息
- push(path):跳转到某个页面，参数path表示要跳转的路径
- go(n):前进或者退后某个页面，参数n表示前进或后退页面数量(比如:-1表示后退到上一页)

代码：

	import {BrowserRouter as Router,Route,Link} from 'react-router-dom'
	class Login extends React.Component{
	    handleLogin=()=>{
	        // 使用编程式导航实现路由跳转
	        this.props.history.push('/home')
	    }
	    render(){
	        return (
	            <div>
	                <p>登入页面</p>
	                <button onClick={this.handleLogin}>登录</button>
	            </div>
	        )
	    }
	}
	const Home =(props)=>{
	    const handleBack=()=>{
	        // 表示返回上一个页面
	       props.history.go(-1)
	    }
	    return(
	    <div>
	        <h1>后台首页</h1>
	        <button onClick={handleBack}>返回登入页面</button>
	    </div>)
	}
	const App=()=>(
	    <Router>
	    <div>
	        <h1>编程式导航</h1>
	        <Link to="/login">登入页面</Link>
	        <Route path="/login" component={Login}></Route>
	        <Route path="/home" component={Home}></Route>
	    </div>
	    </Router>
	)
	ReactDOM.render(<App></App>,document.getElementById('root'))

### 6.6 默认路由

- 问题：现在的路由都是点击导航菜单后展示的，如何在进入页面的时候就展示呢？
- 默认路由：表示进入页面时就会匹配的路由
- 默认路由path为:/   
`<Router path="/ component={Home} />`

### 6.7 匹配模式

#### 6.7.1 模糊匹配模式

- 问题：当Link组件的to属性值为:"/login"时，为什么默认路由也被匹配成功(默认路由还显示在页面中)？
- 默认情况下，React路由是模糊匹配模式
- 模糊匹配规则，只要pathname以path开头就会匹配成功
- 当path为"/"，都能匹配所有的pathname

#### 6.7.2 精确匹配模式

- 问题：默认路由任意情况下都会展示，如何避免这种问题？
- 给Route组件添加excat属性，让其变为精确匹配模式
`<Route exact path="/" component={Home}>`

### 6.8 React路由基础总结

1. React路由可以有效的管理多个视图(组件)实现SPA
2. Router包裹整个应用，只需要使用一次
3. Link组件是入口，Route组件是出口
4. 通过props.history实现编程式导航
5. 默认模糊匹配，添加exact变精确匹配
6. React路由的一切都是组件，可以像思考组件一样思考路由
