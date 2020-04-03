    iplot(kind='scatter', data=None, layout=None, filename='', sharing=None, 
          title='', xTitle='', yTitle='', zTitle='', theme=None, colors=None, 
          colorscale=None, fill=False, width=None, dash='solid', mode='lines', 
          interpolation='linear', symbol='circle', size=12, barmode='', 
          sortbars=False, bargap=None, bargroupgap=None, bins=None, histnorm='', 
          histfunc='count', orientation='v', boxpoints=False, annotations=None, 
          keys=False, bestfit=False, bestfit_colors=None, mean=False, mean_colors=None, 
          categories='', x='', y='', z='', text='', gridcolor=None, zerolinecolor=None, 
          margin=None, labels=None, values=None, secondary_y='', secondary_y_title='', 
          subplots=False, shape=None, error_x=None, error_y=None, error_type='data', 
          locations=None, lon=None, lat=None, asFrame=False, asDates=False, 
          asFigure=False, asImage=False, dimensions=None, asPlot=False, asUrl=False, 
          online=None, **kwargs)
    
    通用参数
         kind    图表类型,
                 默认为scatter, 可以选择 (scatter, bar, box, spread, ratio
                 heatmap, surface, histogram, bubble, bubble3d, scatter3d       
                 scattergeo, ohlc, candle, pie, choroplet)中的其中一种
    
         mode    trace(s)的形状样式
                 dict, list or string, 默认为'lines'
                 1. string : applies to all traces
                 2. list : applies to each trace in the order specified
                 3. dict: {column:value} for each column in the dataframe
                                                       
                 Plotting mode for scatter trace
                         lines
                         markers
                         lines+markers
                         lines+text
                         markers+text
                         lines+markers+text
    
                  什么是trace ?
                  "A trace is just the name we give a collection of data and the 
                  specifications of which we want that data plotted. Notice that 
                  a trace will also be an object itself, and these will be named 
                  according to how you want the data displayed on the plotting surface."
    
         theme    布局主题 
                  ['ggplot', 'pearl', 'solar', 'space', 'white',  'polar', 'henanigans']其中之一
    
         title    图表标题
    
         x        包含x轴数值的列名, 字符串
               
         y        包含y轴数值的列名, 字符串
    
         z        包含z轴数值的列名, 字符串
                                       
         xTitle   x轴的坐标轴标签
    
         yTitle   y轴的坐标轴标签
    
         zTitle   z轴的坐标轴标签
    
         colors   颜色
                  可以为dict, list 或 string
                  - dict， {key:color} to specify the color for each column
                  - list，[colors] to use the colors in the defined order
                  
    
         colorscale : string, Color scale name
                          If the color name is preceded by a minus (-) , then 
                          the scale is inversed
                          Only valid if 'colors' is null
                          See cufflinks.colors.scales() for available scales
    
         text     包含文本值的列名, 字符串
    
         secondary_y        在右边y轴上绘制的列的列名, 字符串或列表(可以为多个)
    
         secondary_y_title  第二y轴的轴标签
    
         subplots   是否将每个trace都绘制为子图
                    bool型， 默认为Fasle
    
         shape      subplots的布局 
                    值为行数和列数组成的元组, (rows,cols), 如果省略会自动设置  
                    * Only valid when subplots=True
    
         asFigure   是否返回一个plotly Figure对象
                    布尔值, 默认为False
