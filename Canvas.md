# HTML5 Canvas API
	用代码绘制图形
	使用Canvas绘制出的图形是位图，依赖于分辨率
	之前是flash完成
	html5 canvas 用canvas来制作游戏
# 使用canvas API
<canvas></canvas>
	使用canvas绘制图形图像，我们需要结合借助javascript中canvas的接口来完成绘制
	标签属性 class/id/style/title/
			 width/height 默认宽高为300px*150px
			 注意：1，通过width height属性方式设置宽高
			 	   2，通过css样式设置canvas宽高
			 	   但是，这两者设置宽高是有区别的
	除IE6-8之外大部分浏览器都支持
	解决兼容问题：1，<canvas> 您的浏览器不支持，请升级最新浏览器</canvas>
				  2，使用js库：<!-- [if] -->
	1,获取绘图环境对象
		绘制环境对象.getContext("2d");
		var o=绘制环境对象.getContext("2d");
		颜色
		坐标系统

	2,绘制方法
		矩形API
		-绘制填充矩形
			o.fillRect(x,y,width,height);-填充（无描边）
			o.fillStyle="color";---填充的颜色
			o.fillRect()==o.rect(x,y,width,height)+o.fill()
		-绘制描边矩形
			o.strokeRect(x,y,width,height);-无填充（描边）
			o.strokeStyle="color"---描边的颜色
			o.strokeRect()==o.rect()+o.stroke()