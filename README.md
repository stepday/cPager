# cPager
基于jQuery的客服端分页插件cPager.js，分页展示美观大气，结合CSS3.0的呈现美化效果

### 安装

clone项目地址
git clone https://github.com/stepday/cPager.git

<pre>
	-|
	 |-index.html  demo演示页面
	 |-js
	   |-template.js js模板引擎 用于快速渲染页面列表的
	   |-cPager.js   基于jQuery封装的客户端分页插件
	 |-css
	   |-cPager.css  分页插件相关样式文件
</pre>

### 插件引入步骤
1、head头内引入cPager.css 样式文件;<br/>
2、head头内引入jquery.js 脚本文件；<br/>
3、head头内引入cPager.js 脚本文件；<br/>
4、页面内设置分页容器:
<pre>
<div class="turn-page" id="pager"></div>
</pre>
5、调用插件
<pre>
	$(this).cPager({
        pageSize: 8, //每一页显示的记录条数
        pageid: "pager", //分页容器ID
        itemClass: "li-item" //个体元素名称
    });
</pre>

### 插件优点
1、支持分页每一页显示的记录条数；<br/>
2、支持分页容器的配置；<br/>
3、支持个体元素的样式标记配置；<br/>
4、自动提取数据进行元素总数和总页数的计算；

示例代码如下：
<pre>
	//调用客户端分页
    $(this).cPager({
        pageSize: 8, //每一页显示的记录条数
        pageid: "pager", //分页容器ID
        itemClass: "li-item" //个体元素名称
    });
</pre>

### 插件缺点
为了页面展示不闪屏，建议默认列表渲染的时候，所有个体元素为隐藏模式(display:none)

