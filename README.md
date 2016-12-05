# ng-route-require

> ngRoute指令的装饰器，可以在ngRoute对template进行编译之前，对template中的js资源进行加载，当资源都加载完毕之后，在调用原有编译流程

##### 使用

由于依赖oclazyload，所以在单页应用入口处先加载oclazyload资源，然后加载装饰器文件，最后加载应用文件，如下：

```
<script type="text/javascript" src="./lib/ocLazyLoad.js"></script>
<script type="text/javascript" src="./lib/ng-router-require.js"></script>
<script type="text/javascript" src="./index.js"></script>
```