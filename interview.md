

#### js模块化规范
 1. CommonJS
  module.exports = {} 对外输出
  require() 读取文件

 2. AMD 
  加载模块：require([module], function(module){})；
  定义模块：define([module], function(module){})； module为依赖模块；

 3. CMD
  define(function(require, exports, module){
   var a = require('a');
   a.foo();
  };

 4. UMD 通用模块定义规范 它可以通过 运行时或者编译时 让同一个代码模块在使用 CommonJs、CMD 甚至是 AMD 的项目中运行
 5. ES6 模块
   import { a } from './module-a'
   export a
