### Welcome to Book ！

 <p align="left">
 	<img src='https://img.shields.io/github/workflow/status/Obsoletes/Maybe/.NET Core'>
 	<img src='https://img.shields.io/nuget/v/Observer.Maybe.svg'>
 </p>
 
 
 * 均来自网络收集与自行整理


 #### 简介
  ```
  - 支持Book的epub自制书籍
  - 不局限于单一风格图书
  ```
  
 #### Api
![](http://pic.caigoubao.cc/590732/%E5%A4%A7%E4%BA%8C%E4%B8%8B/%E4%BB%99%E8%8D%89/%E6%9C%9F%E4%B8%AD/img2.png)

 	
 	```
 	public bool HasValue { get; }
 	public bool HasException { get; }
 	public Exception? InnerException { get; }


 ## Install

 	dotnet add package Observer.Maybe 
 	or

 or

 	Install-Package Observer.Maybe

 
 ## Usage

 	```C#
 	```
 	Maybe<string> maybe = "123456";
 	var testObj = maybe.Then(s => s.Substring(0, 3));
 	var result = testObj switch
 @@ -49,7 +51,11 @@ Usage
 	};
 	```

 ChangeLog
 ## ChangeLog

 	**1.0** 2020-3-18
 	基本实现
 	基本实现

 ## License

 [MIT](LICENSE) © Richard Littauer
 
 
 
