- 第一章 Material Design
  collapsed:: true
	- **原则**
	  Material Design是一种隐喻(metaphor)，它学习现实世界中物体的纹理、反光和投影，重新展现物理世界中纸张和墨水表达的信息。
		- 粗体(Bold)、图形(Graphic)、目的(Intentional)
		  collapsed:: true
		  *Material Design以印刷设计(print design)(排版typography、网格grids、空间space、比例scale、颜色color和图像imagery)为指导，去创建有层次结构hierarchy、意义meaning和焦点focus的产品，让观众沉浸在体验中*
		- 动效带来意义
		  *动效通过微妙的反馈(subtle feedback)和连贯的过渡(coherent transitions)来集中注意力并保持连续性。当元素出现在屏幕上时，它们会通过交互产生新的转换来转换(transformation)和重组环境*
	- **组件**
	  Material组件是用于创建用户界面的交互式构建块(interactive building block)，包括一个内置的状态系统(built-in states system)，用来传达焦点(focus)、选择(selection)、激活(activation)、错误(error)、悬停(hover)、按下(press)、拖动(drag)、和禁用状态(disabled states)。组件库可用于Android、IOS、Flutter和Web。
	  **组件涵盖了一系列接口需求，包括：**
		- ^^显示^^(display)：使用卡片(cards)、列表(lists)和工作表(sheets)等组件放置和组织内容
		- ^^导航^^(navigation)：允许用户使用导航抽屉(navigation drawers)和标签(tabs)等组件在产品中移动
		- ^^操作^^(actions)：允许用户使用浮动操作按钮(floating action button)等组件执行任务
		- ^^输入^^(Input)：允许用户使用文本字段(text fields)、芯片(chips)和选择控件(selection controls)等组件输入信息或进行选择
		- ^^通信^^(communication)：使用快捷栏(snackbars)、横幅(banners)和对话框(dialogs)等组件
	- 主题化
	  可自定义颜色、排版样式和角样式的内置支持和指导，让Material Theme可以轻松自定义Material Design以匹配品牌的外观和感觉。
	  *可以轻松修改按钮等组件的颜色、排版和形状，以匹配风格*
		- ^^颜色^^(color)：Material 的颜色系统(color system)是一种将颜色运用于UI的有组织的方法。全局颜色样式在组件中具有语义(semantic)名称和定义的用法——主要(primary)、次要(secondary)(品牌颜色)、表面(surface)、背景(background)和错误(error)。*每种颜色还有一种互补色(complementary)，用于放置在其“上方”的元素，以促进一致性(consistency)和可访问的对比度(accessible contrast)*
		- ^^排版^^(typography)：Material Design类型量表(type scale)为从标题(headlines)到正文(body text)和标签(caption)提供13种排版样式。每种样式在界面中都有明确的含义和预期应用。
	- 形状
	  应用形状样式有助于引导注意力或识别组件、传达其状态和表达品牌。
	  所有Material组件都根据其大小(small、medium、large)分为形状类别。这些全局样式提供了一种快速更改类似大小组件形状的方法。
