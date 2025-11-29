第一步：安装pyecharts
pip install pyecharts
第二步：复制粘贴下面代码
python -c "from pyecharts import options as opts; from pyecharts.charts import Map; import webbrowser; Map(init_opts=opts.InitOpts(width='1500px', height='700px')).add('数据示例', [('北京',300),('上海',400),('广东',500),('江苏',450),('浙江',420),('四川',380)], 'china', zoom=1.5, center=[105.0, 35.0]).set_global_opts(title_opts=opts.TitleOpts(title='中国省级数据地图', pos_top='5%'), visualmap_opts=opts.VisualMapOpts(max_=500, pos_bottom='5%')).render('china_province_map.html'); webbrowser.open('china_province_map.html')"
