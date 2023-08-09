# 思源笔记-kmind 插件
    xmind你不要打电话来了，我怕kmind误会
## 重要通知 
由于多tab页的数据复杂性，目前插件版Kmind会有拖拽节点时节点丢失的bug
（kmind挂件为单一数据源，所以无此问题），请将现存的文件导出为json格式，即可在kmind挂件中或者
<a href="https://wanglin2.github.io/mind-map/#/">此在线网站</a> 中导入使用，也可以导出为xmind文件使用。
也可以直接使用挂件版kmind直接选择导入kmind插件文件夹下的的kmind文件。
如果您不需要kmind挂件的悬浮预览功能，也可以卸载此插件！

## 缘起
思源笔记是一款我很喜欢的笔记软件，但是它的导图功能却不是很完善，而我恰好是思维导图重度使用者 

一直以来都是用的xmind做笔记，规划生活等等，但是由于xmind比较贵，并且绑定设备，而且必须要使用xmind客户端才能打开，
拥有多台设备的我感觉很痛苦，并且在与其它软件或者生态的联动方面，xmind一直都迟迟不做改进。

所以我基于开源库开发了思源思维导图挂件：[kmind](https://github.com/suka233/siyuan-Kmind)。
后来，思源的目录插件作者[@TinkMingKing](https://github.com/TinkMingKing)建议我开发一个插件版思维导图，
我想想，确实，挂件版本的kmind由于只能插入到某篇具体的文档中，和单篇文档高度相关，无法覆盖所有的思维导图应用场景，所以这个插件就诞生啦~

高强度使用此插件半个多月的我突然发现，我已经好久没有打开过xmind了，所以，xmind你以后不要打电话来了，我怕kmind误会 :p

## kmind特点
1.随意导入 or 导出xmind文件，并且额外支持导出为图片、markdown、svg文件，以及通用的json文件，这也是我从xmind转为kmind的底气
![exportToXmind.gif](img%2FexportToXmind.gif)
2.现代化的设计：采用了蚂蚁的Ant Design UI组件库，界面简洁大方

3.高度可配置：支持自定义主题、结构、节点的字体、字号、并且可以配置新建导图的默认动作，比如新建一张kmind的时候，自动选择某个设定好的主题，自动开启禅模式等等
![changeStyle.gif](img%2FchangeStyle.gif)
4.富文本节点：目前市面上的思维导图的节点为普通的文本格式，富文本节点由于可以加粗指定文字，更改背景或者文字颜色，可以更好的突出重点

5.和思源笔记深度结合：如果把节点的超链接设置为思源的块超链接，点击即可跳转到思源笔记的指定块，如果按住Alt键点击，还可以直接在kmind中悬浮预览思源笔记的指定块
![kmindguide.gif](img%2Fkmindguide.gif)
6.开放性：得益于开源的力量，单个节点能承载的功能可以开发出更多玩法，比如：在节点中渲染出思源笔记指定的编辑区是什么样的体验？
![siyuanBlock.gif](img%2FsiyuanBlock.gif)
7.数据安全：kmind的所有数据全部存储于本地，并且与思源的笔记本数据完全隔离，也没有任何交互。所以不会对思源的数据造成任何影响。此外，kmind会在你编辑的时候，智能每隔1s自动保存数据到本地，意外断电也不怕丢失啦。

## 使用方式
1.在插件市场安装并启用后，在左下角找到kmind的dock，然后点击新建即可
![newKmind.gif](img%2FnewKmind.gif)
2.右上角的菜单为全局配置菜单，可以设置默认的主题、字体、字号、新建导图的默认动作等等，下个版本开放

3.快捷键的说明详见插件菜单，由于为了避免kmind快捷键和思源的快捷键冲突，所以kmind的快捷键是绑定在单张kmind内部的，所以当快捷键失效的时候，只需要先点击kmind的画布空白处，快捷键即可恢复（挂件遇到此问题同理）
![shortcut.png](img%2Fshortcut.png)
## 反馈

如果你需要反馈，可以去我的github仓库提交[issue](https://github.com/suka233/siyuan-kmind-plugin/issues),如果你没有github账号，可以[点我反馈](https://wj.qq.com/s2/12591272/adf1/)。如果你要捐赠我，可以[点我](https://wj.qq.com/s2/12591272/adf1/)，
或者去我的github仓库给[本插件](https://github.com/suka233/siyuan-kmind-plugin/issues)点一颗star吧~

## 付费

kmind插件的基础编辑功能永久免费使用，不限制导图数量，也不限制节点数量。之后与思源或者外部结合的高级功能可能需要付费（目前此插件收益负50元，因为我向上游库的导图库作者捐赠了50元😋 ），等到正式付费，各位的捐赠金额可以双倍抵扣kmind费用

## 致谢

感谢[@wanglin2/mind-map](https://github.com/wanglin2/mind-map)大佬开发的导图库，没有他就没有本项目
感谢思源目录插件作者：[@TinkMingKing](https://github.com/TinkMingKing/siyuan-index-plugins) 大佬的提议与帮助
感谢顶栏日历插件作者：[@svchord](https://github.com/svchord/siyuan-arco-calendar) 大佬的vue模板参考
感谢开放API插件作者：[@Zuoqiu-Yingyi](https://github.com/Zuoqiu-Yingyi) 萌佬的插件参考与答疑，kmind挂件的悬浮预览脱胎于此
感谢插件系统的开拓者：[@zuoez02](https://github.com/zuoez02/siyuan-plugin-excalidraw) Z佬的Excalidraw插件参考，抄了一点点新建自定义tab页的写法，嘿嘿

## 最后
1.导出为PDF的功能，由于打包问题暂时未解决，所以当前仅在Kmind挂件中提供，如果需要导出为PDF的功能，请去Kmind挂件使用
