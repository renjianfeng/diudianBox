# Diudian-Box 丢点盒子模型

![image](http://www.diudian.com/image/logo.png)

##更适合中国WEB前端生态的布局CSS
###完美兼容ie8、火狐、chrome等国内双核浏览器！

###开始使用

####方法1.在页面上通过css引入
```html  
  <link rel="stylesheet" href="css/diudian.css">
```
####方法2.通过SASS @import到你的.scss文件
```css  
  @import "diudian.scss";
```

###布局介绍

####左右弹性模型
#####使用范围最广的模型，适合单行中有固定和弹性适应的排版，单元格中有一列或多列，以固定宽度（宽度自己设置）固定，其余部分填充铺满
demo
```html  
		<div class="row-cell">
            <div class="col-ela" style="width: 300px"><div class="test">col-ela固定宽度部分( style="width: 300px")</div></div>
            <div class="col-ela"><div class="test">col-ela弹性宽度部分</div></div>
        </div>
        <div class="row-cell">
            <div class="col-ela"><div class="test">col-ela弹性宽度部分</div></div>
            <div class="col-ela" style="width: 300px"><div class="test">col-ela固定宽度部分( style="width: 300px")</div></div>
        </div>
        <div class="row-cell">
            <div class="col-ela" style="width: 300px"><div class="test">col-ela固定宽度部分( style="width: 300px")</div></div>
            <div class="col-ela"><div class="test">col-ela弹性宽度部分</div></div>
            <div class="col-ela" style="width: 300px"><div class="test">col-ela固定宽度部分( style="width: 300px")</div></div>
        </div>
```
弹性效果
![image](http://www.diudian.com/image/btth3.gif)

####表格布局模型
#####类似于table中的td标签，同列中的多个子栏目永不换行，如果单行列数之和超过12（col-列数），超出12个之后的被压缩至最小宽度，如果单行列数之和少于12（col-列数），将重新按照比例分配宽度，确保当前行铺满！。
demo
```html  
	 <div class="row-cell">
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
    </div>
```
弹性效果
![image](http://www.diudian.com/image/btth1.gif)


####栅格布局模型
#####经典的平铺模型，当页面单元的列数总和多于12列（col-列数）时，超出单元自动换行。当页面单元的列数总和少于12列（col-列数）时，页面子单元则右侧留出所缺少的部分！
demo
```html  
	 <div class="row-body">
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
        <div class="col-1"><div class="test">col-1</div></div>
    </div>
```
弹性效果
![image](http://www.diudian.com/image/btth2.gif)
