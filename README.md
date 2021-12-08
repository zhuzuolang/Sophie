# Sophie

0.什么叫框架？

1.什么是技能(Ability)？
	逻辑层
		task
			task就是具有一个独立功能的拥有初始参数的小模块(比如，移动actor,旋转相机，2s后跳跃等等)
				确定性task，给定初始参数和task的任意一个时间点，可以推演出之后的所有状态
				非确定性task，只能根据初始参数来执行
		技能:
			1.技能可以包含task
			2.技能可以包含技能
			因此技能是颗树，非叶子节点就是技能，叶子节点是task
			因此技能就是各种技能及其组合在时间线上的推进
			技能就是任务运行器(an ability is a TaskRunner)
			怎么运行？
			子技能:
				
		
	表现层
		Instant Cue 和 Loop Cue
		主端Cue和远端Cue


2.技能系统组件(AbilitySystemComponent)？
	管理技能
	
3.属性，AttributeSetComponent?
	能否和AbilitySystemComponent独立？
	
2.Ability和Buff有区别吗？
	除了名字不一样之外没有区别，因此，buff也可以有自己的逻辑
	也就是说，buff也具有可嵌套性，buff也是任务运行器

3.投射物和召唤物有区别吗？
	没有区别，和玩家一样都是Entity，它们都可以拥有并释放技能。
	
4.目标选取怎么做比较好？
	目标选取是Component而不是Entity