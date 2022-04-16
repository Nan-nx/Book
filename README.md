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
 
 
 
 
 # MyMusic
 现代操作系统应用开发期中课程设计
 MyMusic 0.5 版本新鲜出炉，人生一大错觉，总觉得项目就快打好了。。。༼ ಥل͟ಥ ༽

 首先，首页已经做好了：

 ![](http://pic.caigoubao.cc/590732/%E5%A4%A7%E4%BA%8C%E4%B8%8B/%E4%BB%99%E8%8D%89/%E6%9C%9F%E4%B8%AD/img1.png)

 是不是很帅，，，＼（＠￣∇￣＠）／

 首先，侧边栏的响应已经做好了，除了点击**发现音乐**之外，其他的界面都会跳转到BlankPage，你们需要在MainPageViewModel.cs文件中更改为需要跳转到的页面：

 ![](http://pic.caigoubao.cc/590732/%E5%A4%A7%E4%BA%8C%E4%B8%8B/%E4%BB%99%E8%8D%89/%E6%9C%9F%E4%B8%AD/img2.png)

 然后，整个页面的结构主要是一个侧边栏，中间一个ContentFrame，下面一个PlayingBar

 然后你们做的基本应该是把你们的页面放在ContentFrame，所以，你们换ContentFrame里的内容为你们的内容的方法：

 1. 先获取一个ContentFrameViewModel单例

 ```c++
 private ContentFrameViewModel ContentFrameVm = ContentFrameViewModel.GetInstance();
 ```
 
