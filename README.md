# Promise_study
TECHF5VE暑假活动之Promise实现  

## 什么是Promise
Promise对象用于表示一个异步操作的最终完成(或失败)及其结果值。 

## Promise理解 
1、抽象表达：它是JS中进行异步编程的新的解决方案  
2、具体表达：（1）从语法上说，Promise是一个构造函数  
　　　　　　　（2）从功能上说，promise对象用来封装一个异步操作并可以获取其结果  

## promise的状态
有三种状态：pending、resolved、rejected   
状态的改变只有两种：pending=>resolved  
　　　　　　　　　　 pending=>rejected  
一个promise对象的状态只能改变一次，无论成功失败，都会有一个结果数据，成功的结果数据一般称为value，失败的一般称为reason  

## 为什么要用Promise
1、指定回调函数的方法更灵活  
旧的方法必须在启动异步任务之前指定回调函数    
promise：启动异步任务=>返回promise对象=>给promise对象绑定回调函数（可在异步任务结束后指定）  
2、支持链式调用，可以解决回调地狱问题  

