---
id: 201
title: 十年学会程序设计
date: 2007-05-18T19:59:35+00:00
author: Eric
layout: page
guid: http://blog.youxu.info/fyi/21-days/
dsq_thread_id:
  - 336134934
---
<p style="text-align: center;">
  <h2 align="center">
    十年学会程序设计
  </h2>
  
  <p style="text-align: center;">
    <span style="font-family: 细明体; font-size: small;"><em><a href="http://www.norvig.com/index.html">Peter Norvig (Copyright 2001)</a></em> <a href="http://www.norvig.com/21-days.html">原文网址</a></span>
  </p>
  
  <pre></pre>
  
  <h3>
    为何大家如此匆忙?
  </h3>
  
  <p>
    走进任何一家书店，你会看到书架上一排不见尽头的放着如 <7天自学Java语言> 以及几天或者几小时学会Windows, 因特网或者Visual Basic 这类书。我在<a title="Amazon" href="http://www.amazon.com/">Amazon</a> 网上书店用一下的方式进行<a title="高级搜索" href="http://www.amazon.com/exec/obidos/tg/browse/-/468558/104-5938873-6579160">高级搜索</a>:
  </p>
  
  <p>
    <a title="出版年份: 1992以后　书名包括：“天” 和 “学习” 或 “自学”" href="http://www.amazon.com/exec/obidos/search-handle-url/ix=books&rank=%2Bfeaturedrank&fqp=power%01pubdate%3A%20after%201992%20and%20title%3A%20days%20and%0D%20%28title%3A%20learn%20or%20title%3A%20teach%20yourself%29&sz=25&pg=1/ref=s_b_np">出版年份: 1992以后　书名包括：“天” 和 “学习” 或 “自学”</a>
  </p>
  
  <p>
    得到了268条搜索结果，其中前78条都是计算机书（第79条是 <a title="30天学会孟加拉语" href="http://www.amazon.com/exec/obidos/ASIN/0781802245/">30天学会孟加拉语</a>）。 我用 “<a title="小时" href="http://www.amazon.com/exec/obidos/search-handle-url/ix=books&rank=%2Bfeaturedrank&fqp=power%01pubdate%3A%20after%201992%20and%20title%3A%20hours%20and%0D%20%28title%3A%20learn%20or%20title%3A%20teach%20yourself%29&sz=25&pg=3/ref=s_b_np">小时</a>&#8221; 代替“天” 作为关键字，得到了神奇般类似的结果：这次有253本书，前77本是计算机书， 第78本是 <a title="24小时自学语法和写作风格" href="http://www.amazon.com/exec/obidos/ASIN/0028638999/">24小时自学语法和写作风格</a>。排名前200的书中有96%是计算机书。
  </p>
  
  <p>
    由此可见，人们要不就是急着想学会计算机，要不就是计算机相比于其他事情太容易学会了。比如说把，没有书是写在几天弹奏贝多芬或几天学会量子物理，甚至也没有几天学会帮小狗打扮这样的书。
  </p>
  
  <p>
    让我们分析一下 <a title="三天学会Pascal语言" href="http://www.amazon.com/exec/obidos/ISBN=1556225679/4094-7934802-027992">三天学会Pascal语言</a> [英文网页] 这样的标题表达了什么意思：
  </p>
  
  <ul>
    <li>
      学会:
    </li>
  </ul>
  
  <p style="margin-left: 40px;">
    在 三天内，你没有时间去写几个有意义的程序，或者从成功和失败中学到东西。你也没时间跟有经验的程序员一起工作，所以也无法了解在真正编程是什么样子。简短 的说，就学会而言，时间显然不够。所以这些书只是浮于表面的熟悉，而不是深刻的理解。如同Alexander Pope 所说，一知半解是危险的。
  </p>
  
  <ul>
    <li>
      Pascal 语言:
    </li>
  </ul>
  
  <p style="margin-left: 40px;">
    三 天内你可能学会Pasacl语言的语法（如果你已经掌握一个类似的编程语言），但你无法学会如何合理运用这些语法。简言之，如果你是个Basic 程序员，你可以用Pascal 语言写出类似Basic 风格的程序，但你学不到Pascal语言的优点（还有缺点）到底在哪。重点是什么呢? <a title="Alan Perlis" href="http://www-pu.informatik.uni-tuebingen.de/users/klaeren/epigrams.html">Alan Perlis</a> 曾说: &#8220;如果编程语言不能影响你的编程思维，那就不值得去学.&#8221; 另一个可能是，你必须学会一点点Pascal语言（或是像VB语言、Javascript等），因为你需要跟现成的工具组合完成特定的工作。不过这个时候，你实际上学的不是怎么写程序，而是要学着如何完成工作。
  </p>
  
  <ul>
    <li>
      三天
    </li>
  </ul>
  
  <p style="margin-left: 40px;">
    不幸的是三天根本不够；下面的章节会告诉你为什么
  </p>
  
  <h3>
    十年学会程序设计
  </h3>
  
  <p>
    研究者 <a title="Hayes" href="http://www.amazon.com/exec/obidos/ASIN/0805803092">Hayes</a>, <a title="Bloom" href="http://www.amazon.com/exec/obidos/ASIN/034531509X/">Bloom</a> 的研究表明，在几乎所有的各种领域，大约要十年才能培养出专业技能。这些领域包括下西洋棋、音乐作曲、绘画、钢琴、游泳、网球，及神经心理学和数学拓扑学。似乎没有真正的捷径－－即便是莫扎特在四岁就展露出音乐天才，在他写出世界级的音乐之前仍然用了超过十三年的时间。
  </p>
  
  <p>
    再看另一种类型的领域。披头士乐团似乎是在１９６４年的Ed Sullivan 剧场表演突然地火起来并成为第一乐队的。但其实他们从 1957 年开始，就在利物浦、汉堡等地的小型俱乐部表演。虽然他们很早就显现强大的吸引力，但他们决定性的成功作品<span style="font-style: italic;"> Sgt Pepper</span> 也到1967年才发行。Samuel Johnson 则认为或许还不止十年才行，他说：任何领域的卓越成就都必须用一生的努力才能取得; 稍微低一点的代价都是换不到的。Chaucer 则感叹道： “生命如此短促，学习技艺却要这么地长”
  </p>
  
  <p>
    以下是我在编程上成功的秘诀:
  </p>
  
  <ul>
    <li>
      对编程产生感兴趣并因为乐趣而写程序。确信你自始至终都能乐在其中，这样你才愿意将十年光阴投入编程事业.
    </li>
    <li>
      与其他程序员交流；阅读别人的代码。这比任何书任何培训都重要。
    </li>
    <li>
      不断地编写。 最好的学习方法是<a title="在实践中学习" href="http://www.engines4ed.org/hyperbook/nodes/NODE-120-pg.html">在实践中学习</a> 。从技术角度说，&#8221;在特定领域的个人最高效率并不因为经验够多就会自动获得；但若有意识的通过努力去提升经验，个人效率会变高”（<a title="第336页" href="http://www2.umassd.edu/swpi/DesignInCS/expertise.html">第336页</a>）而 “高效的学习一般需要明确的任务和因人而异的适当难度，以及及时的反馈和重复或者修正错误的机会”（20～21页）<a title="Cognition in Practice: Mind, Mathematics, and Culture in Everyday Life" href="http://www.amazon.com/exec/obidos/ASIN/0521357349">Cognition in Practice: Mind, Mathematics, and Culture in Everyday Life</a> （<span style="font-style: italic;">实践中认知：心智、数学与日常文化</span>） 是这个观点的一本有趣参考书籍。
    </li>
    <li>
      如 果你愿意，你可以去读四年大学（或再读研究生）。这可以让你满足一些工作的学历要求，同时也可让你对这个领域有更深的认识。但如你不喜欢上学，你也能（得 有牺牲）通过工作获得类似的经验。无论如何，只读书是不够的。《New Hacker&#8217;s Dictionary》的作者Eric Raymond 曾经说过: “计算机的教育无法让人成为编程的专家，正如研究画笔与颜料不能让人成为专业画家一样.” 一个在我所有招聘过的人中属于最优秀之一的程序员只有高中毕业，但他写出很多<a title="很棒" href="http://www.xemacs.org/">很棒</a> 的<a title="程序" href="http://www.mozilla.org/">程序</a>，他甚至有自己的<a title="新闻组" href="http://groups.google.com/groups?q=alt.fan.jwz&meta=site%3Dgroups">新闻组</a>。他获得的股票期权使得他可以拥有自己的<a title="午夜酒吧" href="http://http//en.wikipedia.org/wiki/DNA_Lounge">午夜酒吧</a>.
    </li>
    <li>
      跟其他程序员一起完成项目。在一些项目中成为最好的程序员；在一些中则充当最差的一个。当你是最佳的，你要测试自己领导项目的能力，并以你的能力鼓励他人。当你是最差的，要看看高手做些什么，他们不喜欢做什么 (因为他们会叫你去帮他们做).
    </li>
    <li>
      接手别的程序员完成项目。全心投入并理解别人的程序。当原作者不在的时候，看看在理解与修改时有什么要注意的。想想如何设计你的程序使得后来维护的人容易上手。
    </li>
    <li>
      至 少学会六门编程语言。一种要支持类/对象(class abstractions)的语言, 如Java或C++; 一种函数式(functional abstraction)语言, 如 LISP 或 ML; 一种支持语法抽象(syntactic abstraction) 的语言 如 LISP; 一种声明式语言, 如Prolog或 C++模版; 一种支持协同式(coroutines)编程, 如 Icon 或 Scheme; 还有一种支持并行(parallelism)的语言, 如 Sisal.
    </li>
    <li>
      记住在 “计算机科学” 中包括&#8221;计算机&#8221; 这个词。要知道你的计算机执行一条指令需要多久，到内存中取一个字需要多久(缓存是否击中), 到磁盘读取连续的字需要多久，而磁盘的定位又需要多久. (解答见文末)
    </li>
    <li>
      进行语言标准化的工作。可以像是由ANSI　C++ 委员会，或由你自己的团队，来决定你们的编码风格，譬如说缩排是2或4个空格。不管怎样，你都能学到别人到底喜欢什么，对语言的感受有多深，甚至能了解到一点他们为什么有这样的感觉。
    </li>
    <li>
      并具备良好的判断力，也别老纠缠在语言标准化上.
    </li>
  </ul>
  
  <p>
    谈 了上面所有的想法后，我不禁要问究竟能从书上学到多少。在第一个孩子出生前，我读完了所有的 &#8220;怎样…&#8221; 的书，仍觉得自己是个一无所知的（照顾孩子的）菜鸟。30个月后，第二个孩子出世，我要重回这些书好好复习么? 不! 取而代之的是，我开始相信自己的个人经验。这些难得的经验，比专家写的几千页手册还要有用，而且让我重新找到了自信.
  </p>
  
  <p>
    Fred Brooks (译注: <人月神话>作者) 在他的文章 <a title="没有银弹" href="http://citeseer.nj.nec.com/context/7718/0">没有银弹</a> 中指出，发掘卓越软体设计者的三部曲：
  </p>
  
  <p>
    １．尽早尽可能地以系统化的方式发掘最佳设计人员。<br /> ２．给有潜力者指派生涯规划师，并谨慎地规划他们的职业生涯。<br /> ３．提供机会给正在成长的程序员，让他们能相互影响，彼此激励。
  </p>
  
  <p>
    这里假定了某些人已具备成为卓越设计师的必要潜能；工作只是诱导他们前进。<a title="Alan Perlis" href="http://www-pu.informatik.uni-tuebingen.de/users/klaeren/epigrams.html">Alan Perlis</a> 说得更简洁了，你可以教任何人学雕塑，但对米开朗基罗而言，要教他的<br /> 反倒是有哪些事不要做, 卓越的程序员也一样。
  </p>
  
  <p>
    所以，尽管买那些 Java 书吧！你或许能从中找到点有用的，但是在24小时，几天或者几个月中，这些都不会改变你的人生，你也不能掌握一个真正的程序员应该具备的真正的综合的技能。
  </p>
  
  <p>
    <br style="font-weight: bold;" /><span style="font-weight: bold;">参考文献:</span>
  </p>
  
  <p>
    Bloom, Benjamin (ed.) <em><a href="http://www.amazon.com/exec/obidos/ASIN/034531509X">Developing Talent in Young People</a></em>, Ballantine, 1985.
  </p>
  
  <p>
    Brooks, Fred, <em><a href="http://citeseer.nj.nec.com/context/7718/0">No Silver Bullets</a></em>, IEEE Computer, vol. 20, no. 4, 1987, p. 10-19.
  </p>
  
  <p>
    Hayes, John R., <em><a href="http://www.amazon.com/exec/obidos/ASIN/0805803092">Complete Problem Solver</a></em> Lawrence Erlbaum, 1989.
  </p>
  
  <p>
    Lave, Jean, <em><a href="http://www.amazon.com/exec/obidos/ASIN/0521357349">Cognition in Practice: Mind, Mathematics, and Culture in Everyday Life</a></em>, Cambridge University Press, 1988.
  </p>
  
  <p>
    ________________________________
  </p>
  
  <p>
    <a title="解答" name="解答"></a> <strong>解答</strong>:
  </p>
  
  <p>
    各种操作的时间，以2001年夏季，典型配置的 1GHz 个人计算机为标准：
  </p>
  
  <table border="1" cellspacing="0">
    <tr>
      <td>
        执行单一指令
      </td>
      
      <td>
        1 纳秒
      </td>
    </tr>
    
    <tr>
      <td>
        从L1 高速缓存取一个字
      </td>
      
      <td>
        2 纳秒
      </td>
    </tr>
    
    <tr>
      <td>
        从内存取一个字
      </td>
      
      <td>
        10 纳秒
      </td>
    </tr>
    
    <tr>
      <td>
        从磁盘取连续存放的一个字
      </td>
      
      <td>
        200 纳秒
      </td>
    </tr>
    
    <tr>
      <td>
        磁盘寻址并取字
      </td>
      
      <td>
        8 毫秒
      </td>
    </tr>
  </table>
  
  <p>
    ________________________________<br /> <br style="font-weight: bold;" /><span style="font-weight: bold;">附录 I: 语言的选择</span><br style="font-weight: bold;" /><br /> 好几个人问过我一开始应该先学哪个计算机编程语言，这个问题没有唯一的答案，不过选择的时候可以从以下的几个方面考虑：
  </p>
  
  <ul style="font-weight: bold;">
    <li>
      朋友在用的. <span style="font-weight: normal;">当 人们问我:&#8221;我该用什么操作系统的时候&#8221;， 我通常的回答是：“用你朋友用的”. 这样的好处是从朋友那儿学习可以弥补复杂的操作系统差异或者编程语言差异(给你造成的困惑)。这里也要考虑你未来的朋友：如果你一直使用的话，开发社区会 是你的朋友。你选择了一个具有有巨大的增长的开发社区还是一个小的快消失的开发社区的语言? 它有相关的书，网站和论坛可以获取解答么? 你喜欢那些论坛上的人么?</span>
    </li>
  </ul>
  
  <ul style="font-weight: bold;">
    <li>
      <span style="font-weight: bold;">保持简单. </span>诸如C++和Java 是为那些关心代码执行效率的有经验的大型团队的开发人员设计的。因此这些语言中有些为这些特殊场合设计的部件。你只是关心编程而不需要关心复杂情况。你需要一个为新学编程的人设计的容易学习和理解的语言。
    </li>
  </ul>
  
  <ul style="font-weight: bold;">
    <li>
      <span style="font-weight: bold;">实践. </span>什么是学习钢琴的好方法呢? 是一边听音一边弹奏的“交互式” 的方法呢，还是全听完整首歌然后再弹奏的那种“批处理”方式呢? 很显然, 交互学习的方式能够让学钢琴变得简单&#8211;这也适用于编程. 选取一种交互式的编程语言并且坚持使用.
    </li>
  </ul>
  
  <p>
    基于以上的这些标准，我对于第一次接触编程的人推荐 Python 或 Scheme. 但是情况各有不同，或许也有其他的选择. 如果你不满10岁，你可能会喜欢Alice 或者Squeak(年龄大的人或许也喜欢这些). 重要的是在选择后, 立即开始学习和使用.
  </p>
  
  <p style="font-weight: bold;">
    附录II: 书和其他资源:
  </p>
  
  <p>
    很多人问我该从什么书或者什么网页开始看起。我重申一句：“仅仅看书是不够的”，不过我也推荐一下的一些：
  </p>
  
  <ul>
    <li>
      <strong>Scheme:</strong> <a href="http://www.amazon.com/gp/product/0262011530">计算机程序的结构和释义 (Abelson & Sussman)</a> 可能是计算机科学最好的导论了, 他还告诉程序员怎么理解计算机科学, 你可以访问这本书的 <a href="http://www.swiss.ai.mit.edu/classes/6.001/abelson-sussman-lectures/">在线视频讲座</a> 和 <a href="http://mitpress.mit.edu/sicp/full-text/book/book.html">全文在线</a>. 这本书也很有挑战性，可能会排除掉一些可能在其他领域成功的人.
    </li>
  </ul>
  
  <ul>
    <li>
      <strong>Scheme:</strong> <a href="http://www.amazon.com/gp/product/0262062186">怎样设计程序(Felleisen <span style="font-style: italic;">等</span>)</a> 是讲解怎样设计优雅的函数式语言的最好的书之一.
    </li>
  </ul>
  
  <ul>
    <li>
      <strong>Python:</strong> <a href="http://www.amazon.com/gp/product/1887902996">Python 编程，面向计算机科学的导论 (Zelle)</a> 是用Python 介绍计算机科学的好书.
    </li>
  </ul>
  
  <ul>
    <li>
      <strong>Python:</strong> 一些关于Python的 <a href="http://wiki.python.org/moin/BeginnersGuide">入门教程</a> 可以在 <a href="http://python.org/">Python.org</a> 上找到.
    </li>
  </ul>
  
  <ul>
    <li>
      <strong>Oz:</strong> <a href="http://www.amazon.com/gp/product/0262220695">计算机编程的概念，技术和模型(Van Roy & Haridi)</a> 可以视为第一本书的现代版. 他是关于编程的一些总揽，包含了比第一本书更加广泛也更加容易阅读和理解的领域。这本书使用了一个不太为人所知的编程语言叫 Oz, 不过这个可以作为学习其他编程语言的一个基础。
    </li>
  </ul>
  
  <p>
    ________________________________
  </p>
  
  <p>
    注: T. Capey 指出，在Amazon 的 问题彻底解决者 的页面上购买了这本书的人还买了: &#8220;21天学孟加拉语&#8221; 和 &#8220;自学语法和写作风格&#8221; 这两本书，我估计大部分是我这个页面带过去的用户.
  </p>
  
  <p>
    <a title="Peter Norvig (Copyright 2001)" href="http://www.norvig.com/index.html">Peter Norvig (Copyright 2001)</a>
  </p>
  
  <p>
    <a title="Eric You XU" href="http://www.youxu.info/">Eric You XU</a> 翻译，2007年4月
  </p>
  
  <p>
    <br style="font-weight: bold;" /><span style="font-weight: bold;">译者附记:</span>
  </p>
  
  <p>
    这是一篇经典的揭示计算机学习和计算机编程领域浮躁苗头的文章。原有的中文翻译链接已经失效，因此特此重新翻译一次。在翻译的过程中，我参考了<a title="台湾网友" href="http://www.open-asm.com/article/tenyears.htm">台湾网友</a>的部分遣词造句以及个别我不能理解的句子的含义，特此向他表示感谢.
  </p>
  
  <p>
    如果有什么地方因为个人水平疏漏翻译不到或者打字错误的地方，恳请网友不吝指出。 我的邮件地址是 youxu A@T wustl.edu, 把 A@T 换成 @, 我叫Eric You XU, 你可以直接叫我Eric.
  </p>