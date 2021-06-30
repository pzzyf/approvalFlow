# 内推
 渣渣一个，之前部门缺人的时候有幸过了面试。现在又有缺口，HR忙不过来，领导说只能靠自己内推了。大家有兴趣多看看。

【联系方式】微信： SNFocus_

岗位可零基础培养

如有疑问可询问

投过字节跳动，面试挂过不要紧！部门直推，捞起再面！

项目经验没有强制要求。聪明、基础过硬、深入掌握一门语言即可！ˇˇ

没毕业的同学也可以考虑来实习，实习转正so easy，妈妈再也不用担心我的offer！

满足每周工作4天且实习3个月即可

【我们的愿景】
将行业内的资深精英联合在一起，打造学习体验更好、效率更高、效果更好的

产品
【我们的优势】
业务发展迅猛！团队HC多多，氛围超赞，发展空间巨大!

大平台核心产品，团队氛围好，牛人多，机会多，导师nice，新人培养是团队最重要的事情之一！

字节跳动已经孵化了众多产品，并将持续探索更多的可能性

通过深入理解业务、进行抽象建模，以及用技术手段为业务赋能等方法，将产品打磨到极致，致力为用户提供最满意的服务

【我们希望你】

积极乐观，责任心强，工作认真细致，具有良好的团队沟通与协作能力

对产品有好奇心，关注业内产品，喜欢使用产品，关注产品体验

热爱编程，有良好的自驱力，有较强的学习能力，有强烈的求知欲、好奇心和进取心 ，能及时关注和学习业界最新技术。

Q&A

Q：整体流程是怎么样的？

A：投递简历 -> 通过简历筛选 -> 约面 -> 收割offer

Q：内推相比自己投递有什么优势？

A：业务部门直接内推，可以做到更快通过筛选，更快约面，同时方便直接了解面试进度

Q：可以提前实习吗？

A：非常欢迎选择实习提前加入团队

Q：我之前参加过字节跳动的面试但挂了可以投递吗？

A：可以，前提希望你已经做了更充分的面试准备（LeetCode刷题、操作系统、计算机网络、数据结构）

Q：工作地点在哪里？

A：北京、上海、深圳、广州、杭州

微信： SNFocus_

# 仿钉钉后台审批流程
> 渣新出品，不曾想放到GitHub上居然有人给了Star，人生第一次，分享出来给大家，虽然多半没什么用，供大家一乐也好。垃圾代码，还望轻喷。

基于JakHuang大佬的[form-generator](https://github.com/JakHuang/form-generator)的，仿钉钉后台审批流程创建界面

[Gitee预览入口](http://soning.gitee.io/approvalflow/)

[GitHub仓库](https://github.com/SNFocus/approvalFlow)

[Gitee仓库](https://gitee.com/soning/approvalFlow)

## 主要功能
1. 表单配置(form-generator)
  - 拖拽表单，生成布局页面
  - 配置拖拽组件属性，定制组件形态
  - 生成JSON数据并生成预览页面
2. 流程节点配置(仿钉钉界面)
  - 创建审批流程(发起人，审批人，条件节点，抄送人)
  - 配置节点详细数据，包括条件节点表达式及期望值等
  - 配置节点对表单得权限（目前并未在预览页面中做控制）
  - 必填节点校验

## 基本结构
```
// src
|-- components
|---- BasicSetting // 基础设置
|---- DynamicForm      // 表单配置
|---- Process          // 流程配置
|---- AdvancedSetting  // 高级设置
|---- FormControls     // 扩充表单组件

|-- views
|---- admin  // 后台配置界面
|---- custom // 前台预览界面
```
> 不想把JakHuang大佬的项目拆分出来 一是为了方便学习大佬代码 二是为了以后单独抽离表单出来更方便 所以没有把form-generator项目的公用文件抽离到顶层 流程创建组件同理

## 表单组件
1. 单行输入框, 多行输入框, 数字输入框, 金额
2. 下拉选择, 级联选择, 省市区
3. 单选框组, 多选框组
4. 时间选择, 时间范围, 日期选择, 日期范围
5. 滑块, 组织机构, 附件, 计算公式
6. 布局容器, 表格/列表

## 界面预览
![YL5ip8.png](https://s1.ax1x.com/2020/05/22/YL5ip8.png)
![YL5AXQ.png](https://s1.ax1x.com/2020/05/22/YL5AXQ.png)
![YL5k6g.png](https://s1.ax1x.com/2020/05/22/YL5k6g.png)
![YL5Cff.png](https://s1.ax1x.com/2020/05/22/YL5Cff.png)
![YL5F1S.png](https://s1.ax1x.com/2020/05/22/YL5F1S.png)
![YL5Z0s.png](https://s1.ax1x.com/2020/05/22/YL5Z0s.png)
![YL5Vmj.png](https://s1.ax1x.com/2020/05/22/YL5Vmj.png)

## 郑重感谢
非常感谢JakHuang的[form-generator](https://github.com/JakHuang/form-generator)为我解决了很多问题，也从中学习到了很多。再者就是我fork`form-generator`版本和JakHuang现在的版本也有很大的区别，感兴趣的童鞋可以去JakHuang那儿看看。

## 捐赠
项目发布到现在收到了很多问题反馈和留言，感谢大家的关注，对此我也非常的开心。有同学留言希望能有捐赠通道表示对项目的认同，我也感到非常惊喜。再次表达对大家的感谢之情。
![DTcMUs.png](./public/pay.png)



