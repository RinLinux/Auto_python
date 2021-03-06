# Borg 的scrapy爬虫、python数据清洗、R语言可视化项目  
+ Forked from: https://github.com/BigBorg/Scrapy-playground

抓取python招聘信息，获取经纬度，经纬度还需要进一步转换成国际标准，最后在地图上可视化。
最后产出的R语言写的可视化报告：
因为html文件比较大，两兆多，github网站国内网速又不是很快，如果加载过慢可以用[七牛外链](http://7xshuq.com1.z0.glb.clouddn.com//githubrepo/scrapy/RAnalysis.html)，还可通过[rpub](http://rpubs.com/Borg/208385)访问，后续更新可能不会更新七牛和rpub，代码仓库内 R-visualization 文件夹下的html文件会是最新版本。


大致可视化效果截图如下：  
1. ggplot的条形图，用ggplotly后可交互，即可放大缩小、拖拽，鼠标悬停在条形图上还会显示具体的数据。
![bar](./R-visualization/img/bar.png)
2. plotly的scatergeo图，圆圈大小代表数据大小，经过根号调整过大小，不然差距太大，小圆圈全都被覆盖了。右侧的四分位点击后是可以隐藏或者显示特定颜色的圆圈的。还有鼠标悬停在圆圈上同样会显示详细信息。plotly做可视化还是很好的，就是有些图片只有美国可以细分到州，其它国家没有。
![geo](./R-visualization/img/geo.png)
3. leaflet地图显示每一个招聘信息的位置，点击后有职位名称和公司名称，职位名称还是个链接。
![leaflet](./R-visualization/img/leaflet.png)  
