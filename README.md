a ConTeXt template for slide

ConTeXt幻灯片模板

## 用法

* 参考下面的done条，以及说明见环境文件env_slide.tex和示例文件slide.lmtx
* 编译：`>context slide.lmtx`

## done, TODO & bug 

* [x] `\slide{content by steps}`分步演示的幻灯片环境（自动生成每个步骤的独立页面）
  * [x] `\step[n]{content}`保持内容占位，在步骤切换时仅显隐或高亮内容
    * [x] 显示以前步骤，隐藏后续步骤（默认模式）
    * [x] 高亮当前步骤模式（`\enablemode[highlightcurrentstep] ... \disablemode[highlightcurrentstep]`）
  * [x] 不预先占位，在步骤切换时确定是否排入
    * [x] `\onstep[n]{content}`仅在预定步骤排入
      * [x] `\noteonstep[n]{content}`无宽度（不影响对齐）的单行小字注释，适用于行末
    * [x] `\fromstep[n]{content}`在预定步骤以后所有步骤排入
      * [x] `\notefromstep[n]{content}`
* [x] 预制样式
  * [x] `\sChapter{content}` 标题
  * [x] `\sTitle{content}` 不编号标题（不列入目录）
  * [x] `\sItems{content}` 圆点头列表
  * [x] `\sItemsA{content}` 大写字母头列表
  * [x] `\sPar{content}` 段落
* [x] 进度条
* [ ] 添加手稿模式，可打印成讲义
* [ ] 跳转和回跳示例
* [ ] 多媒体嵌入
* [ ] 最后一两张的页面布局可能有误（出现页码，可能是装饰页设置有误）
