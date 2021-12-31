- ^^盒子模型^^
  [参考资料]([CSS盒子模型](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model))
- ^^Flex布局^^
	- 一、Flex是Flex Box的缩写，意为“弹性布局”，用来为盒状模型提供最大的灵活性。
		- 任何一个容器都可以指定为Flex布局
		  ``.box{
		           display: flex;
		  }``
		- 行内元素也可以使用Flex布局
		  ``.box{
		           display: inline-flex;
		  }``
		- 在设置Flex布局以后，子元素的float、clear和vertical-align属性将失效
	- 二、采用Flex布局的元素，称为Flex容器(flex container)，简称“容器”。它的所有子元素将自动称为容器成员，称为Flex项目(Flex iteam)，简称“项目”
	  ![2021_12_31_bg2015071004.png](https://cdn.logseq.com/%2F95018d4c-669b-4f2c-ba55-a52b94e8b69d72cc1056-4412-4428-a3b0-2e7b6aba56862021_12_31_bg2015071004.png?Expires=4794540906&Signature=RAVQ17WViBMvivVQczZfKoRqn2nlbOMqwHuQjg8t0iMmc0m0yaIFyL~b9055oAHvMj6PjvDhuTf2kuvqafUBtD1nYvykY7B8E52c5F-8KZohKPy5FuhQvVmYkNfFm61dBq-SLCSK0IZSKEGR4Bn2myW98yn3Ec0sbnTQ5y4Rp4Suq3y4gwEcG8GzKcDorc8jyypVMz4Cxfo3PpGxy0A02dZ1C8E9TOz5s26B~k6gD36~5Sasl1A8SV48uYkqYeO3uA1aV4~odIWaCmeNIs03kO7aGIDUmLelkjDvkL1lzi7hq9UYay3-jBx-YuDw9czEIp1-v9bqyZvBwV7MmSFxTg__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA){:height 312, :width 514}
		- 容器默认存在两根轴：
		  + 水平的主轴(main axis)：主轴开始的位置叫main start，结束的位置叫main end。
		  + 垂直的交叉轴(cross axis)：交叉轴开始的位置叫cross start，结束的位置叫cross end。
		- 项目默认沿主轴排列。单个项目占据的主轴空间叫做main size，占据的交叉轴空间叫做cross size
	- 三、容器的属性
	          + flex-direction
	          + flex-wrap
	          + flex-flow
	          + justify-content
	          + align-item
	          + align-content
	- 四、项目的属性
	  + order
	  + flex-grow
	  + flex-shrink
	  + flex-basis
	  + flex
	  + align-self
- [Flex布局教程-阮一峰](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html?utm_source=tuicool)