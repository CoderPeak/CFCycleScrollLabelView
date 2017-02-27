# CFCycleScrollView (交流QQ 545486205)
### 简单好用的, 走马灯效果, 自动循环(水平/竖直方向)逐条无限循环滚动的控件  

### 因为cell可以自定义---实现仅文字/仅图片/文字+图片等样式, 因此将项目名改为 CFCycleScrollView 

### 注: 竖直方向滚动为 单行逐条滚动 单行逐条滚动 单行逐条滚动

##### 暂未支持pod导入 
##### 因为此需求通常定制性较强, 自定义---可以实现仅文字/仅图片/文字+图片等样式, 为了迎合不同需求, 建议拖入项目中使用

### demo展示 - 由于网络原因, 可能gif效果图会展示的比较卡, 可以下载运行查看demo---简单使用代码

### 使用
- 创建使用仅需几行代码即可

```
    // 提供的数据源 - 通常为网络请求到的数据
    NSMutableArray *dataSource = [NSMutableArray array];
    for (NSInteger i = 0; i < 9; i++) {
        [dataSource addObject:[NSString stringWithFormat:@"显示一行 展示demo数据---%zd", i]];
    }
   // 创建  需提供 frame/数据源/展示的行数
   CFCycleScrollView *cycleScrollView = [CFCycleScrollView cycleScrollViewWithFrame:CGRectMake(0, 230, CFScreenWidth, 66) dataSourceArray:self.dataSource showLabelCount:1];
    // 水平方向 (不设置 默认竖直方向滚动)
   cycleScrollView.scrollDirection = UICollectionViewScrollDirectionHorizontal;
   [self.view addSubview:cycleScrollView];
        
```

### 效果图集

![](/文字-竖直-一行循环轮播.gif) 
![](/图片-竖直-一行循环轮播.gif) 

![](/文字-竖直-二行循环轮播.gif) 
![](/图片-竖直-二行循环轮播.gif)

![](/文字-竖直-三行循环轮播.gif) 
![](/图片-竖直-三行循环轮播.gif) 

![](/文字-水平-一行循环轮播.gif) 
![](/图片-水平-一行循环轮播.gif) 

![](/文字-水平-二行循环轮播.gif) 
![](/图片-水平-二行循环轮播.gif)

![](/文字-水平-三行循环轮播.gif) 
![](/图片-水平-三行循环轮播.gif)
