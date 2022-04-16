### Welcome to Book ！

 <p align="left">
 	<img src='https://img.shields.io/github/workflow/status/Obsoletes/Maybe/.NET Core'>
 	<img src='https://img.shields.io/nuget/v/Observer.Maybe.svg'>
 </p>
* 均来自网络收集与自行整理

 ### Feature 

 ========================= 

 @@ -15,11 +15,11 @@ Feature
 - 支持捕获异常
 - 支持 C# 8 的 `switch` 模式匹配

 Api
 ## Api

 ========================

 	```C#
 	```
 	public bool HasValue { get; }
 	public bool HasException { get; }
 	public Exception? InnerException { get; }
 @@ -31,15 +31,17 @@ Api
 	public Maybe<T> Or(T obj);
 	```

 Install
 ## Install

 	dotnet add package Observer.Maybe 
 	or

 or

 	Install-Package Observer.Maybe

 Usage
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
