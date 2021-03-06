# 后端Java书单

## 书单适合谁
* 转行或者大学科班基础薄弱的朋友

## 书单不适合谁
* 非全日制本科学历的以下的人。可能有人会说我歧视学历，但是就我个人来看，获得本科学历代表你至少是会动脑子的人，有较强于普通人的自控力。书单里面的书很多很多，涉及知识真的很广，如果你没拿到全日制本科学历，大概率是无法将这些东西看完，并掌握这些有益于你整个软件开发职业生涯的知识，如果你不幸学历未达标，也请不要气馁，请拿出证明我观点错误的勇气，挑战你自己。

## 我对计算机知识以及行业的理解

* 书单里面的书大多侧重原理基础跟一些代码层面的最佳实践。我个人的观点一直是你掌握了基础的东西，然后上层的东西就很容易理解了，如果你一直只了解抽象层面上面的事情，很多事情你是没法做的，很多书你也看不懂。例如一个新手Java转行的程序员，他可能根本无法理解Kafka为什么会存在零拷贝的技术，因为对新手开发工程师来讲，他用了一个系统调用从硬盘上读取了一个文件，他是不了解整个流程的细节的，对于新手开发工程师来讲，一个打开文件的方法或者类只是一个黑盒而已，我每次只是告诉盒子我要什么，然后盒子会给他一些东西，至于盒子内部的运作方式也许是他从未知晓过的事物。

* 关系数据库的SQL 它本身的抽象层次很高，又是一种声明式的语言，你只能告诉数据库我要什么，至于它内部的一个方式，你根本无从所知，这意味着熟练的软件工程师无法应用自己对数据结构的理解 对算法的理解去优化，只能去了解数据库的底层实现方式，然后在抽象层之上应用一些窍门去做优化的工作，最终开发工程师还是得回到SQL语言抽象层下面去了解数据库的实现，让黑盒变成对开发工程师透明的白盒。

* 在数据量场景小的情况下，其实一切的关于优化的问题都不是问题，因为这个时候你的优化只是浪费你的生命而已，你对SQL的优化，可能带来50ms的优化，或者你的后台业务系统用户根本不在乎多等上3秒钟再返回数据库的结果。

* 面试造火箭，上班拧螺丝，主要的一大原因还是市场上根本没有那么多岗位需要去造摩天大楼，绝大部分软件开发者都可以应付盖一个狗窝的工作，因为狗窝不大，如果你没盖好，可以推翻重来，大不了浪费一个下午。但是摩天大楼不一样，也许一个细微的环境做不到位，可能导致整个大楼的抗台风能力降低几个数量级，要知道很多摩天大楼都在楼顶安装了一种类似钟摆的玩意，这个东西造价还非常的贵。但是对于一个狗窝来讲，台风刮走了你的狗窝，你大不了再建一个，对一个狗窝进行地基加强，或者增加狗窝的抓地力，实在是一种不明智的做法。

* 识别什么是造狗窝的工作，什么是盖摩天大楼的工作是一个重要的能力，也许你每天都干着造狗窝的活，但是如果你想在激烈的软件开发工作就业市场获得良好的回报，那么请在业余时间了解并实践一下造摩天大楼的工作技能。

* 认识技术的局限性，大部分人有一种技术改变世界的想法，或者寄希望于技术能给他带来巨大的回报，但事实是大部分人可能无法通过技术改变命运，IT技术与其它技术并没有什么区别，如果你想谋得职业上的发展，或者获得世俗意义上的成功，那么请多关注一下代码之外的软技能。

## 我的后端书单

* Think in Java , 这本书确实不适合新手，因为作者编写的时候，就考虑过这本书的受众是有其它编程语言经验但是不了解Java语言特性的程序员，里面包含了多线程 GUI Java语法 设计模式 OOAD 等许多内容，当然大多只是相关的介绍，并没有过度的深入，但是对于1-2年转行的程序员来讲，它介绍了不少软件开发的理念还有编程相关东西，而且这些东西都是结合Java来讲的，本身确实是一本不错的书籍，可以拓宽1-2年转行程序员的视野。

* CSAPP 中文 深入理解计算机系统，第一这本书真的不深入 也谈不上理解，更多都是介绍性质的东西，而且本身这本书的阅读受众就是大一新生，一开始翻译这本书的人估计想搞个大新闻，上来就弄个 深入理解，然后一堆小白吓得根本不敢去看，Computer Systems: A Programmer's Perspective 实际上原文的标题翻译过来就是 以一个程序员的视角来了解计算机系统，说白了这本书是写给有一些基础的应用程序编写概念，但是不了解计算机系统背后做了什么事情的小白看的，千万不要以为这本书是一本什么很难懂的书，它真的只是写给大一新生看的书，读这本书你可以理解很多系统层面内存管理的方式，以及理解Redis为什么可以通过Fork的方式 全量dump内存到硬盘。

* 《Unix环境高级编程》 ，这本书我推荐的原因其实很简单，大部分后端程序员可能无法绕过Unix/Linux 这一套体系，虽然Linux的实现跟Unix大相径庭，但是他们的在使用跟系统调用上是有很多相似之处的，熟悉Unix编程是一个后端程序员的进阶必备之路。

* 《Unix网络编程》，推荐读这本书主要是为了了解认识操作系统的一些API应用，但是不推荐你直接去使用socket那套API去使用学习，因为使用C语言编写应用程序涉及到大量的内存申请跟内存回收等操作，如果你有兴趣深入了解手动管理内存编写程序的方式，可以先学习一下C语言。

* 《C程序设计》（c语言发明者写的那本） 跟 汇编语言基于Linux环境，我建议一起阅读学习。很多人说C语言难以学习，但其实C语言本身并没有存在太多设计上的问题，它难学的问题在于 它对汇编语言封装的不够，你必须结合汇编层面上的特性来学习C语言。实际上大部分程序员最早是在裸机上编写汇编程序，所以C语言为了讨好汇编语言用户，在设计层面上实际上是参考了汇编语言的，例如swtich case语法就模拟了汇编语言的jmp #address指令的行为。

* 《算法4th》 , 不推荐算法导论的原因在于做工程实践的工程师，没有必要去了解算法的形式证明，大多数人无非是使用并借鉴常见算法 数据结构的思想去解决实际工作中所遇到的问题，而我们通常无需对我们所写的代码做形式化论证，仅加以单元测试保证其在限制条件的正确性即可。

* 《敏捷软件开发—原则、模式与实践》 ， 推荐这本书的原因是希望能通过学习这本书掌握一些代码层面架构的设计，以及理解其中一些思想，我比较认同作者所说的一个观点，不要在最早的时候就开始进行设计，但是你不应该被同一个问题愚弄两次，举个例子

```java
private void callA(int a){
//do something
}

private void callB(int a){
//do something
}

public void main(){
  int a = 0;
  callA(a);
  callB(a);
}
```

* 当你再加入callC的时候，你应该考虑是否采用观察者模式，不要总是在同一个地方摔跟头。


* 《MySQL技术内幕:innodb引擎》 作为后台开发，肯定是要了解数据库的，这本书虽然有些老旧，有些东西也是翻译官方文档，但是还是推荐看一下，虽然MySQL官方文档介绍其实已经很完善了。

```未完待续...```
