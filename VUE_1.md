# P1 入门

MVC模式——Model(数据)，VIEW(用户视图)，Controller(控制器作数据处理)

DOM文件——包括HTML，CSS和JS的目录结合

MVVM模式——Model，View，View，Model模式

VUE基于MVVM模式。



用HBuilderX创建Vue项目，根据官网教程写入门程序：

```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8" />
		<title></title>
		<script src="js/vue.js" type="text/javascript" charset="utf-8"></script>
	</head>
	<body>
		<div id = "app">
			{{title}}
			<h3>{{msg}}</h3>
		</div>
		<!-- <div id = "app2">
			<h3>{{msg2}}</h3>
		</div> -->
		
		<script type="text/javascript">
			let app = new Vue({
				el:"#app",
				data:{
					title:"Hello Vue!",
					msg:"VUE study"
				},
			})
			console.log(app);
		</script>
	</body>
</html>

```

View就是id为app的div，展示在前端页面；Model就是JS中的app的Vue对象，赋值给title和msg数据；剩下的VM由Vue完成。这就是Vue的MVVM模式。



Vue的另一个特点——双向绑定：在HTML界面上右键“检查”，由于```console.log(app)```输出的Vue对象可以在```console控制台```看到，然后可以输入```app.title```更改title数据。



程序先扫描到title，然后会发现vue对象然后赋值——这样效率低下，有脚手架Vue-cli打包完成，以后学。





# P2 条件渲染



