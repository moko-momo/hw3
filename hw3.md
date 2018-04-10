
### 作业内容 
 
 -  参考 Fantasy Skybox FREE 构建自己的游戏场景
 - 写一个简单的总结，总结游戏对象的使用

------
### 1 构建游戏场景

在Asset Store里下载好天空盒以及其他素材，将素材加载到本地；
![enter description here](http://m.qpic.cn/psb?/53f71654-6458-4891-9edb-89c9b2417582/uZg6uuSg2DsZsnfMdKCztpIdXq3fUZzonjNE18wZNCw!/b/dPMAAAAAAAAA&bo=NQHbAAAAAAADB80!&rf=viewer_4)


在create里找到地形，创建一个新的地形；创建一个新的天空盒，拖入天空盒的素材。
利用地形里的工具创建山脉，根据需要拔高降低；加载地面、树木和草的素材后，种树种草。
这里我还下载了一些看上去很可爱的蘑菇的素材，拖进地形里了，看上去很有魔法的感觉。

![enter description here](http://m.qpic.cn/psb?/53f71654-6458-4891-9edb-89c9b2417582/c6PbWmLscqCCaZ7yNbD80U0AVFrfGgFayu9U4esNxBU!/b/dFYBAAAAAAAA&bo=aAdAAwAAAAADd34!&rf=viewer_4)

----

### 2 游戏对象总结


游戏对象(GameObject)是在使用Unity3D制作游戏的过程中一切在游戏中存在组件的基础，包括了3D对象、2D对象、光线，甚至交互界面。所有的游戏对象都是由空对象(EmptyObject)派生出来的，经过添加不同的组件(Component)创造而成，这与编程中类的概念十分相似。我们可以这样理解，一切在游戏世界中存在的实体或者非实体，都可以经过多次抽抽象而转化成一个物体，这个物体就是空对象，包括了一切对象的共同属性，而根据不同的对象所具有的不同的属性，我们为其添加组件，即得到了不同类型的对象。

例如Main Camera这个最为普及的对象，我们可以看出其组件有Transform、Camera、Flare Layer、Audio Listener。那么其中起摄像机主要作用的即是Camera组件，我们创建一个EmptyObject，则其会自动附带Transform组件，为其添加Camera组件，我们发现在界面中其标识变为摄像机的形状，同时我们获得了另一个视野，通过修改其Transform组件，我们可以发现此时在屏幕上出现的新视野是与我们新建的空对象连在一起的，我们这样就得到了一个简单的Camera，再为其添加Flare Layer、Audio Listener组件，我们便得到了一个与原来默认的Main Camera完全相同的游戏对象，完全可以代替Main Camera。这是简单的游戏对象的使用，根据组件的不同我们有不同的对象使用方法。
