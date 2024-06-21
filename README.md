# crystal-symmetry
Theories of symmetry in crystalline materials

这个repo是参加上海国际晶体学会议的一些笔记和杂乱记录的分享，由于作者关注点，并没有覆盖课程的许多内容，仅按照个人思路进行了征集，主要包含如下内容：

## 我们如何表示晶体？

参考[生成所有晶体群和布拉维晶系](https://github.com/Osgood001/crystal-symmetry/issues/2)，里面介绍了如何用唯一确定的符号和数值给出晶体群的结构，核心结论是：晶体的有趣在于存在层级的分类，从7个晶体族，到14晶系，到32晶体空间点群，到230个晶体空间群$g$，每个群下还可选特定的Wyckoff Position$W$，选定后，还需要给出其中的自由度$X$，这些都确定之后，上面放置的元素也各不相同$A$。因此，$g, W, X, A$基本就足以描述了，当然，晶体晶格常数$L$也是需要specify的。因此，一个晶体只需要确定$g,W,X,A,L$即可。

## 230个晶体空间群怎么表示？

参考[阅读Hermain-Mauguin符号以可视化晶体](https://github.com/Osgood001/crystal-symmetry/issues/4)，里面介绍了如何根据HM符号，确定空间群对应的晶体结构。核心结论是：将该符号与晶体类型直接关联可以通过[查表工具](https://github.com/rwgk/sginfo/tree/master?tab=readme-ov-file)，直接可视化可以参考[可视化程序](https://github.com/FurinaWai77/GroupImpact)，主流的软件包Pymatgen也[支持这一功能](https://github.com/materialsproject/pymatgen/blob/6d771fdef16e47a32eb2ebb20cb5e9d1f80cffba/pymatgen/symmetry/groups.py#L119)。

## Wyckoff位置如何确定

参考[计算特定晶体群的Wyckoff位置](https://github.com/Osgood001/crystal-symmetry/issues/3)，里面介绍了如何给出晶体的设计空间，即Wyckoff Position是确定晶体群之后晶体结构还能改变和调整的区间。

## 理论我都懂，怎么实操？

参考[晶体中的群及其计算工具](https://github.com/Osgood001/crystal-symmetry/issues/1)，这部分介绍了如何学习使用crystal server来处理各种与群结构相关的问题。核心结论是：非常推荐！他们的Server具有非常高的制作水准和非常完善的功能，推荐所有群论、群表示论学习者来玩和用。

## 有什么应用？

参考[手性声子](https://github.com/Osgood001/crystal-symmetry/issues/5)，这部分介绍了手性声子这部分课程的一些基础知识。核心结论是：所谓手性声子，就是分子除了振动之外的旋转，这给出了一种带有自旋角动量的声子。

另外，[晶体中的群及其计算工具](https://github.com/Osgood001/crystal-symmetry/issues/1)里面也提到了一些基于对称性来搜索铁电材料的方法。

## 还漏了啥？

本次会议的复习阶段，系统回顾了群论和群表示论的基础，由于作者已经学习过，并未进行记录，另外关于许多计算的细节，也并未一一给出。

群论在本次课程中占据重要的地位，几乎每次的内容都是微扰对称群展开的，参考[手性的基础](https://github.com/Osgood001/crystal-symmetry/issues/6)，其中介绍了大家都很熟悉的手性，但在此基础上还划分了Sohncke群，作为230种空间群的子群。

后面关系磁性材料的部分，我也没有记录，感兴趣的可以点击链接[查看和 Kimi 智能助手的对话］(https://kimi.moonshot.cn/share/cpqll59mqu0apbi53dcg)。

主要是考虑到磁矢量之后对称性的增加。在会议海报阶段，有同学也介绍了自旋空间群（Spin Space Group）据了解是考虑空间群的基础上，加上自旋的群变换，给出的一类新的群。

课程文件考虑到版权并未发布在这里，建议搜索蔻享学术  上海计算晶体学国际会议查看回放。

## 有啥收获？

尽管系统的学习过群论和空间群，这还是第一次系统梳理晶体中的层级，学习了空间群的HM符号系统，知道了Wyckoff位置的推导，并且了解和使用了非常强大的晶体学服务器网站，最有趣的是，对于这些群，还可以通过微扰、增加对称元素等方法，构建一个群的树状图，这些都是首次学习和使用，非常精彩。

相变是物理学，乃至自然界最司空见惯，但又最玄妙的现象之一。朗道认为，相变的本质是对称性破缺，而对称性的描述语言，就是群，本次关于Wyckoff Position Spliting的讨论，让我非常直观的理解了这一点。

推荐大家都来学习和了解这个美妙的理论，群论在晶体学中的应用，是我认为每一个想要学习或者学习过群论的人，都值得再了解的，也是它让我看到了群论的力量。


