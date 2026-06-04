# 序言

  本书是为操作系统课程编写的讲义草稿。它通过剖析一个名为 xv6 的教学内核，来阐述操作系统的核心概念。xv6 的设计原型取自 Dennis Ritchie 和 Ken Thompson 共同开发的 Unix Version 6 (v6) [^17]。xv6 在宏观上沿袭了 v6 的结构与代码风格，但在底层改用 ANSI C [^7] 重新编写，并适配了多核 RISC-V 架构 [^15]。

  阅读本书时应结合 xv6 的源代码同步对照。这种“源码+讲义”的学习模式深受 John Lions 的经典著作《UNIX 6th Edition 源码剖析》（*Lions' Commentary on UNIX 6th Edition*）[^11] 的启发；本书也包含了指向源码的超链接，对应的 GitHub 仓库位于 [mit-pdos/xv6-riscv](https://github.com/mit-pdos/xv6-riscv)。关于 v6 和 xv6 的更多在线资源（包括基于 xv6 设计的多个实验作业），请访问课程官网 [6.1810 课程主页](https://pdos.csail.mit.edu/6.1810)。

  本书已作为 MIT 操作系统课程（6.828 和 6.1810）的教材使用。我们衷心感谢这些课程中的授课教师、助教以及所有学生们，他们均直接或间接地为 xv6 的发展做出了贡献。特别鸣谢 Adam Belay、Austin Clements 和 Nickolai Zeldovich。

  最后，对于所有通过邮件向我们反馈文档 Bug 或提出改进建议的贡献者们，我们在此一并致以诚挚的谢意：
  Abutalib Aghayev, Sebastian Boehm, brandb97, Anton Burtsev, Raphael Carvalho, Tej Chajed, Brendan Davidson, Rasit Eskicioglu, Color Fuzzy, Wojciech Gac, Giuseppe, Tao Guo, Haibo Hao, Naoki Hayama, Chris Henderson, Robert Hilderman, Eden Hochbaum, Wolfgang Keller, Paweł Kraszewski, Henry Laih, Jin Li, Austin Liew, lyazj@github.com, Pavan Maddamsetti, Jacek Masiulaniec, Michael McConville, m3hm00d, Mes0903, miguelgvieira, Mark Morrissey, Muhammed Mourad, Harry Pan, Harry Porter, Siyuan Qian, Zhefeng Qiao, Askar Safin, Salman Shah, Huang Sha, Vikram Shenoy, Adeodato Simó, Ruslan Savchenko, Pawel Szczurko, Warren Toomey, tyfkda, tzerbib, Vanush Vaswani, Chen Wang, Xi Wang, and Zou Chang Wei, Sam Whitlock, Qiongsi Wu, LucyShawYang, ykf1114@gmail.com, 以及 Meng Zhou。

  如果您在阅读过程中发现任何错误，或有进一步的修改建议，请发送邮件至 Frans Kaashoek 和 Robert Morris (kaashoek,rtm@csail.mit.edu)。