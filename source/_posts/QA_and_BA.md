title: QA and BA
date: 2013-03-14
categories:
- Work
tags:
- QA
- BA
comments: true
---

去年7月初开始和某银行保险项目的合作，到我明天下项目，都9个月了。其中，经历了2个项目，其中一个项目由于客户那边的人力资源缺乏问题仅仅维持了3个月；另一个呢，则从开始到现在都6个月了，预计今年6月上线，也就是总周期预计9个月。

和之前不同，这次我在项目中挑战了BA/QA双重身份，简单小结下我理解的两者的工作内容：

`（仅代表我个人项目的经历，不一定和敏捷中QA或者BA标准高度匹配，特此申明下）`

### QA(Quality Analyst）

#### 开发前：

以Story为载体，通过和BA讨论，获得对需求的全面了解，并在开发人员开发之前，确定测试用例集；或者，根据项目需要，和开发人员结对进行功能性自动化测试。

#### 开发中：

随时和开发人员和BA沟通，确保测试用例都实现，针对一些大家都不确定的需求，会找客户产品经理确认。

#### 开发完成：

开始各种测试，侧重探索性测试，因为之前所生成的测试用例，团队默认在开发中这些已经被开发人员实现了，所以开发之后的测试更要侧重一些之前没有写下来的测试场景，侧重回归性测试等

### BA(Business Analyst)

#### 需求分析前：

尽量熟悉产品，分析产品用户群的操作习惯，分析产品的商业价值以及产品经理对产品的定位。

这些都作为在后续活动中的指导方针，比如，这个项目是个针对保险索赔用户的个人信息管理网站，那质量和用户友好性将是最重要的，在后续的开发和测试中，任何关乎用户体验和页面质量的问题我们都需要注意。

#### 需求分析中：

将大块需求，拆分成大小合适，相互依赖较小，可测可估的story, 并且针对这些story,和客户的产品经理深度沟通讨论，把全部信息记录在story上，也就是AC(验收标准)，这个是作为后续各种开发和测试活动的沟通载体存在的。

#### 需求分析后：

story有着清晰详细的验收标准，并且测试人员，开发人员都对需求有个一致的理解，这才是分析任务结束的标准。这之后呢，需求分析人员就要随时根据测试或者开发中出现的预期之外的问题做出响应，比如，测试人员测试发现了一个Bug, 分析人员就要根据产品的定位做出相应的响应，比如这个是不是对产品产生致命影响的，是不是可以暂时降低优先级的，等等，如果还是无法确定，就需要和客户产品经理直接沟通了。
