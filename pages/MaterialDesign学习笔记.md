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
		  collapsed:: true
		  Material Design具有三维特性(three-dimensional qualities)，这体现在它对表面、深度和阴影的使用上。
			- ^^物质环境(Material environment)^^
			  collapsed:: true
				- 物理世界(The physical world)
				  在物理世界中，物体可以堆叠(stack)或相互连接，但是不能相互穿过。它们投射阴影并反射光。
				  Material Design 通过表面(surface)的显示和在UI中的移动规则来展示物理世界的这些品质。表面以及他们如何在三个维度中移动，与一种类似于在物理世界中移动的方式进行方法上的交流学习。这种空间模型可以在应用程序中一致地应用。
				- 深度(Depth)
				  Material Design显示在使用光、表面、和投射阴影表达3D空间的环境中。Material环境中的所有元素都沿着Z轴水平、垂直和以不同的深度移动。*深度是通过在沿Z轴正方向向观察者延伸的各个点放置元素来描绘。*
				  在Web上，用户界面通过操纵(manipulate)Y轴来表达3D空间。
			- ^^特性(Properties)^^
			  collapsed:: true
			  Material 表面在整个材料设计中有一致的、不可改变的特性(characteristics)和行为(behaviors)。
				- 尺寸(Dimensions)
				  Material具有不同的x和y尺寸(以dp为单位)和均匀的厚度(1dp)。
				- 阴影(Shadows)
				  不同高度的Material 表面投射不同阴影。
				- 分辨率(Resolution)
				  Material具有无限分辨率
				- 内容(content)
				  内容以任何形状和颜色显示在Material上。内容不会增加Material的厚度。内容不会以单独的层展现。
					- Material可以显示任何形状和颜色。内容的行为可以独立于Material，但是仅限于Material的边界范围内。
					- 内容行为可以独立于表面行为。
					- 内容行为可以取决于表面行为。
				- 物理特性(Physical properties)
					- Material是固态的。用户输入和交互不能穿透Material表面。
					  				* 输入事件只影响材质的表面
					  				* 输入事件不能通过Material表面
					- 多个Material元素不能同时占据空间中的同一点。
					  				* 防止多个Material元素同时占据空间中的同一点，例如通过使用高程(elevation)分隔元素。
					- Material不能穿透另一个Material。例如，当改变高程时，一个Material表面不能穿透另一个Material表面。
					- Material的行为不像气体。
					  				* Material通过透明度、大小和位置的变化进出。
					- Material不像液体或凝胶那样具有流动性，但他可能会显示具有流体特性的内容
				- 变换材料(Transforming Material)
					- Material可以改变形状
					- Material可以改变透明度
					  				* Material可以在其整个表面均匀的改变不透明度
					  				* Material可以改变其表面一部分的不透明度
					- Material仅沿其平面生长和收缩
					- Material在UI深度内弯曲或折叠。
					- Material表面可以连接在一起成为单一的Material表面
					- 拆分时，Material可以重新连接。例如，如果您从表面移除一部分材料，该表面将再次变得完整。
				- 移动(Movement)
					- Material可以在环境中的任何地方自发生成或消除。
					- Material可以沿任何轴移动
					- Material表面可以协调运动
					- Material沿Z轴运动通常是用户交互的结果
			- ^^属性(Attributes)^^
				- 基础Material表面(Basic Material surface)
				  基础的Material表面是不透明的白色，厚度为1dp，并投射阴影。所有的UI元素都源于对该表面的修改。
				- 行为(Behavior)
				  Material表面以一些特定的行为表现：
				  			* 刚性表面(Rigid surfaces)：在所有交互中保持相同的大小
				  			* 可拉伸表面(Stretchable surfaces)：可以沿着一条或多条边生长和收缩到一定尺寸的限制，然后表现为刚性表面。
				  			* 平移表面(Pannable surfaces)：在整个交互中保持相同的大小。可以在区域内滚动显示其他内容，直到达到内容限制。材料表面尺寸可以保持刚性，但内容可以在表面上滚动或平移。
					- 复合表面(composite surfaces)：表面可以分为显示不同类型行为的区域。
					  				* 单个表面可以包含多个可平移表面
					  				* 卡片可以拉伸以显示独立于卡片其他内容的滚动区域
				- 可拉伸表面(Stretchable surfaces)：
				  可拉伸表面在达到限制点成为刚性表面之前可以拉伸。表面可以垂直、水平或双向拉伸。
				  通常，用户与表面的交互会使其向一个方向拉伸。
					- Material拉伸的方向可以完全是垂直的。
					- Material拉伸的方向可以完全是水平的。
					- Material可以独立或同时沿水平和垂直的轴拉伸。
				- 表面定位和位移(Surface positioning and movement<x/y>)
				  表面可以在X轴和Y轴保持固定的位置，也可以沿任何方向移动。
					- 表面运动可以限制在单个轴上，允许运动沿着单个轴运动，或允许运动同时沿着两个轴运动。
					- 表面可以彼此独立的运动，或者他们的运动可以影响或依赖其他表面的运动。
					  相关性可以基于各种机制(mechanics)，例如附近的表面在另一个表面膨胀时移动，或者在视差中移动的表面之间的运动比例。
				- 表面不透明度(Surface opacity)
				  Material表面可以是透明、半透明或不透明的。
					- 透明和半透明的表面上的文本可能需要进行背景处理以保持可读性。
					- 透明表面缺少清晰的边缘，因此很难确定表面的起点和终点以及表面内容所属的位置。
				- 纱布(Scrim)
				  纱布是临时处理，可以应用于Material表面，目的是让表面上的内容不那么突出显眼。它们引导用户的注意力到屏幕的其他地方，远离覆盖纱布的区域。
				  纱布可用多种方式实现：
				  			* 使表面和其内容变暗或变亮
				  			* 减少表面和其内容的透明度
				   屏幕上的多个表面可以同时覆盖纱布层。纱布层可以出现在任何高程，无论前景还是背景。
		- 高度(Elevation) 
		  collapsed:: true
		  高度是两个表面沿着Z轴的相对距离(relative distance)。
			- Material Design中的高度(Elevation in Material Design)
			  collapsed:: true
				- 测量高度(Measure elevation)
				  			* 在Material Design中，高度就是两个Material表面之间测量的距离。从一个Material表面前部到另一个Material表面前部的距离是沿着Z轴以密度无关的(density-independent)像素进行测量，并（默认情况下）使用阴影来表示。
				  			* 当其他表面出现在背后时，同一高度的表面可能会以不同的方式出现。
				- 高度系统(The elevation system)
				  所有的Material表面和组件都有高度值。
				  不同高度的表面都执行以下操作：
				  			* 允许表面在其他表面前后移动，例如内容在应用栏背后滚动。
				  			* 反映空间关系，例如浮动操作按钮的阴影表明它和卡片集合是分开的。
				  			* 注意力集中在最高的高度上，例如临时出现在其他表面前面的对话框
				   可以使用阴影或其他视觉提示（表面填充或不透明度）来显示高程。
				- 默认高度(Resting elevation)
				  默认高度是默认情况下组件的起始高度。为响应用户交互或系统事件，组件从默认高度移动。所有Material组件中同类型的组件的高度是一致的。例如，所有卡片具有彼此相同的默认高度，对话框也有相同的高处。
				  			* 默认高度和环境：默认高度因环境、平台和应用而异。移动端的默认高度旨在提供视觉提示，如阴影，表明组件是可以交互的。相反，**桌面端的默认高度就更浅**，因为其他提示（悬浮状态）会在组件交互时显示。
				- 可变高度(Changing elevation)
				  组件可以改变高度以响应用户输入和系统事件。发生这种情况时，组件移动到预设的**高度动态补偿值**(dynamic elevation offsets)，这是组件未静止时移动到的默认高度。
				  			* 每种类型的组件的高度动态补偿值是一样的。例如，所有卡片使用相同的偏移量，所有浮动操作按钮也使用相同的偏移量。
				  			* 一旦用户输入（系统事件）完成或取消，组件迅速返回其默认高度。
				  			* 有些组件通过减少高度来响应用户输入
				- 高度冲突(Elevation interference)
				  当组件在其默认高度和动态高度补偿值之间进行移动时，不应与其他组件发生碰撞。
				  			* 为了避免发生碰撞，可将障碍组件移开。例如，如果增加一个卡片的高度位置，它就会穿过其上浮动操作按钮，可以通过让按钮消失或移除屏幕来避免冲突。
				  			* 也可以重新架构应用的布局来避免这种冲突，例如将浮动操作按钮放置在卡片旁边，而不是直接置于其上。
			- 描绘高度(Depicting elevation)
			  collapsed:: true
			  要成功描绘出高度，表面必须显示：
			  + 表面边缘(edges)，让表面与周围环境形成鲜明对比
			  + 与其他表面重叠(overlap)，无论静止还是运动
			  + 与其他表面有距离
				- 表面边缘(surface edges)
				  边缘有助于表达Material表面的触觉质感(the tactile quality)。它们通过将UI的不同部分分离成可识别的组件来显示一个表面的结束和另一个表面的开始。
				  表示边缘的方式：
				  + 使用阴影
				  + 给表面不同的颜色
				  + 给表面不同的透明度
				  边缘必须在表面之间产生足够的对比度（通过满足或超过可获得的对比度），以便它们被视为彼此分开。
				- 表面重叠(surface overlap)
				  当一个面与另一个面部分或完全重叠时，表明这两个面所处的高度不同（但不是他们之间差异的程度和数量）。高处的表面出现在低处表面的前面，意味着它们沿着X轴被定位在不同的高度上。表面可能在默认情况下相互重叠，或者由于运动改变了它们在UI中的位置而变得重叠。
				  当表面有不同的透明度或相互之间的对比度不足时，会使人很难分辨哪个表面在另一个前面。通过确保明确的界定边缘来避免模糊的重叠。
				- 距离(distance)
				  collapsed:: true
				  表面之间的高度差程度可以用纱布背景(scrimmed backgrounds)，或阴影来表达。
					- 纱布背景(Scrimmed backgrounds)
					  当UI中的背景被遮罩时，表明其上的内容处于更高的高度。 纱布背景表达了大量且未指定(unspecified)的高度。
					  	* **纱布背景可以表示表面重叠，但不能表示高度。**
					- 阴影(Shadows)
					  阴影可以实现其他方式无法表达的两个表面之间的高度。
					  阴影的大小和柔和度(softness)或弥散度(diffusion)都能表示两个表面之间的距离。例如，具有小而清晰的阴影的表面表示该表面与其后面的表面更接近。相反，更大、更柔和的阴影表示更远的距离。
					  阴影大小和扩散的细微差别传达了：
					  	* 两个表面之间距离的详细程度
					  	* 非重叠表面之间的高度差
				- 动效和高度(motion and elevation)
				  collapsed:: true
				  动效可以使用以下方式强调高度：
					- 阴影的变化(changing in shadows)
					  阴影大小和柔和度的变化强调了高度的变化
					- 显示重叠(displaying overlap)
					  一个表面在动画中部分或完全重叠另一个表面，显示了此表面在另一个表面前面。
					- 推动(pushing)
					  具有相同高度的表面可以在它们的路径上移动表面。
					- 缩放(scaling)
					  向上或向下缩放表面可以强调高度变化
					- 视差(Parallax)
					  **不同高度的多个表面以不同速度移动会产生深度感并将焦点聚集在前景内容上。**
					- 结合动效结束(combining motion techniques)
					  可以通过组合动效来强调高度。
			- 高度层级关系(Elevation hierarchy)
			  collapsed:: true
			  内容之间的关系取决于它们是否处于相似或不同的高度。
				- 不同高度的内容(content at different elevations)
				  一个表面前面的表面通常：
				  		* 包含更重要的内容
				  		* 集中注意力，例如对话框
				  		* 控制其后的表面，例如应用栏中的操作
				- 共面内容(content on coplanar surfaces)
				  		* 将表面定位在同一高度使它们共面，并暗示它们包含彼此相同重要的内容。例如，集合中的所有卡片都具有同等重要性。
				  		* 不表示高度的表面看起来是共面的。对于不表示高度的表面，可以通过它们的内容并通过调整水平和垂直的布局位置建议相对的层次级别来传达层次差异。
			- 默认高度(Default elevation)
			  collapsed:: true
			  所有元素都有默认高度和高度动态补偿值的默认值。默写组件处于比其他组件更高的高度，从而在所有组件间建立一致的高度顺序(a consistent elevation)。例如，对话框总是出现在其他组件前面。
			  + 默认高度值：
			  + 默认高度值示意图：
		- 光与影(Light and shadows)
		  collapsed:: true
		  Material 表面阻挡光源时会投射阴影。
			- 光(light)
				- 光与影(light and shadows)
				  在Material Design环境中，虚拟光照亮UI。主光(key light)会产生更清晰的定向阴影，称为**关键阴影(key shadows)**。环境光(ambient light)从各个角度出现以产生漫射的柔和阴影，称为**环境阴影(ambient shadows)**。
				- 光源(light sources)
				  Material Design中的阴影有主光和环境光投射。在Andriod和IOS开发中，当光源沿着沿着Z轴的不同位置被表面阻挡时，就会出现阴影。在Web中，仅通过操纵Y轴来描绘阴影。
			- 阴影(shadows)
			  阴影提供的有关深度、运动方向和表面边缘的提示。一个表面的阴影由其高度和与其他表面的关系决定。
				- 用法(usage)
				  由于阴影表示表面之间的高度，因此必须在整个产品中保持一致。
				  			* 高度通过一致使用阴影来描绘
				  			* 阴影大小反映高度
				- 阴影和运动(shadow and motion)
				  阴影提供有关表面运动方向以及表面之间距离是增加还是减少的有用提示。
				  			* 当表面改变形状或比例，但其高程保持不变，其阴影不变
				  			* 当表面改变高程，阴影也改变。
	- 布局(Layout)
		- 了解布局(Understanding layout)
		  collapsed:: true
		  Material Design布局使用统一的元素和间距，以促进跨平台、环境和屏幕大小的一致性。
			- 原则(Principles)
			  collapsed:: true
			  		* 可预测性(Predictable)：使用具有一致UI区域(consistent UI region)和空间组织(spatial organization)的直观(intuitive)和可预测的布局
			  		* 一致性(consistent)：布局应该一致地使用网格、基线(keyline)和边距(padding)
			  		* 响应性(responsive)：布局时自适应的。它们能对来自用户、设备和屏幕元素的输入做出反应。
			- 布局结构(Layout anatomy)
			  collapsed:: true
			  **布局区域(layout regions)**是交互体验的基础。它们是布局的**构建块(building blocks)**，由具有相同功能的元素和组件构成。**布局区域还可以对较小的容器（例如卡片）进行分组。**
			  大屏幕布局有三个主要区域：
			  		* 应用栏(app bar)
			  		* 导航(navigation)
			  		* 主体(body)
			   在创建响应式布局系统时，为主体和边距创建最小和最大的**尺寸**以及允许每个区域适应不同形状因素的**缩放行为**是有帮助的。以下指南描述了Material的基准尺寸和行为。
				- 主体区域(body region)
				  主体区域用来显示一个应用程序中大部分的内容。它通常包含列表、卡片、按钮和图片等组件。
				  主体区域使用三个参数的缩放值(scaling value)：
				  			* 垂直和水平尺寸(vertical and horizontal dimension)
				  			* 列数(number of column)
				  			* 边距(margins)
				   在超小的断点处(extra small breakpoints)边距是16dp。随着布局尺寸增加，主体部分相对于屏幕宽度进行扩展。到达第一个断点(600dp)边距增加到32dp。当主体的宽度达到840dp，边距增加到最大宽度200dp。在到达这个最大宽度后，主体区域再次变得可响应。
				   ^^响应式网格(responsive column grid)^^：响应式网格由列、槽、边距组成，为主体区域内的元素布局提供方便的结构。组件、图片和文本与列网格对其，以确保跨屏幕尺寸和方向的有逻辑且一致的布局。随着主体区域大小增大或缩小，网格列数会相应发生变化。
				- 导航区域(navigation region)
				  导航区域包含导航组件和元素，例如导航抽屉(navigation drawer)或导航栏(navigation rail)。它可以帮助用户在应用程序中的目的地之间导航或访问重要操作。**导航区域在展开(expand)时保持一致的256dp，折叠(collapse)时为72dp。**
				  如果布局的边距小于48dp（例如，屏幕宽度在600dp到839dp之间），主体区域的宽度可以减小以适应导航区域。
				  			* 当使用导航抽屉时，主体区域可以压缩以容纳导航区域
				  			* 处于折叠状态的导航区域(72dp)可以使用导航栏。
				  			* 如果屏幕宽度小于600dp，导航区域可以使用模态导航抽屉(modal navigation drawer)。抽屉看起来高于主体区域
				- 应用栏(app bar)
				  应用看用于显示和分组组件和操作，帮助用户执行主要操作，或对主体区域的元素执行操作。
			- 构成(Composition)
			  collapsed:: true
				- 视觉分组(visual grouping)
				  **在布局中创建秩序的第一步就是视觉分组**。布局中有相同内容或功能的元素可以组合在一起，并使用开放空间、排版和分割线与其它元素分开。
				- 包含(containment)
				  在视觉分组之后，下一组要考虑的是任何通过共享上下文达到相关的元素（即组内元素），例如图片及其标题(caption)和支持信息。这些上下文相关的元素(contextually related elements)可以使用约束的概念组合在一起。 通过在组之间创立边界来实现约束。
				  			* 方法1：**隐式包含(implicit containment)**，通过将相关元素拉近来减少它们周围的开放空间。同时，增加了这个分组之外的空间，以创建一个独特的概念边界。
				  			* 方法2：**显示包含(explicit containment)**，通过向一组相关元素添加**边框(outline)**或**高度层级(elevation level)**来创建。例如，根据图像及其标题或支持信息创建卡片，通过卡片升高的边界(elevated boundary)使元素定义为一组。
				   当使用元素或组件来包含文本时，请确保每个容器使用响应式尺寸，以便文本能轻松缩放和保持可读性。
				- 随文本缩放(scaling with text)
				  文本的理想长度是40-60个字符。当缩放包含文本的元素（例如卡片）时能保证可读性。当元素包含文本时，边距(margin)和排版属性(typographic properties)应该是响应式的，这样能确保文本在水平布局不会延伸太长。达到最长行后，排版有助于提高可读性。
				  如果文本必须很长的话，就要考虑调整行高(line height)来提高可读性。
				- 锚点和约束(anchors and constraints)
				  			* 当缩放组件或布局容器时，需要考虑它们的位置(position)及对齐方式(alignment)如何缩放。当父容器缩放时，内部元素可以锚定到左侧、右侧或者中心。内部元素也可以保持固定位置，例如当浮动操作按钮和导航抽屉的情况下。
				  			* 组件内部的组成应适应其承载的设备的人体工程学需求(ergonomic needs)。例如，移动设备上横向卡片可以适应更大屏幕上更方形的卡片。此更改使图像更突出，并允许使用更大的字体样式来提高可读性。在图标按钮中，按钮中的图标和文本标签可以保持彼此锚定，在按钮水平缩放时保持局中。
			- Material 距离(Material measurements)
			  		* 为了确保Material Design视觉上保持平衡，大多数测量值都与8dp对齐，这对应间距和整体布局。组件的大小是以8dp为增量，确保每个屏幕的视觉节奏一致
			  		* 较小的元素(例如图标)可以与4dp网格对齐，而排版可以落在4dp基线网格上，这意味着每行的排版基线与其相邻元素的间距以4dp为增量。
			- 资源(Resources)
		- 像素密度(Pixel density)
		  屏幕像素密度和分辨率(resolution)因平台而异
			- 像素密度(pixel density)
			  一英寸内的像素数称为像素密度(ppi)
				- 屏幕密度变化(screen density variations)
				  高密度屏幕(high-density screens)的每英寸像素数比低密度屏幕(low-density screens)多。因此，相同像素数量的UI元素在低密度像素屏幕上显得更大，而在高密度屏幕上显得小。
				- 计算像素密度(calculating pixel density)
			- 密度独立(density independence)
			- Andriod上的像素密度(pixel density on Android)
			- IOS上的像素密度(pixel density on IOS)
			- Web上的像素密度(pixel density on the web)
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
			  Material Design以**有意义的方式**/将颜色应用于UI。在此系统中，可以选择一个主要颜色(primary)和次要颜色(secondary)来代表品牌。然后以**不同的方式**将每种颜色的深色和浅色变体(variant)应用于UI。
				- 颜色和主题
				  + 颜色主题旨在和谐(harmonious)，确保可访问的文本(accessible text)，并将UI元素和表面(surface)彼此区分开来。
				  + 工具： ((61d3c6db-9fab-436f-8a70-2377f5b1bc2b))
				- 原则
				  + **分层**(Hierarchical)：颜色指示哪种元素可以交互，它们与其他元素的关系以及它们的突出层度(prominence)。
				  + **清晰易读**(legible)：当出现在彩色背景上时，文本和重要元素（如图标）应符合易读性标准(legibility standards)。
				  + **富有表现力**(expressive)：在令人难忘的时刻展现品牌色彩，强化品牌风格。
			- ^^色彩主题创作(Color theme creation)^^
				- 基线Material颜色主题(The baseline Material color theme)
				  Material Design有一个内置的基线主题，可以按原样使用，直接从众所周知的盒子(proverbial box)里出来。
				  ![2022_01_04_unnamed.png](https://cdn.logseq.com/%2F95018d4c-669b-4f2c-ba55-a52b94e8b69d02b1749d-f8f7-4b63-8289-e46a9457dd062022_01_04_unnamed.png?Expires=4794902864&Signature=Io6A58qii4MLgFtxcTAVOOyTW66oVPA0DLRLPNOmEUrkly5GLJzQyeL4DkQFJ97iFuoxlbJyf1~V~Myj88q8uF4mseZEwgpe71ffXQkvgSRZjM6BR2z8p-RmWpa3f-4v8opncEAwgxf5zNlV7nX5ZBvm7nCAbAYCa1I5X6p~Lu4U-Ffi5HVC2WYeOsmA16FGJfqEpYeD~-2GbPWGinWq5mOYvRA3n50ja0fhbZeskH1fVm9Sxqnc5bE8ogD12Ij6w9GGQt6pW5ghrRdX0yjBEV0CRz53jpzSkcdjpfuzAo057Z5wSMlMGp064tzXDzxuHR1rU0n0XSx3FiL8pyfoDw__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA)
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
				  ![2022_01_04_屏幕截图 2022-01-04 213051.png](https://cdn.logseq.com/%2F95018d4c-669b-4f2c-ba55-a52b94e8b69dc4458d3d-22f2-48f5-ac0e-65f5e0cd74092022_01_04_%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-01-04%20213051.png?Expires=4794903098&Signature=KS-BK5hdr1wYZjwjIDsQdI-e6xm1mTbGWWBKhqb6rnkYpgACyq3oPqRc3QsahLsdPZGNjDNUX6t4oV0nG8wKamT28GfQwdPRHfmU1e1kaRNRKIT4US0T91jH8xlBmo9EMuKbb0XNHjf2ugfqa0gqL4OAL3AI01Y75mBAS8OC~V9FqXwBDgwXAePYQNKttnmK~aUzCXn0a3JoxY4wwR5yNn0kem8OfLgDxR8W6SkD9ogONuONlMlfSwQNYajkxGjEDlIt8wNPyShloTAI6dSF6ZibFiKCCTjr7nP1FNlWGM6hYMaU3DonHKraY-25eM2fJ6o5MII-qLMUyZtOU2o9YQ__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA)
				- 排版(typography)和图标(iconography)的颜色
				  “On”颜色：**命名规则——On Primary / On Secondary / On Background / On Surface / On Error**
				  应用程序界面使用调色板中特定类别的颜色，比如主色。每当元素（例如文本或图标）出现在这些表面之前，元素应使用在其背后颜色对比下能清晰易读的颜色。此类颜色称为“On”颜色，指的是它们为出现在使用以下颜色的表面上的元素着色：主色、辅色、表面颜色、背景颜色和错误颜色。
				  "On"颜色可以用于文本、图标和描边(strokes)。有时可以用于表面。
				  ![2022_01_04_unnamed (2).png](https://cdn.logseq.com/%2F95018d4c-669b-4f2c-ba55-a52b94e8b69d743e7cd2-9349-441e-810c-15cb4fa0fe262022_01_04_unnamed%20%282%29.png?Expires=4794903218&Signature=AMgAjTVdqEIcjbnySKF~JQHtT8qCaUPvbzmZfil13TaSZ0pMDglZ6L6YMh-tWG6TSwKz8jYqke7-AoIICzzrP9N-xnptmmNC2VW1eiuH0LaWg94ULGeU873DiB1ZOEMATGJoUR-bo29jnTEefozhAmGST0pf81uyZ4gQbNmLikWcS3To9r~-ye0JHfqiNqQtWPWwhO0NDfdFVIZsDlL~IHrgbqCGrqNUoACaP3SsLZj-u-OArhkBPKDkEgm4VU9YxRFWNqg0K-RbcUZYo~I-ZTTzb8L9PnvPkrnFHWsLshkkODNFZQWwbdpC8pOKWAgYXBs21wAjhsZWG791sHCi9g__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA)
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
					  ![2022_01_04_unnamed (3).png](https://cdn.logseq.com/%2F95018d4c-669b-4f2c-ba55-a52b94e8b69deaf4f4a6-4696-4067-9ec8-7d5d0ff028452022_01_04_unnamed%20%283%29.png?Expires=4794903513&Signature=iSO0PSCFoqeBppGPbxZugC2PBboQbUqhA16ME2VPAn5fbSVKintcEge9sF2LxBnz8pmpwHSMv5nnbbesKmvw5DAhUgWRb63abyVmC9Rya5dTMB1YpkQ~0O8A0yvVT-SH33p~naPPczM2WbprF8dB~14QD61ur5CKAxedEaDIh-EYSUnuXk9jGsP6UpwzNYn7tAPgX7Hr1Kqoxjs7M~szhbbXIx-22wEj2gUNaRnOyAkaNj1~H7i7NGqv1zr6CBtQZFYn06~~y9l1deswmUypNHYJs0HOWlZugCqrHlJHaq8AwofXCJdODDDBkEnJRTZ7YiM5LM1wObSaI-No33mnow__&Key-Pair-Id=APKAJE5CCD6X7MP6PTEA)
			- ^^[挑选颜色的工具(Tools for picking colors)](https://material.io/design/color/the-color-system.html#tools-for-picking-colors)^^
			  id:: 61d3c6db-9fab-436f-8a70-2377f5b1bc2b
				- Material调色板生成器(palette generator)
				- 2014Material Design调色板(color palettes)
				- [Color Tool](https://material.io/resources/color/#!/?view.left=0&view.right=0&primary.color=6002ee)
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