- 第二章 Material Foundation
	- 基础
	  Material Design定义了可以由UI区域(UI region)、表面(surface)和组件(component)表达的品质。使用从广泛和详细的角度解决设计问题的基础来设计和制定应用程序的构建方式。
	- 环境(Environment)
		- 表面(surface)
		  Material Design具有三维特性(three-dimensional qualities)，这体现在它对表面、深度和阴影的使用上
		- 海拔(elevation)
		- 光与影(Light and shadows)
	- 布局(Layout)
		- 了解布局(Understanding layout)
		- 像素密度(Pixel density)
		- 响应式布局网格(Responsive layout grid)
		- 间距方法(Spacing method)
		- 组件行为(Component behavior)
		- 应用密度(Applying density)
	- 导航(Navigation)
		- 了解导航(Understanding navigation)
		- 导航转换(Navigation transitions)
		- 搜索(search)
	- 颜色(color)
		- **颜色系统(The color system)**
		  collapsed:: true
		  Material Design颜色系统可以帮助创建反映品牌或风格的颜色主题。
			- ^^颜色使用和调色板(Color usage and palettes)^^
			  collapsed:: true
			  Material Design以**有意义的方式**/将颜色应用于UI。在此系统中，可以选择一个主要颜色(primary)和次要颜色(secondary)来代表品牌。然后以**不同的方式**将每种颜色的深色和浅色变体(variant)应用于UI。
				- 颜色和主题
				  + 颜色主题旨在和谐(harmonious)，确保可访问的文本(accessible text)，并将UI元素和表面(surface)彼此区分开来。
				  + 工具： ((61d3c6db-9fab-436f-8a70-2377f5b1bc2b))
				- 原则
				  + **分层**(Hierarchical)：颜色指示哪种元素可以交互，它们与其他元素的关系以及它们的突出层度(prominence)。
				  + **清晰易读**(legible)：当出现在彩色背景上时，文本和重要元素（如图标）应符合易读性标准(legibility standards)。
				  + **富有表现力**(expressive)：在令人难忘的时刻展现品牌色彩，强化品牌风格。
			- ^^色彩主题创作(Color theme creation)^^
			  collapsed:: true
				- 基线Material颜色主题(The baseline Material color theme)
				  Material Design有一个内置的基线主题，可以按原样使用，直接从众所周知的盒子(proverbial box)里出来。
				- 主色(primary color)：主色是在应用程序的屏幕和组件显示最频繁的颜色。
				  + 主色的深色和浅色变体(Dark and light primary variants)：主色可用于为应用制作颜色主题，包括主色的深色和浅色变体
				  + 区分UI元素(distinguish UI Elements)：要在UI元素（例如系统栏的顶部应用栏）之间创建对比(contrast)，可以使用主色的浅色或深色变种。也可以使用这些来区分组件内元素，例如浮动操作按钮的图标与其圆形容器。
				- 辅色(secondary color)：辅色提供更多方式来强调和区分产品。辅色是可选的(optional)，应该谨慎应用以突出UI的选定部分。如果没有辅色，主色也可用于强调元素。
					- 辅色最适合：
					  + 浮动操作按钮(floating action buttons)
					  + 选择控件，如滑块(sliders)和开关(switches)
					  + 突出选定的文本(highlighting selected text)
					  + 进度条(progress bars)
					  + 链接(links)和标题(headlines)
					- 辅色的深色和浅色变体：
					  就像主色一样，辅色也有深色和浅色两种变体。颜色主题可以使用主色、辅色以及每种颜色的深色和浅色变体。
				- 表面(surface)、背景(background)和错误(error)颜色：表面、背景和错误颜色通常不代表品牌。
				  + 表面颜色(surface color)：会影响组件的表面，例如卡片、工作表和菜单
				  + 背景颜色(background color)：滚动内容后面的背景，默认(baseline)的背景和表面颜色都是#FFFFFF
				  + 错误颜色(error color)：表示组件中的错误，例如文本字段中的无效文本。默认的错误颜色是#B0020
				- 排版(typography)和图标(iconography)的颜色
				  “On”颜色：**命名规则——On Primary / On Secondary / On Background / On Surface / On Error**
				  应用程序界面使用调色板中特定类别的颜色，比如主色。每当元素（例如文本或图标）出现在这些表面之前，元素应使用在其背后颜色对比下能清晰易读的颜色。此类颜色称为“On”颜色，指的是它们为出现在使用以下颜色的表面上的元素着色：主色、辅色、表面颜色、背景颜色和错误颜色。
				  "On"颜色可以用于文本、图标和描边(strokes)。有时可以用于表面。
				- 无障碍颜色(accessible colors) 
				  为了确保浅色或深色文本背后的背景可访问，背景可以使用主色和辅色的浅色和深色变体。或者这些颜色可用于出现在浅色和深色背景前的排版。
					- 色板(color swatches)
					  一个样本是从一系列相似颜色中选择的颜色样本
					- 使用白色文本的应用程序必须具有在白色文本下可访问的背景。
					  使用黑色文本的应用程序必须具有在黑色文本下可访问的背景。
				- 替代颜色(alternative colors)
				  Material Design颜色系统支持替代颜色，这些颜色用作品牌主色和辅色的替代颜色（它们构成主题的附加颜色）。替代颜色可以用于区分UI不同的部分。
				  可适用于：
				  + 具有明暗主题的应用
				  + 不同版块有不同主题的应用
				  + 作为产品套件一部分的应用程序
					- 明暗主题
					  一些应用同时具有浅色和深色主题。为了保持元素的可见性(visibility)和文本的易读性(legibility)，可以为深色和浅色主题调整不同的配色方案(color schemes)。
					- 部分主题的替代颜色
					  替代颜色可用为应用程序的不同部分设置主题。
					- 用于数据可视化(data visualization)的附加颜色
					  应用程序可以使用其他颜色来传达主颜色主题之外的类别。它们仍然是完整调色板的一部分。
			- ^^挑选颜色的工具(Tools for picking colors)^^
			  collapsed:: true
			  id:: 61d3c6db-9fab-436f-8a70-2377f5b1bc2b
				- Material调色板生成器(palette generator)
				- 2014Material Design调色板(color palettes)
		- 将颜色应用到UI(Applying color to UI)
		- 颜色使用(Color usage)
		- 文本易读性(Text legibility)
		- 暗色主题(Dark Theme)
	- 排版(Typography)
		- 类型系统(The type system)
		- 理解排版(Understanding typography)
		- 语言支持(Language support)
	- 声音(Sound)
	- 图标(Iconography)
		- 产品图标(Product icons)
		- 系统图标(System icons)
		- 动画图标(Animated icons)
	- 形状(Shape)
		- 关于形状(About shape)
		- 形状和层次结构(Shape and hierarchy)
		- 形状作为表达(Shape as expression)
		- 形状和运动(shape and motion)
		- 将形状应用到UI(Applying shape to UI)
	- 运动(motion)
		- 理解运动(Understanding motion)
		- 运动系统(The motion system)
		- 速度(Speed)
		- 编舞(Choreography)
		- 定制(Customization)
	- 交互(Interaction)
		- 手势(Gestures)
		- 选择(Selection)
		- 状态(States)
	- 沟通