# Interview-questions
面试题汇总
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">的意思</span></span></strong><strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; PHP</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是一个基于服务端来创建动态网站的脚本语言，您可以用PHP和HTML生成网站主页</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么事面向对象？主要特征是什么？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">面向对象是程序的一种设计方式，它利于提高程序的重用性，使程序结构更加清晰。主要特征：封装、继承、多态。</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">SESSION </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">与 COOKIE的区别是什么，请从协议，产生的原因与作用说明? </span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、http无状态协议，不能区分用户是否是从同一个网站上来的，同一个用户请求不同的页面不能看做是同一个用户。</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、SESSION存储在服务器端，COOKIE保存在客户端。Session比较安全，cookie用某些手段可以修改，不安全。Session依赖于cookie进行传递。</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">禁用cookie后，session不能正常使用。<strong>Session的缺点：</strong>保存在服务器端，每次读取都从服务器进行读取，对服务器有资源消耗。Session保存在服务器端的文件或数据库中，默认保存在文件中，文件路径由php配置文件的session.save_path指定。Session文件是公有的。</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">不使用cookie向客户端发送一个cookie. </span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">理解：session_start（）开启时，生成一个常量 SID，当COOKIE开启时，这个常量为空，当COOKIE关闭时，这个常量中存储了PHPSESSID的值。通过在URL后加一个SID参数来传递SESSIONID的值，从而使客户端页面可以使用SESSION里面的值。 当客户端开启COOKIE和服务器端开启SESSION时。 浏览器第一次请求，服务器会向浏览器端发送一个COOKIE里面存储SESSIONID. 当浏览器第二次请求时，会把已存在的COOKIE一起提交到服务器端。</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述Cookie的设置及获取过程</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">设置COOKIE的值：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Setcookie(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">名称，值，保存时间，有效域);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取值：$_COOKIE[&#39;名称&#39;];</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">HTTP </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">状态中302、403、 500、<span style="color:#333333">200</span><span style="color:#333333">、404、502</span>代码含义？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">一二三四五原则: 一. 消息系列&nbsp; 二. 成功系列&nbsp;&nbsp; 三. 重定向系列&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 四. 请求错误系列&nbsp;&nbsp;&nbsp;&nbsp; 五. 服务器端错误系列 &nbsp;302:临时转移成功，请求的内容已转移到新位置 403:禁止访问 500:服务器内部错误 401代表未授权。 </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:gray">200</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:gray">是请求成功，404是文件未找到，502是服务器内部错误。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出数据类型(int char varchar datetime text)的意思；请问 varchar 和 char有什么区别？</span></span></strong>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">19、</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Int </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">整数 char 定长字符 Varchar 变长字符 Datetime 日期时间型 Text 文本型 <strong>Varchar 与char的区别</strong> char是固定长度的字符类型，分配多少空间，就占用多长空间。 Varchar是可变长度的字符类型，内容有多大就占用多大的空间，能有效节省空间。 Varchar是变长，节省存储空间，char是固定长度。查找效率要char型快，因为varchar是非定长，必须先查找长度，然后进行数据的提取，比char定长类型多了一个步骤，所以效率低一些</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">MyISAM </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和 InnoDB 的基本区别？索引结构如何实现？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">MyISAM</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">类型不支持事务处理等高级处理，而InnoDB类型支持。MyISAM类型的表强调的是性能，其执行速度比InnoDB类型更快，但是不提供事务支持，而InnoDB提供事务支持以及外部键等高级数据库功能。</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">创建索引：alert table tablename add index (`字段名`)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">isset() </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和 empty() 区别</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;Isset</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">判断变量是否存在，如果存在则返回真，empty判断变量是否为空为假，如果为空为假则返回真。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">include</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">与require的区别?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1.include()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在执行文件时每次都要进行读取和评估</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; require()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">文件只处理一次(实际上文件内容替换了require()语句)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2.require()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">通常放在PHP脚本程序的最前面</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp; include()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的使用和require()一样,一般放在流程控制的处理区段中,PHP脚本文件读到include()语句时,才将它包含的文件读进来,这种方式,可以把程序执行时的流程简单化</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3,require()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">和include()语句是语言结构,不是真正的函数,可以像PHP的其他语言结构一样</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4,include_once()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">和require_once()语句也是在脚本执行期间包括并运行指定文件,与include()require()唯一的区别是如果文件中的代码已经被包括了,则不会再次包括.</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5,require()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">包含文件失败,停止执行,给出错误(致命的)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">include()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">常用于动态包含.</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">通常是自动加载的文件,即使加载出错,整个程序还是继续执行</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">一个页面声明,另一个页面调用</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">包函文件失败,继续向下执行,返回一条警告</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">字符串中单引号与双引号的区别?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">单引号不能解释变量，而双引号可以解释变量。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">单引号不能转义字符，在双引号中可以转义字符。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <a></a><a><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">请说明 PHP 中传值与传引用的区别。什么时候传值什么时候传引用？</span></span></strong></a><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#969696"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">按值传递：函数范围内对值的任何改变在函数外部都会被忽略</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; &nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">按引用传递：函数范围内对值的任何改变在函数外部也能反映出这些修改</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; &nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">优缺点：按值传递时，php必须复制值。特别是对于大型的字符串和对象来说，这将会是一个代价很大的操作。按引用传递则不需要复制值，对于性能提高很有好处。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function test(&amp;$a)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=$a+100;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b=1;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $b;//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出１</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">test($b);&nbsp;&nbsp; //</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">这里$b传递给函数的其实是$b的变量内容所处的内存地址，通过在函数里改变$a的值　就可以改变$b的值了</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo &quot;&lt;br&gt;&quot;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $b;//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出101</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">in, not ni, exist, not exist</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">的作用和区别？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">in</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在什么中</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Not in </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不在什么中</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Exists </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">存在</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Not exists </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不存在</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">面向对象中接口和抽象类的区别及应用场景?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、有抽象方法的类叫做抽象类，抽象类中不一定有抽象方法，抽象方法必须使用abstract关键字定义。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、接口中全部是抽象方法,方法不用使用abstract定义。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、当多个同类的类要设计一个上层，通常设计为抽象类，当多个异构的类要设计一个上层，通常设计为接口。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo(),print(),print_r()</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">的区别？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是PHP语句, print和print_r是函数,语句没有返回值,函数可以有返回值(即便没有用)&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; Print()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">只能打印出简单类型变量的值(如int,string)&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; print_r()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">可以打印出复杂类型变量的值(如数组,对象)&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; echo&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出一个或者多个字符串</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">mysql_fetch_row() </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和mysql_fetch_array之间有什么区别?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysql_fetch_row()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">以索引数组的方式取查询的结果集，mysql_fetch_array()以索引数组和关联数组两种方式取查询的结果集。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请描述出两点以上XHTML和HTML最显著的区别<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(1)XHTML</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">必须强制指定文档类型DocType，HTML不需要<br/> (2)XHTML所有标签必须闭合，HTML比较随意</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">33. HTTP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">协议中GET、POST和HEAD的区别？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">HEAD</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">： 只请求页面的首部。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">GET</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">： 请求指定的页面信息，并返回实体主体。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">POST</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">： 请求服务器接受所指定的文档作为对所标识的URI的新的从属实体。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（1）HTTP 定义了与服务器交互的不同方法，最基本的方法是 GET 和 POST。事实上 GET 适用于多数请求，而保留 POST 仅用于更新站点。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（2）在FORM提交的时候，如果不指定Method，则默认为GET请 求，Form中提交的数据将会附加在url之后，以?分开与url分开。字母数字字符原样发送，但空格转换为“+“号，其它符号转换为%XX,其中XX为 该符号以16进制表示的ASCII（或ISO Latin-1）值。GET请求请提交的数据放置在HTTP请求协议头中，而POST提交的数据则放在实体数据中；</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">GET</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方式提交的数据最多只能有1024字节，而POST则没有此限制。</span>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（3）</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">GET </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">这个是浏览器用语向服务器请求最常用的方法。POST这个方法也是用来传送数据的，但是与GET不同的是，使用POST的时候，数据不是附在URI后面传递的，而是要做为独立的行来传递，此时还必须要发送一个Content_length标题，以标明数据长度，随后一个空白行，然后就是实际传送的数据。网页的表单通常是用POST来传送的。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">表单中 get与post提交方法的区别?<br/> </span></span></strong>　<span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1. get</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是把参数数据队列加到提交表单的ACTION属性所指的URL中，值和表单内各个字段一一对应，在URL中可以看到。post是通过HTTP post机制，将表单内各个字段与其内容放置在HTML HEADER内一起传送到ACTION属性所指的URL地址。用户看不到这个过程。</span>
</p>
<p style="line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　　2. 对于get方式，服务器端用Request.QueryString获取变量的值，对于post方式，服务器端用Request.Form获取提交的数据。</span>
</p>
<p style="line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　　3. get传送的数据量较小，不能大于2KB。post传送的数据量较大，一般被默认为不受限制。但理论上，IIS4中最大量为80KB，IIS5中为100KB。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">get</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">安全性非常低，post安全性较高。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">foo()</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和@foo()之间有什么区别?(1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; @foo()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">控制错误输出</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">线性表和顺序表的区别？</span></span></strong>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、线性表包括顺序表和链表。</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、顺序表中的元素的地址是连续的，链表里面节点的地址不是连续的，是通过指针连起来的。</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么是数据库索引，主键索引，唯一索引的区别，索引的缺点是什么？</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">索引用来快速地寻找那些具有特定值的记录。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">主键索引和唯一索引的区别：主键是一种唯一性索引，但它必须指定为“PRIMARY&nbsp;KEY”,每个表只能有一个主键。唯一索引索引列的所有值都只能出现一次，即必须唯一。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">索引的缺点：</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、创建索引和维护索引要耗费时间，这种时间随着数据量的增加而增加。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、索引需要占用物理空间，除了数据表占数据空间之外，每一个索引还要占一定的物理空间，如果要建立聚簇索引，需要的空间就会更大。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、当对表中&nbsp;的数据进行增加、删除、修改的时候，索引也要动态的维护，这样就降低了数据的维护速度。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">浏览器IE和非IE浏览器的划分，区别是什么？</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">IE</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">浏览器指的是使用IE内核的浏览器，对一些W3C标准的网页代码的支持不是很好。</span>
</p>
<p style=";margin-bottom:0;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">非IE浏览器指的是没有使用IE内核的浏览器，对W3C标准的网页代码有很好的支持。</span>
</p>
<p style=";margin-bottom:0;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数据库中的事务是什么?</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">事务（transaction）是作为一个单元的一组有序的数据库操作。如果组中的所有操作都成功，则认为事务成功，即使只有一个操作失败，事务也不成功。如果所有操作 完成，事务则提交，其修改将作用于所有其他数据库进程。如果一个操作失败，则事务将回滚，该事务所有操作的影响都将取消。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">解释:左连接,右连接,内连接,索引。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、內连接仅选出两张表中互相匹配的记录．因此，这会导致有时我们需要的记录没有包含进来。内部连接是两个表中都必须有连接字段的对应值的记录，数据才能检索出来。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、左连接和右连接都是外部连接，也就是区别于内部连接，它对不满足连接条件的行并不是象内部连接一样将数据完全过滤掉，而是保留一部分数据，行数不会减少。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、左连接是只要左边表中有记录，数据就能检索出来，而右边有的记录必要在左边表中有的记录才能被检索出来</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、右连接是只要右边表中有记录，数据就能检索出来 ；</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、全连接则会回返回两个表中的所有记录</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述0000000中无限分类的实现原理。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、数据库分类表的设计：id字段、父id字段、类名称字段、path字段</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Path字段存当前分类的路径，格式：0,父类id,本身id</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、查询分类：select * from 分类表order by path asc;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、这样就查出来每个分类及其对应的子类。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">能够使html和php分离开使用的模板？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Smarty</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、template、PHPlibTemplate、FastTemplate</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用那些工具进行版本控制？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Clear case</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、CVS、SVN、PVCS、Perforce、CCC、StarTeam、RCS</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出三种以上MySQL数据库存储引擎的名称（提示：不区分大小写）</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> MyISAM</span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、InnoDB、BDB（Berkeley DB）、Merge、Memory（Heap）、Example、Federated、Archive、CSV、Blackhole、MaxDB 等等十几个引擎</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么是模板技术、能够使HTML和PHP分离开使用的模板？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">模板技术就是使程序的逻辑代码和界面分开的技术。</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">能够使HTML和PHP分开的模板有：<a></a><a>Smarty、Template、PHPlib Template、FastTemplate</a></span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">实现中文字串截取无乱码的方法</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mb_substr();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用PHP写出显示客户端IP与服务器IP的代码</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取客户端IP：get_env(“REMOTE_ADDR”);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取服务器端IP：$_SERVER[&quot;SERVER_ADDR&quot;];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数据库索引有几类，分别是什么？什么时候该用索引？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">普通索引、主键索引、唯一索引</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">并非所有的数据库都以相同的方式使用索引，作为通用规则，只有当经常查询列中的数据时才需要在表上创建索引。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写几个魔术方法并说明作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__call()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当调用不存在的方法时会自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__autoload()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在实例化一个尚未被定义的类是会自动调用次方法来加载类文件</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__set()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当给未定义的变量赋值时会自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__get()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当获取未定义变量的值时会自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__construct()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">构造方法，实例化类时自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__destroy()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">销毁对象时自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__unset()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当对一个未定义变量调用unset()时自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__isset()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当对一个未定义变量调用isset()方法时自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__clone()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">克隆一个对象</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">__tostring()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当输出一个对象时自动调用的方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$_REQUEST</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">、$_POST、$_GET、$_COOKIE、$_SESSION、$_FILE的意思是什么？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">它们都是PHP预定义变量</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_REQUEST</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取post或get方式提交的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_POST</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取post方式提交的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_GET</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取get方式提交的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_COOKIE</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取cookie存储的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_SESSION</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取session存储的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_FILE</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来获取上传文件表单的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数组中下标最好是什么类型的，为什么？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">数组的下标最好是数字类型的，数字类型的处理速度快。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">++i</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和i++哪一个效率高，为什么？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">++i</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">效率比i++的效率更高，因为++i少了一个返回i的过程。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">magic_quotes_gpc()</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">、magic_quotes_runtime()的意思是什么？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Magic_quotes_gpc()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是php配置文件中的，如果设置为on则会自动POST,GET,COOKIE中的字符串进行转义，在‘之前加\</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Magic_quotes_runtime()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是php中的函数，如果参数为true则会数据库中取出来的单引号、双引号、反斜线自动加上反斜杠进行转义。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">框架中什么是单一入口和多入口，单一入口的优缺点？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、多入口就是通过访问不同的文件来完成用户请求。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">单一入口只web程序所有的请求都指向一个脚本文件的。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、单一入口更容易控制权限，方便对http请求可以进行安全性检查。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">缺点：URL看起来不那么美观，特别是对搜索引擎来说不友好。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你对Memcach的理解，优点有哪些？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Memcache</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是一种缓存技术，在一定的时间内将动态网页经过解析之后保存到文件，下次访问时动态网页就直接调用这个文件，而不必在重新访问数据库。使用memcache做缓存的好处是：提高网站的访问速度，减轻高并发时服务器的压力。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Memcache</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的优点：稳定、配置简单、多机分布式存储、速度快。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">对关系型数据库而言，索引是相当重要的概念，请回答有关索引几个问题:</span></strong>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">a) </span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">索引的目的是什么?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、快速访问数据表中的特定信息，提高检索速度</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、创建唯一性索引，保证数据库表中每一行数据的唯一性</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、加速表和表之间的连接</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用分组和排序子句进行数据检索时，可以显著减少查询中分组和排序的时间</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">b) </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">索引对数据库系统的负面影响是什么?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">负面影响：创建索引和维护索引需要耗费时间，这个时间随着数据量的增加而增加；索引需要占用物理空间，不光是表需要占用数据空间，每个索引也需要占用物理空间；当对表进行增、删、改的时候索引也要动态维护，这样就降低了数据的维护速度。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">c) </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">为数据表建立索引的原则有哪些?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、在最频繁使用的、用以缩小查询范围的字段上建立索引</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、在平频繁使用的、需要排序的字段上建立索引</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">d) </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么情况下不宜建立索引?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、对于查询中很少涉及的列或者重复值比较多的列，不宜建立索引</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、对于一些特殊的数据类型，不宜建立索引，比如文本字段(text)等。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">web</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">应用中,数据库的读取频率远高于写入频率, 如何优化MySQL而应对此种情景?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用memcache缓存技术，将动态数据缓存到文件，访问动态页面时直接调用缓存文件，而不必重新访问数据库，这样就减少了查询数据库的次数。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">如果网站的访问量很大，可以把数据库读写服务器分开，使用多态服务器去处理数据库查 询，使用较少的服务器去处理数据库的写入和修改。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如果是一个Web频繁访问的查询，上题的查询如何优化？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用memcache缓存技术，在一定时间内将动态内容缓存到文件中，访问动态页面时，世界调用缓存文件而不必重新查询数据库。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数据库设计时，常遇到的性能瓶颈有哪些，常有的解决方案？</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">瓶颈主要有：</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、磁盘搜索&nbsp;优化方法是：将数据分布在多个磁盘上</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、磁盘读/写&nbsp;优化方法是：从多个磁盘并行读写。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、CPU周期&nbsp;优化方法：扩充内存</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、内存带宽&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请举例说明在你的开发过程中用什么方法来加快页面的加载速度</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">要用到服务器资源时才打开，及时关闭服务器资源，数据库添加索引，页面可生成静态，图片等大文件单独服务器。使用代码优化工具。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">描述一下大流量高并发量网站的解决方案</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、确认服务器硬件是否足够支持当前的流量。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用memcache缓存技术，将动态数据缓存到内存中，动态网页直接调用这些文件，而不必在访问数据库。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、禁止外部的盗链。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、外部网站的图片或者文件盗链往往会带来大量的负载压力，因此应该严格限制外部对自身图片或者文件盗链，目前可以简单的通过refer来控制盗链，apache自己就可以通过配置来禁止盗链。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、控制大文件的下载。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">大文件的下载会占用很大的流量，对于非SCSI硬盘来说会消耗，使得网站响应能力下降。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用不同的主机分流主要流量</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 7</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用流量统计软件。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在网站上安装一个流量统计软件，可以即时知道哪些地方耗费了大量流量，哪些页面需要再进行优化。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 8</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、分库分表。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 9</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Sphinx全文索引引擎。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">对于大流量的网站,您采用什么样的方法来解决访问量问题?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">优化程序，优化数据库，如果程序和数据库已经最优化，使用以下解决方法：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、确定当前服务器设备是否满足流量需求。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用Memcache缓存技术，把动态内容缓存到文件中，动态网页直接调用这些文件，而不必再访问数据库。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、禁止外部盗链，图片和文件外部盗链会给服务器带来大量的负载压力，可以通过refer来禁止外部盗链，或者使用apache来配置禁止盗链。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、控制大文件的下载，大文件的下载对于非SCSI硬盘来说会占用大量的资源，导致服务器的响应能力下降。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用不同的主机分流主要流量，使服务器均衡负载。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用流量统计软件统计分析网站流量，可以知道哪些地方耗费了大量的流量，哪些页面需要再进行优化。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何设计或配置Mysql，才能达到高效使用的目的。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、数据库设计方面，设计结构良好的数据库，允许部分数据冗余。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">选取最适用的字段属性，尽可能把字段设置为NOTNULL，这样在查询的时候，数据库不用去比较NULL值。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、系统架构设计方面，表散列，把海量数据散列到几个不同的表里面，集群，数据库查询和写入分开。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">写高效sql语句，以提高效率。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用连接(join)来代替子查询</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用联合(union)来代替手动创建的临时表</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">所得皆必须，只从数据库取必须的数据。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">必要的时候用不同的存储引擎，比如Innodb可以减少死锁，HEAP可以提高一个数量级的查询速度。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用事务</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用外键</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用索引</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">设定网站的用户数量在千万级，但是活跃用户的数量只有1%，如何通过优化数据库提高活跃用户的访问速度？</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">我们可以根据用户的活跃程度，把活跃的用户提取出来放到另外一张表里面，每次活跃的用户登陆的时候就直接到活跃用户表中进行查询，这样就提高了数据库的查询速度。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">了解XSS攻击吗? 如何防止 ?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">XSS</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是跨站脚本攻击，首先是利用跨站脚本漏洞以一个特权模式去执行攻击者构造的脚本，然后利用不安全的Activex控件执行恶意的行为。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用htmlspecialchars()函数对提交的内容进行过滤，使字符串里面的特殊符号实体化。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">SQL</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">注入漏洞产生的原因 ? 如何防止?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">SQL</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">注入产生的原因：程序开发过程中不注意规范书写sql语句和对特殊字符进行过滤，导致客户端可以通过全局变量POST和GET提交一些sql语句正常执行。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">防止SQL注入：</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、开启配置文件中的magic_quotes_gpc和magic_quotes_runtime设置</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、执行sql语句<em>时</em>使用addslashes进行sql语句转换</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Sql语句书写尽量不要省略小引号和单引号</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、过滤掉sql语句中的一些关键字：update、insert、delete、select、*</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、提高数据库表和字段的命名技巧，对一些重要的字段根据程序的特点命名，取不易被猜到的。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Php配置文件中设置register_globals为off，关闭全局变量注册</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">7</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、控制错误信息，不要再浏览器上输出错误信息，将错误信息写到日志文件中。</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何进行防SQL注入？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">&nbsp;1</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、过滤掉一些常见的数据库操作关键字：select,insert,update,delete,and,*等</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">或者通过系统函数：addslashes(需要被过滤的内容)来进行过滤。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、在PHP配置文件中</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Register_globals=off;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">设置为关闭状态 //作用将注册全局变量关闭。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">比如：接收POST表单的值使用$_POST[&#39;user&#39;],如果将register_globals=on;直接使用$user可以接收表单的值。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、SQL语句书写的时候尽量不要省略小引号(tab键上面那个)和单引号</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、提高数据库命名技巧，对于一些重要的字段根据程序的特点命名，取不易被猜到的</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、对于常用的方法加以封装，避免直接暴漏SQL语句</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、开启PHP安全模式</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Safe_mode=on;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 7</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、打开magic_quotes_gpc来防止SQL注入</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; Magic_quotes_gpc=off;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">默认是关闭的，它打开后将自动把用户提交的sql语句的查询进行转换，把&#39;转为\&#39;，这对防止sql注入有重大作用。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">因此开启：magic_quotes_gpc=on;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 8</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、控制错误信息</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">关闭错误提示信息，将错误信息写到系统日志。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 9</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、使用mysqli或pdo预处理。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用PHP写出一个安全的用户登录系统需要注意哪些方面。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、密码要使用MD5(密码+字符串)进行加密。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、登录表单的名称不要跟数据库字段一样，以免暴漏表字段。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、用户表的表名、字段名、密码尽量用不容易被猜到的。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、要使用验证码验证登陆，以防止暴力破解。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、验证提交的数据是不是来自本网站。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、登录后台处理代码数据库部分使用预处理，做好过滤，防止sql注入。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何实现多个线程安全的写入一个文件数据。</span></span></strong>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">采用锁机制，当一个用户在对此文件进行读写入操作时，将此文件锁定，操作完毕后解除锁定，在该用户进行读写入操作过程中，其他用户不能操作此文件，需要排队等待。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么是满二叉树？什么事完全二叉树？</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">满二叉树：除了叶子节点外的所有节点都有两个子节点。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">完全二叉树：每个节点最多有两个子节点，缺右不缺左，而且最多只能缺少一个叶子节点。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">字符串转数组,数组转字符串,字符串截取,字符串替换,字符串查找的函数分别是什么?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; Implode()</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、explode()、substr()、str_replace()、strpos、strrpos、strstr</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">GD</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">库是做什么用的? (1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> gd</span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">库提供了一系列用来处理图片的API，使用GD库可以处理图片，或者生成图片。 </span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在网站上GD库通常用来生成缩略图或者用来对图片加水印或者对网站数据生成报表。<br/> 在网站上GD库通常用来生成缩略图或者用来对图片加水印或者对网站数据生成报表。</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">John</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出Zend框架的目录结构，简单说明目录作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">application/ – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">存放应用程序的目录，包括 MVC 系统、配置文件、服务以及引导程序（Bootstrap.php）</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; configs/ –</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">配置文件目录。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; application/modules&nbsp;&nbsp; – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">多模块目录结果例如admin(后台前程),default(前台),shop（商城）各个模块下都有自己的controllers，modules，Views</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; controllers/models/views/ – </span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">控制器/模型/视图 目录。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; application/cache –</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">存放缓存等数据</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; application/helpers/ – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">这个是存放“行动助手”（action helper）的目录。这些助手类默认的命名空间是“Controller_Helper_”，如果是多模块那么命令空间将是“&lt;Module&gt;_Controller_Helper”。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Bootstrap.php – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">这个是应用程序入口文件。这个类的主要工作是引导应用程序，注册并初始化组件（component）。注意：不要在这个文件调用前置控制器（front controller）的dispatch() 方法。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">library/ – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">存放类库的目录。第三方的类库和自己写的类库放在这里进行自动 加载 但要注意要用自己独立的命名空间（建子目录）。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">public/ – </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">存放公开文件的目录，也即网站的根目录，存放可以被用户访问的文件，例如js、css和图片等等。index.php 是应用程序的单入口，其主要工作是建立php环境，引用Bootstrap.php来初始化，并调用前置控制器的dispatch()方法来分发请求。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">谈谈对mvc的认识？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">由模型(model),视图(view),控制器(controller)完成的应用程序<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 由模型发出要实现的功能到控制器,控制器接收组织功能传递给视图;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">MVC</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是一个设计模式，它强制性的使应用程序的输入、处理和输出分开。使用MVC应用程序被分成三个核心部件：模型、视图、控制器。它们各自处理自己的任务。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">视图是用户看到并与之交互的界面。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">模型表示企业数据和业务规则。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">控制器接受用户的输入并调用模型和视图去完成用户的需求。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">MVC</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的优点：低耦合性、高重用性和可适用性、较低的生命周期成本、快速的部署、可维护性、可扩展性，有利于软件工程化管理</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">MVC</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的缺点：没有明确的定义，完全理解MVC并不容易。不适合小型规模的应用程序。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何抛出和接收错误？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用try...catch，异常的代码放在try代码块内，如果没有触发异常，则代码继续执行，如果异常被触发，就会抛出一个异常。Catch代码块捕获异常，并创建一个包含异常信息的对象。$e-&gt;getMessage()，输出异常的错误信息。</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;"><a href="http://www.mianwww.com/html/2012/01/12879.html"><span style="color:windowtext">PHP</span><span style="color:windowtext">的网站主要攻击方式有哪些？</span></a> </span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、命令注入(Command Injection)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、eval注入(Eval Injection)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、客户端脚本攻击(Script Insertion)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、跨网站脚本攻击(Cross Site Scripting, XSS)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、SQL注入攻击(SQL injection)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">6</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、跨网站请求伪造攻击(Cross Site Request Forgeries, CSRF)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">7</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Session 会话劫持(Session Hijacking)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">8</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Session 固定攻击(Session Fixation)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">9</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、HTTP响应拆分攻击(HTTP Response Splitting)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">10</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、文件上传漏洞(File Upload Attack)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">11</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、目录穿越漏洞(Directory Traversal)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">12</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、远程文件包含攻击(Remote Inclusion)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">13</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、动态函数注入攻击(Dynamic Variable Evaluation)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">14</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、URL攻击(URL attack)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">15</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、表单提交欺骗攻击(Spoofed Form Submissions)</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">16</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、HTTP请求欺骗攻击(Spoofed HTTP Requests)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">几个重要的php.ini选项</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Register Globals</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">php&gt;=4.2.0</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">，php.ini的register_globals选项的默认值预设为Off，当register_globals的设定为On时，程序可以接收来自服务器的各种环境变量，包括表单提交的变量，而且由于PHP不必事先初始化变量的值，从而导致很大的安全隐患。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">safe_mode</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">安全模式，PHP用来限制文档的存取、限制环境变量的存取，控制外部程序的执行。启用安全模式必须设置php.ini中的safe_mode = On</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span></strong><strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、限制文件存取</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">safe_mode_include_dir = “/path1:/path2:/path3″</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不同的文件夹用冒号隔开</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span></strong><strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、限制环境变量的存取</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">safe_mode_allowed_env_vars = string</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">指定PHP程序可以改变的环境变量的前缀，如:safe_mode_allowed_env_vars = PHP_ ,当这个选项的值为空时，那么php可以改变任何环境变量</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">safe_mode_protected_env_vars = string</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来指定php程序不可改变的环境变量的前缀</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span></strong><strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、限制外部程序的执行</span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">safe_mode_exec_dir = string</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">此选项指定的文件夹路径影响system、exec、popen、passthru，不影响shell_exec和“` `”。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">disable_functions = string</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不同的函数名称用逗号隔开，此选项不受安全模式影响</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">magic quotes</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来让php程序的输入信息自动转义，所有的单引号(“’”)，双引号(“””)，反斜杠(“\”)和空字符(NULL)，都自动被加上反斜杠进行转义</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">magic_quotes_gpc = On </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">用来设置magic quotes 为On，它会影响HTTP请求的数据(GET、POST、Cookies)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">程序员也可以使用addslashes来转义提交的HTTP请求数据，或者用stripslashes来删除转义</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用过哪些PHP框架。试描述其优劣点。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、BroPHP框架：</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">优点：轻量级学习型框架，配置简单，操作简单，容易上手，提供了比较全面的文档。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">缺点：</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、ThinkPHP框架：</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">优点：功能比较全面，配置相对比较简单，操作相对比较简单，有很多使用示例程序。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">缺点：提供的操作方法太多，新手不知如何选择，文档不够全面。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">php</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">中,模板引擎的目的是什么? 你用过哪些模板引擎?</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用模板引擎的目的是使程序的逻辑代码和html界面代码分离开，是程序的结构更清晰。</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">使用过的模板引擎：Smarty、ThinkPHP的ThinkTemplate</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">7. </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何在页面之间传递变量(至少两种方式) ? &nbsp;&nbsp;</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">GET,POST,COOKIE,SESSION</span>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">8. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所知道的php数组相关的函数？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">创建数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_combine()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">通过合并两个数组来创建一个新数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">range()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">创建并返回一个包含指定范围的元素的数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">compact()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">建立一个数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_chunk()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">将一个数组分割成多个</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_merge()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">把两个或多个数组合并成一个数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_slice()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在数组中根据条件取出一段值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_diff()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">返回两个数组的差集数组</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_intersect()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">计算数组的交集</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_search()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在数组中搜索给定的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_splice()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">移除数组的一部分且替代它</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_key_exists()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">判断某个数组中是否存在指定的key</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">shuffle()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">把数组中的元素按随机顺序重新排列</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_flip()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">交换数组中的键和值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_reverse()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">将原数组中的元素顺序翻转，创建新的数组并返回</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">array_unique()----</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">移除数组中重复的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所知道的PHP的一些技术（smarty等）？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Smarty,jquery,ajax,memcache,div+css,js,mysqli,pdo,svn,thinkphp,brophp,yii</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所熟悉的PHP论坛系统 有哪些？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Discuz</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所熟悉的PHP商城系统 有哪些？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Ecshop</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所熟悉的PHP开发框架 有哪些？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Brophp,thinkphp</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你所知道的设计模式有哪些？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">工厂模式、策略模式、单元素模式、观察者模式、命令链模式</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">说说你对代码管理的了解？ 常使用那些代码版本控制软件？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">通常一个项目是由一个团队去开发，每个人将自己写好的代码提交到版本服务器，由项目负责人按照版本进行管理，方便版本的控制，提高开发效率，保证需要时可以回到旧版本。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">常用的版本控制器：SVN</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">说说你对SVN的了解？优缺点？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">SVN</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">是一种版本控制器，程序员开发的代码递交到版本服务器进行集中管理。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">SVN</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的优点：代码进行集中管理，版本控制容易，操作比较简单，权限控制方便。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">缺点：不能随意修改服务器项目文件夹。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">怎么找到PHP.ini的路径？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">一般都在php的安装目录下，或者window系统的windows目录下。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">加速模式/扩展？ PHP调试模式/工具？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Zend Optimizer</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">加速扩展</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">调试工具：xdebug</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你常用到的mysql命令？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Show databases</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Show tables</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Insert into </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">表名() values()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Update </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">表名 set 字段=值 where ...</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Delete from </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">表名 where ...</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select * from </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">表名 where 条件 order by ... Desc/asc limit ... Group by ... Having ...</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">进入mysql管理命令行的命令？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysql -uroot -p </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">回车 密码</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">show databases; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示当前mysql服务器中有哪些数据库</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">show create database mysql; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示创建数据库的sql语句</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">show create table user; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示创建表的sql语句</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">desc user; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">查询user表的结构</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">explain select * from user; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取select相关信息</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">show processlist; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示哪些线程正在运行</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">SHOW VARIABLES; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示系统变量和值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">SHOW VARIABLES like ’%conn%’; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">这个命令的作用？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">显示系统变量名包含conn的值</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">LEFT JOIN </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个SQL语句？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">SELECT A.id,A.class FROM A LEFT JOIN B ON A.cid=B.id</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出5个常用的unix操作命令。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Ls&nbsp;-l</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、tar&nbsp;-zxvf</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Touch</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Cat</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mkdir</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">6</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、rm</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出以下5个UNIX系统配置文件/服务的作用。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">/etc/passwd&nbsp;</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">/etc/hosts&nbsp;</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">/etc/fstab&nbsp;</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Crontab</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">sshd</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、/etc/passwd&nbsp;：用户信息文件，其中包含用户名、用户是否有密码、用户ID及用户所属组</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、/etc/hosts：主机名数据库，包IP地址、主机名或域名、别名等信息，在此文件中添加记录可绕过DNS</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、/etc/fstab&nbsp;&nbsp;保存了系统所有分区信息的配置文件。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Crontab&nbsp;计划任务命令</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Sshd&nbsp;远程连接管理命令</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出5个常用的SQL操作关键字。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select&nbsp;,update,&nbsp;delete,&nbsp;insert&nbsp;into,&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">create&nbsp;,group&nbsp;by&nbsp;,order&nbsp;by</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请列出5个常用的PHP操作MySQL的函数</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mysql_connect()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mysql_select_db()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mysql_query()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mysql_fetch_row()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Mysql_close()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请列出4个常用的HTML标签名&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;table&gt;&lt;/table&gt;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;a&gt;&lt;/a&gt;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;form&gt;&lt;/form&gt;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;div&gt;&lt;/div&gt;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">怎么找到数据库的配置文件路径？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在数据库安装目录下，my.ini</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">什么是时间戳? 如何取得当前时间戳?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">时间戳是从1970年1月1日 00:00:00到指定日期的秒数。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取当前时间戳：time()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">有一个网页地址, 比如PHP开发资源网主页: <a href="http://www.phpres.com/index.html,%CE%B5??"><span style="color:windowtext">http://www.phpres.com/index.html,</span><span style="color:windowtext">如何得到它的内容?</span></a></span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">获取网页内容：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$url=”<a href="http://www.phpres.com/index.html"><span style="color:#333333;text-underline:none">http://www.phpres.com/index.html</span></a>“;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$str=file_get_contents($url);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述如何得到当前执行脚本路径，包括所得到参数</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_SERVER[&#39;DOCUMENT_ROOT&#39;].$_SERVER[&#39;REQUEST_URI&#39;];</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">取得当前页面的完整路径和参数。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">取得参数：$_SERVER[&#39;QUERY_STRING&#39;];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何用php的环境变量得到一个网页地址的内容？ip地址又要怎样得到？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $_SERVER [&quot;PHP_SELF&quot;];<br/> echo $_SERVER [&quot;SERVER_ADDR&quot;];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">求两个日期的差数，例如2007-2-5 ~ 2007-3-6 的日期差数</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$begin=strtotime(“2007-2-5″);<br/> $end=strtotime(“2007-3-6″);<br/> echo ($end-$begin)/(24*3600);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">给一个变量赋值为0123，但是输出该变量的值总是为其他数字，请问这是什么问题？</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> PHP </span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解释器会把以0开始的数字当做是八进制的，所以它的值会变成八进制的。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">里面如何定义一个常量(constant)?<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">通过define()指令，例如：define(”MYCONSTANT”, 100)<br/> </span><strong><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何对一个变量进行值传递？<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">可以像C++那样， 在变量的前面加上&amp;, 例如：$a = &amp;$b</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在PHP里面可以对string “10″ 和整型 11进行比较吗？</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">可以，PHP内部实现会把所有东西转换成整型，所以数字10和11可以进行比较</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在什么情况下需要用endif 来结束条件语句？</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">当if语句后面跟的是冒号”:”而不是大括号{时，需要用endif来结束条件语句</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">优化MYSQL数据库的方法。(4分，多写多得)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、选取最适用的字段属性,尽可能减少定义字段长度,尽量把字段设置NOT NULL,例如’省份,性别’,最好设置为ENUM<br/> 2、使用连接（JOIN）来代替子查询:<br/> 3、使用联合(UNION)来代替手动创建的临时表<br/> 4、事务处理:<br/> 5、锁定表,优化事务处理:<br/> 6、使用外键,优化锁定表<br/> 7、建立索引:<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; a.格式:<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="text-decoration:underline;">(</span><span style="text-decoration:underline;">普通索引)-&gt;</span><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 创建:CREATE INDEX &lt;索引名&gt; ON tablename (索引字段)<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 修改:ALTER TABLE tablename ADD INDEX [索引名] (索引字段)<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 创表指定索引:CREATE TABLE tablename([...],INDEX[索引名](索引字段))<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="text-decoration:underline;">(</span><span style="text-decoration:underline;">唯一索引)-&gt;</span><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 创建:CREATE UNIQUE &lt;索引名&gt; ON tablename (索引字段)<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 修改:ALTER TABLE tablename ADD UNIQUE [索引名] (索引字段)<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 创表指定索引:CREATE TABLE tablename([...],UNIQUE[索引名](索引字段))<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="text-decoration:underline;">(</span><span style="text-decoration:underline;">主键)-&gt;</span><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 它是唯一索引,一般在创建表是建立,格式为:<br/> CREATA TABLE tablename ([...],PRIMARY KEY[索引字段])<br/> 8、优化查询语句</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">MYSQL</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">取得当前时间的函数是?，格式化日期的函数是(2分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; now(),date()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">实现中文字串截取无乱码的方法。(3分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function GBsubstr($string, $start, $length) {<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(strlen($string)&gt;$length){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $str=null;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $len=$start+$length;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($i=$start;$i&lt;$len;$i++){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(ord(substr($string,$i,1))&gt;0xa0){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $str.=substr($string,$i,2);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $i++;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $str.=substr($string,$i,1);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $str.’…’;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $string;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">分别指出php.ini中 magic_quotes_gpc, magic_quotes_runtime两项参数的作用.</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Magic_quotes_gpc</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的作用是在POST、GET、COOKIE数据上使用addslashes()自动转义。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Magic_quotes_runtime</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">参数的作用是设置状态，当状态为0时则关闭自动转义，设置为1则自动转义，将数据库中取出来的单引号、双引号、反斜线这些字符加上反斜杠转义。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用面向对象来实现A对象继承B和C对象</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Interface B{ ... }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Interface C{ ... }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Class A implements B,C{ ... }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出Smarty模板引擎中你最常用的关键词</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Assign&nbsp;&nbsp;&nbsp;&nbsp; Display&nbsp;&nbsp;&nbsp; Foreach</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Section&nbsp;&nbsp; Loop&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Item</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$smarty&nbsp; Now&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Const&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; get</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何快速下载一个远程http服务器上的图片文件到本地?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$file=</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”&quot;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$fp=fopen($file,</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">’rb’);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$img=fread($fp,10000);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$dir=</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”./”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$local=fopen($dir.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">’/’.basename($file),’w&#39;);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Fwrite($local,$img);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">一个字节占多少bit ? 一个IPv4地址占几个字节? 一个IPv6地址呢?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">一个字节占8bit，一个IPV4占用4字节，一个IPV6占用16字节。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">M ADSL</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">宽带连接, 理想情况下, 最大下载速度是多少KB/s&nbsp; ?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">256KB/s</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Fatal error: Call to undefined method ge_user() in /website/index.php on line 39</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">调用了未定义的方法ge_user()，检查程序中有没有定义此方法</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Fatal error: Class ’client’ not found in /website/index.php on line 173</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">类client没有找到，检查文件中有没有client类，或者有没有包含client类文件</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Warning: Cannot modify header information - headers already sent by (output started at /website/index.php:1) in /website/index.php&nbsp; on line 3</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">提示文件前面有输出，检查是否有输出，或者编码</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Warning:session_start(): open(/website/tmp/sess_47e067121facf033785f9a1cb16d243b,&nbsp;&nbsp; O_RDWR) failed: No such file or directory (2) in /website/index.php on line&nbsp; 10</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">没有找到文件或目录，检查文件是否存在</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#969696">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Parse error: syntax error, unexpected T_STRING in /website/index.php on line 18</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">18</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">行语法错误，检查语法</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Warning:fopen(welcome.txt) [function.fopen]: failed to open stream: No such file or directory in /website/index.php on line 2</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">没有找到welcome.txt文件，检查文件是否存在</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">抓取远程图片到本地,你会用什么函数?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">fsockopen, A</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用PHP打印出前一天的时间，打印格式是2007年5月10日22:21:21</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo date(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘Y-m-d H:i:s’,strtotime(‘-1 day’));</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">//</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">正在浏览当前页面用户的 IP 地址:127.0.0.1<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $_SERVER[&quot;REMOTE_ADDR&quot;].</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”&lt;br /&gt;”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">//</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">查询（query）的字符串（URL 中第一个问号 ? 之后的内容）:id=1&amp;bi=2</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> echo $_SERVER[&quot;QUERY_STRING&quot;].</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”&lt;br /&gt;”;<br/> //当前运行脚本所在的文档根目录:d:inetpubwwwroot<br/> echo $_SERVER[&quot;DOCUMENT_ROOT&quot;].”&lt;br /&gt;”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在PHP中，heredoc是一种特殊的字符串，它的结束标志必须?(1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> <a></a><a></a><a>heredoc</a></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的语法是用”&lt;&lt;&lt;&quot;加上自己定义成对的标签，在标签范围內的文字视为一个字符串<br/> 例子:<br/> $str = &lt;&lt; my name is Jiang Qihui!<br/> SHOW;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何声明一个名为”myclass”的没有方法和属性的类? (1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; class myclass{ }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何实例化一个名为”myclass”的对象?</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; new myclass()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你如何访问和设置一个类的属性? (2分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$object = new myclass();<br/> $newstr = $object-&gt;test;<br/> $object-&gt;test = &quot;info&quot;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">指出一些在PHP输入一段HTML代码的办法。(1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> echo &quot;<a href="http://www.mianwww.com/html/2011/05/index.php"><span style="color:#333333;text-underline:none">aaa</span></a>&quot;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面哪个函数可以打开一个文件，以对文件进行读和写操作?[ c ]<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(a) fget() (b) file_open() <span style="text-decoration:underline;">(c) fopen() </span>(d) open_file()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述Linux下安装PHP的过程？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">安装软件之前先安装编译工具gcc、gcc-c++</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">拷贝源码包，解包解压缩</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Cd /lamp/php</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">进入php目录</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">./configure –prefix=/usr/local/php –with-config-file-path=/usr/local/php/etc</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">指定安装目录和配置文件目录</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">编译</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make install</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">安装</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述Linux下安装Mysql的过程？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Groupadd mysql </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">添加一个用户组mysql</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Useradd -g mysql mysql </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">添加一个mysql用户指定分组为mysql</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Cd /lamp/mysql </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">进入mysql目录</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">./configure –prefix=/usr/local/mysql/ –with-extra-charsets=all</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make all</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述Linux下安装apache的过程？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Cd /lamp/httpd </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">进去apache软件目录</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">./configure –prefix=/usr/local/apache2/ –sysconfdir=/etc/httpd/ –with-included-apr</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Make all</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Linux </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下建立压缩包，解压缩包的命令</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Gz:</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打包: tar czf file.tar.gz file.txt</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解压: tar xzf file.tar.gz</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Bz2:</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打包: tar zxvf file.tar.bz2 file.txt</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解压: tar zcvf file.tar.bz2</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Gzip:</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打包: gzip file1.txt</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解压: gunzip file1.txt.gz</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Zip:</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打包: zip file1.zip file1.txt</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解压: unzip file1.zip</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出匹配URL的正则表达式. </span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">/^[a-zA-z]+:\/\/(\w+(-\w+)*)(\.(\w+(-\w+)*))*(\?\S*)?/ </span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请用正则表达式（Regular Expression）写一个函数验证电子邮件的格式是否正确。</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(isset($_POST[&#39;action&#39;]) &amp;&amp; $_POST[&#39;action&#39;]==</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">’submitted’){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $email=$_POST[&#39;email&#39;];<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(!preg_match(“/^(?:w+.?)*w+@(?:w+.?)*w+$/”,$email)){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo “电子邮件检测失败”;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo “电子邮件检测成功”;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写一个函数验证电子邮件的格式是否正确</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function checkemail($email){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo preg_match(‘/^[\w]+@[\w]+[\.]([\w]+)$/’,$email)?’email</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">格式正确‘:’email格式不正确‘;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出一个正则表达式,用于匹配一个HTML文件中&lt;img /&gt;标记中的图片地址</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$url=</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”&lt;img src=’11.jpg’/&gt;”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">/&lt;img[\s]*src=[&#39;|\&quot;](.*)[&#39;|\&quot;][\s]*\/&gt;/</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出一个正则表达式，过虑网页上的所有JS/VBS脚本(即把scrīpt标记及其内容都去掉):</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:gray">preg_replace(&quot;//si&quot;, &quot;newinfo&quot;, $script);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在PHP中error_reporting这个函数有什么作用？<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">设置 PHP 的报错级别并返回当前级别。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:gray">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">windows</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">平台, Apache Http Server启动失败, 排错思路是什么?</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">检查apache使用的80端口是否被占用，如果被占用，先停止占用80端口的服务，然后启动apache服务器</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">php</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">读取文件内容的几种方法和函数？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打开文件，然后读取。Fopen() fread()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">打开读取一次完成 file_get_contents()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">以下程序，变量str什么值的情况下输入111? </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">if( ! $str ) { echo 111; }</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在$str值为：0，’0′，false,null,”&quot;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出常见的排序算法，并用PHP实现冒泡排序，将数组$a = array()按照从小到大的方式进行排序。 </span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">常见的排序算法: 冒泡排序法、快速排序法、简单选择排序法、堆排序法、直接插入排序法、希尔排序法、合并排序法。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">冒泡排序法的基本思想是：对待排序记录关键字从后往前（逆序）进行多遍扫描，当发现相邻两个关键字的次序与排序要求的规则不符时，就将这两个记录进行交换。这样，关键字较小的记录将逐渐从后面向前面移动，就象气泡在水中向上浮一样，所以该算法也称为气泡排序法。</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">// </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">冒泡排序法</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Function mysort($arr){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For($i=0; $i&lt;count($arr); $i++){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For($j=0; $j&lt;count($arr)-1; $j++){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; If($arr[$j] &gt; $arr[$j+1]){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $tmp=$arr[$j];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr[$j]=$arr[$j+1];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr[$j+1]=$tmp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Return $arr;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$arr=array(3,2,1);</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">print_r(mysort($arr));</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用PHP描述快速排序算法，对象可以是一个数组?</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">原理:快速排序使用分治策略来把待排序数据序列分为两个子序列，具体步骤为：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（1）从数列中挑出一个元素，称该元素为“基准”。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（2）扫描一遍数列，将所有比“基准”小的元素排在基准前面，所有比“基准”大的元素排在基准后面。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">（3）通过递归，将各子序列划分为更小的序列，直到把小于基准值元素的子数列和大于基准值元素的子数列排序。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">快速排序（数组排序）</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function QuickSort($arr){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $num = count($arr);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $l=$r=0;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($i=1;$i&lt;$num;$i++){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($arr[$i] &lt; $arr[0]){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $left[] = $arr[$i];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $l++;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $right[] = $arr[$i];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $r++;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($l &gt; 1){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $left = QuickSort($left);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $new_arr = $left;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $new_arr[] = $arr[0];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($r &gt; 1){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $right = QuickSort($right);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($i=0;$i&lt;$r;$i++){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $new_arr[] = $right[$i];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $new_arr;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用PHP描述顺序查找和二分查找（也叫做折半查找）算法，顺序查找必须考虑效率，对象可以是一个有序数组</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">二分查找（数组里查找某个元素）</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function bin_sch($array, $low, $high, $k){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ($low &lt;= $high){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $mid = intval(($low+$high)/2);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ($array[$mid] == $k){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $mid;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }elseif ($k &lt; $array[$mid]){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return bin_sch($array, $low, $mid-1, $k);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return bin_sch($array, $mid+1, $high, $k);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return -1;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">顺序查找（数组里查找某个元素）</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function seq_sch($array, $n, $k){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $array[$n] = $k;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($i=0; $i&lt;$n; $i++){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($array[$i]==$k){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; break;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ($i&lt;$n){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $i;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return -1;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个二维数组排序算法函数，能够具有通用性，可以调用php内置函数</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">二维数组排序， $arr是数据，$keys是排序的健值，$order是排序规则，1是升序，0是降序</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function array_sort($arr, $keys, $order=0) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if (!is_array($arr)) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return false;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $keysvalue = array();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; foreach($arr as $key =&gt; $val) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $keysvalue[$key] = $val[$keys];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($order == 0){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; asort($keysvalue);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; arsort($keysvalue);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; reset($keysvalue);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; foreach($keysvalue as $key =&gt; $vals) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $keysort[$key] = $key;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $new_array = array();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; foreach($keysort as $key =&gt; $val) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $new_array[$key] = $arr[$val];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $new_array;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请以空格作为间隔，拆分字符串’Apple Orange Banana Strawberry’,组成数组$fruit， </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">* </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数组中所有元素都用小写字母，并按照字母先后次序排序 </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">class sort { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private $str; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function __construct($str) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;str=strtolower($str); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private function explodes() { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(empty($this-&gt;str)) return array(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr=explode(&quot; &quot;,$this-&gt;str); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return is_array($arr)?$arr:array($arr); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function sort() { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $explode=$this-&gt;explodes(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sort($explode); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $explode; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$str=&#39;Apple Orange Banana Strawberry&#39;; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sortob=new sort($str); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">var_dump($sortob-&gt;sort());</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">对于用户输入一串字符串$string,要求$string中只能包含大于0的数字和英文逗号，请用正则 表达式验证，对于不符合要求的$string返回出错信息 </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">class regx { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public static function check($str) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(preg_match(&quot;/^([1-9,])+$/&quot;,$str)) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return true; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return false; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$str=&quot;12345,6&quot;; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(regx::check($str)) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo &quot;suc&quot;; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} else { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo &quot;fail&quot;; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写一段程序，在服务器创建一个文件fruit.dat,将试题3中得到的数组写入到改文件中，然后写一段程序从文件中读取并还原数组@author zhuwenqiong </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">class sort { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private $str; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function __construct($str) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;str=strtolower($str); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private function explodes(){ </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(empty($this-&gt;str)) return array(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr=explode(&quot; &quot;,$this-&gt;str); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return is_array($arr)?$arr:array($arr); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function sort() { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $explode=$this-&gt;explodes(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; sort($explode); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $explode; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">class file { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private $sort=null; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private $filepath; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function __construct($arrobj,$path) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;sort=$arrobj; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;filepath=$path; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private function getresource($filename,$mode) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return fopen($this-&gt;filepath.$filename,$mode); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private function closeresource($resource) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; fclose($resource); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function savefile($filename) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr=$this-&gt;sort-&gt;sort(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $fopen=$this-&gt;getresource($filename,&quot;a+&quot;); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(!$fopen){ </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo &quot;</span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">文件打开失败！&quot;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; exit; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; var_dump($arr); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; foreach($arr as $key=&gt;$value) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; fwrite($fopen,$value.&quot;\n&quot;); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;closeresource($fopen); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public function readfile($filename) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;savefile($filename); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $fopen=$this-&gt;getresource($filename,&quot;r&quot;); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(!$fopen){ </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo &quot;</span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">文件打开失败！&quot;;exit; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr=array(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; while(!feof($fopen)) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $get=fgets($fopen); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if(!empty($get)) </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr[]=str_replace(&quot;\n&quot;,&quot;&quot;,$get); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;closeresource($fopen); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $arr; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$file=new file(new sort(&#39;Apple Orange Banana Strawberry&#39;),&quot;E:\\&quot;); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$arr=$file-&gt;readfile(&quot;fruit.dat&quot;); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">var_dump($arr); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">单例模式，创建mysqli数据库链接的单例对象 </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">class Db { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private static $instance; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public $handle; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Private function __construct($host,$username,$password,$dbname) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;handle=NULL; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;getcon($host,$username,$password,$dbname); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; public static function getBb() { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; self::$instance=new Db(); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return self::$instance; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; private function getcon($host,$username,$password,$dbname) { </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($this-&gt;handle!=NULL){ </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return true; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $this-&gt;handle=mysqli_connect($host,$username,$password,$dbname); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;"><br/> <strong><span style="text-decoration:underline;">PHP session</span></strong></span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">扩展默认将session数据储存在哪里? D</span></span></strong>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">A) </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;SQLite Database&nbsp;&nbsp;&nbsp;&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">B)&nbsp; MySQL Database&nbsp;&nbsp;&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">C)&nbsp; Shared Memory</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">D)&nbsp; File System</span></span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">E) &nbsp;Session Server</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如果你想要自动加载类，下面哪种函数声明是正确的 C</span></span></strong>
</p>
<p style="margin-left:0;text-align:left;text-indent:0;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">A) </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;function autoload($class_name)&nbsp;&nbsp;&nbsp;&nbsp; </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">B)&nbsp; function __autoload($class_name, $file)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">C)&nbsp; function __autoload($class_name)</span></span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">D)&nbsp; function _autoload($class_name)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">E)&nbsp; function autoload($class_name, $file)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">程序使用utf-8编码, 以下程序输出结果是什么? B</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;"><br/> &lt;?php<br/> $str = ’hello</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">你好世界’;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo strlen($str);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">?&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">A) 9 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="text-decoration:underline;">B) 13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; C) 18&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D) 17</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">设计一个页面(4个 div 第一个div 宽960px 居中;第2-4个div&nbsp; 3等分960px;)</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;style&gt;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Body{ Text-align:center; Margin:0; Padding:0; }</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">#box{ Width:960px; Margin:0 auto; }</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">.small{ Width:320px; Float:left; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;/style&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;div id=’box’&gt;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;div class=’small’&gt;&lt;/div&gt;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;div class=’small’&gt;&lt;/div&gt;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;div class=’small’&gt;&lt;/div&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;/div&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">简述如何得到当前执行脚本路径，包括所得到参数。(2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> $script_name = basename(__file__); print_r($script_name);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">js</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">中网页前进和后退的代码 </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">前进: history.forward();=history.go(1);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">后退: history.back();=history.go(-1); </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">JS</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">表单弹出对话框函数是?获得输入焦点函数是? (2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">弹出对话框: alert(),prompt(),confirm()<br/> 获得输入焦点 focus()</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">JS</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">的转向函数是?怎么引入一个外部JS文件?(2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; window.location.href, </span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;script type=&quot;text/javascript&quot; src=&quot;hello.js&quot;&gt;&lt;/script&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用javascript取得一个input的值？取得一个input的属性？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">document.getElementById(‘name’).value;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">document.getElementById(‘name’).type;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用Jquery取得一个input的值？取得一个input的属性？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$(“input[name=&#39;aa&#39;]“).val();</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$(“input[name=&#39;aa&#39;]“).attr(‘name’);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个简单的jquery显示隐藏代码？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$(&quot;#aa&quot;).hide();</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$(&quot;#aa&quot;).show();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">javascript</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">能否定义二维数组，如果不能你如何解决？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">javascript</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不支持二维数组定义，可以用arr[0] = new array()来解决</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下列不属于Javascript语法关键/保留字的是&nbsp;B</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">A.&nbsp;var</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">B.&nbsp;$</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">C.&nbsp;function</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">D.&nbsp;while</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请使用JavaScript写出三种产生一个Image 标签的方法（提示：从方法、对象、HTML角度考虑）</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(1)var img = new Image();<br/> (2)var img = document.createElementById(“image”)<br/> (3)img.innerHTML = “&lt;img src=”xxx.jpg” /&gt;”</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">假设a.html和b.html在同一个文件夹下面，用javascript实现当打开a.html五秒钟后，自动跳转到b.html。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;script&gt;<br/> function go2b(){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; window.location = </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">“b.html”;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; window.close();<br/> }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">setTimeout( </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">“go2b()”,5000 ); //5秒钟后自动执行go2b()<br/> &lt;/script&gt;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请您写一段ajax提交的js代码，或者写出ajax提交的过程逻辑。</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">var xmlhttp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(window.XMLHttpRquest){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">xmlhttp=new XMLHttpRequest();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}else if(window.ActiveXObject){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">xmlhttp=new ActiveXObject(‘Microsoft.XMLHTTP’);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">xmlhttp.open(‘GET’,’1.php?aa=name’,true);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">xmlhttp.onreadystatechange=function(){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(xmlhttp.readyState==4){</span>
</p>
<p style="margin-left:28px;text-align:left;text-indent:28px;line-height:15px;text-autospace: ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(xmlhttp.status==200){</span>
</p>
<p style="margin-left:56px;text-align:left;text-indent:28px;line-height:15px;text-autospace: ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">var text=xmlhttp.responseText;</span>
</p>
<p style="margin-left:28px;text-align:left;text-indent:28px;line-height:15px;text-autospace: ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">xmlhttp.send(null);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如下user表结构</span>
</p>
<table>
    <tbody>
        <tr class="firstRow">
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">名称</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">类型</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">说明</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">备注</span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Uid</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Int unsigned</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">主键</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;"></td>
        </tr>
        <tr>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Name</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Varchar(20)</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;"></td>
            <td width="142" valign="top" style="padding: 0px 7px;"></td>
        </tr>
        <tr>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Age</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;">
                <p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align:   top">
                    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Tinyint unsigned</span>
                </p>
            </td>
            <td width="142" valign="top" style="padding: 0px 7px;"></td>
            <td width="142" valign="top" style="padding: 0px 7px;"></td>
        </tr>
    </tbody>
</table>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">需求：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">l </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">增加一个字段性别sex，写出修改语句</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Alert table user add sex enum(’0′,’1′);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">查询出年龄介于20岁到30岁之间的用户</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select * from user where age&gt;20 and age&lt;30</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个函数，算出两个文件的相对路径</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如 $a = ’/a/b/c/d/e.php’;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$b = ’/a/b/12/34/c.php’; </span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">计算出 $b 相对于 $a 的相对路径应该是 <a href="http://www.cnblogs.com/c/d()"><span style="color:windowtext">http://www.cnblogs.com/c/d</span><span style="color:windowtext">将()</span><span style="color:windowtext">添上</span></a></span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$a=”<a href="http://www.cnblogs.com/"><span style="color:windowtext">http://www.cnblogs.com/</span></a>a/b/c/d/e.php”;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$b=”<a href="http://www.cnblogs.com/"><span style="color:windowtext">http://www.cnblogs.com/</span></a>a/b/12/34/c.php”;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$ainfo=parse_url($a);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$binfo=parse_url($b);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$apath=ltrim($ainfo[&#39;path&#39;],&#39;/&#39;);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$bpath=ltrim($binfo[&#39;path&#39;],&#39;/&#39;);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$arr=explode(&#39;/&#39;,$apath);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$brr=explode(&#39;/&#39;,$bpath);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$count=count($arr);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">for($i=0;$i&lt;$count;$i++){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if($arr[$i]==$brr[$i]){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$brr[$i]=&#39;..&#39;;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}else{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">break;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$cha=implode(&#39;/&#39;,$brr);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">print_r($cha);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个函数，能够遍历一个文件夹下的所有文件和子文件夹。</span></span></strong>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function my_scandir($dir){</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp; $files = array();</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp; if ( $handle = opendir($dir) ){</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; while ( ($file = readdir($handle)) !== false ) {</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ( $file != &quot;..&quot; &amp;&amp; $file != &quot;.&quot; ) {</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp; <a></a><a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if ( is_dir($dir . &quot;/&quot; . $file) ) {</a></span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $files[$file] = scandir($dir . &quot;/&quot; . $file);</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }else {</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $files[] = $file;</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; closedir($handle);</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $files;</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other;vertical-align: baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <a><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">Linux</span></span></strong></a><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">的目录进行遍历，编写shell脚本</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">#!/bin/bash</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Tree</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">指出以下代码片段中的SQL注入漏洞以及解决方法(magic_quotes_gpc = off)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">mysql_query(“select id,title from content where catid=’{$_GET[catid]}’ and title like ’%$_GET[keywords]%’”, $link);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">注入漏洞主要存在用户提交的数据上，这里的注入漏洞主要是$_GET[catid]和$_GET[keyword]</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">解决注入漏洞：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$_GET[catid]=intval($_GET[catid]);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sql=”select id,title from content where catid=’{$_GET[catid]}’ and title like ’%$_GET[keywords]%”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sql=addslashes($sql);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysql_query($sql);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出以下php代码的运行结果:<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;?php<br/> function foo($i) {<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $i++;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $i ;<br/> }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function bar(&amp;$i) {</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}<br/> $i = 10 ;<br/> echo $i++ , ++$i;&nbsp;&nbsp;&nbsp; </span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出：10,12<br/> </span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">foo($i); </span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出：13</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> bar($i);&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">输出：无输出</span></span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在HTTP 1.0中，状态码 401 的含义是未授权____；如果返回“找不到文件”的提示，则可用 header 函数，其语句为header(“HTTP/1.0 404 Not Found”);<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <a></a><a>401</a></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">表示未授权;header(“HTTP/1.0 404 Not Found”);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">把 John 新增到 users 阵列？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$users[] = </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘john’;&nbsp;&nbsp; array_push($users,‘john’);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:red">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在PHP中error_reporting这个函数有什么作用？</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> error_reporting() </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">设置 PHP 的报错级别并返回当前级别。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何修改SESSION的生存时间(1分).</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <a></a><a><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法1:将php.ini中的session.gc_maxlifetime设置为9999重启apache</span></a>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法2:$savePath = “./session_save_dir/”;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$lifeTime = </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">小时 * 秒;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">session_save_path($savePath);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">session_set_cookie_params($lifeTime);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">session_start();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法3:</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">setcookie() and session_set_cookie_params($lifeTime);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">有一个网页地址, 比如PHP开发资源网主页: http://www.phpres.com/index.html,如何得到它的内容?($1分)</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法1(对于PHP5及更高版本):</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$readcontents = fopen(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">“http://www.phpres.com/index.html”, “rb”);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$contents = stream_get_contents($readcontents);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">fclose($readcontents);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $contents;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法2:</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo file_get_contents(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">“http://www.phpres.com/index.html”);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个函数，尽可能高效的，从一个标准 url 里取出文件的扩展名</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">例如: http://www.sina.com.cn/abc/de/fg.php?id=1 需要取出 php 或 .php</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答案1:</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function getExt($url){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$arr = parse_url($url);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$file = basename($arr[&#39;path&#39;]);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$ext = explode(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">“.”,$file);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return $ext[1];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答案2:</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function getExt($url) {</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$url = basename($url);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pos1 = strpos($url,</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”.”);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pos2 = strpos($url,</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”?”);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(strstr($url,</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">”?”)){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Return substr($url,$pos1 + 1,$pos2 </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">– $pos1 – 1);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">} else {</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return substr($url,$pos1);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用五种以上方式获取一个文件的扩展名</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">要求：dir/upload.image.jpg，找出 .jpg 或者 jpg ，<br/> 必须使用PHP自带的处理函数进行处理，方法不能明显重复，可以封装成函数</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"> get_ext1($file_name), get_ext2($file_name)</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function get_ext1($file_name){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return strrchr($file_name, </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘.’);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function get_ext2($file_name){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return substr($file_name,strrpos($file_name, </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘.’));</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function get_ext3($file_name){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return array_pop(explode(</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘.’, $file_name));</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function get_ext4($file_name){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$p = pathinfo($file_name);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return $p[&#39;extension&#39;];</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function get_ext5($file_name){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return strrev(substr(strrev($file_name), 0, strpos(strrev($file_name), </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">‘.’)));</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&lt;?php<br/> $str1 = null;<br/> $str2 = false;<br/> echo $str1==$str2 ? ‘</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">相等’ : ‘不相等’;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$str3 = ”;<br/> $str4 = 0;<br/> echo $str3==$str4 ? ‘</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">相等’ : ‘不相等’;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$str5 = 0;<br/> $str6 = ’0′;<br/> echo $str5===$str6 ? ‘</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">相等’ : ‘不相等’;<br/> ?&gt;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">相等 相等 不相等</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">求两个日期的差数，例如2007-2-5 ~ 2007-3-6 的日期差数</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法一：<br/> &lt;?php<br/> class Dtime{<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; function get_days($date1, $date2){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $time1 = strtotime($date1);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $time2 = strtotime($date2);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return ($time2-$time1)/86400;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> }<br/> $Dtime = new Dtime;<br/> echo $Dtime-&gt;get_days(’2007-2-5′, ’2007-3-6′);<br/> ?&gt;<br/> 方法二：<br/> &lt;?php<br/> $temp = explode(‘-’, ’2007-2-5′);<br/> $time1 = mktime(0, 0, 0, $temp[1], $temp[2], $temp[0]);<br/> $temp = explode(‘-’, ’2007-3-6′);<br/> $time2 = mktime(0, 0, 0, $temp[1], $temp[2], $temp[0]);<br/> echo ($time2-$time1)/86400;<br/> 方法三：echo abs(strtotime(“2007-2-1″)-strtotime(“2007-3-1″))/60/60/24 计算时间差</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写一个函数，实现以下功能：<br/> 字符串“open_door” 转换成 “OpenDoor”、”make_by_id” 转换成 ”MakeById”。<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法：<br/> function str_explode($str){<br/> $str_arr=explode(“_”,$str);$str_implode=implode(” “,$str_arr); $str_implode=implode<br/> (“”,explode(” “,ucwords($str_implode)));<br/> return $str_implode;<br/> }<br/> $strexplode=str_explode(“make_by_id”);print_r($strexplode);<br/> 方法二：$str=”make_by_id!”;<br/> $expStr=explode(“_”,$str);<br/> for($i=0;$i&lt;count($expStr);$i++){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo ucwords($expStr[$i]);<br/> }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法三：echo str_replace(‘ ‘,”,ucwords(str_replace(‘_’,’ ‘,’open_door’)));</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">一个表中的Id有多个记录，把所有这个id的记录查出来，并显示共有多少条记录数，用SQL语句及视图、存储过程分别实现。</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> DELIMITER //<br/> create procedure proc_countNum(in columnId int,out rowsNo int)<br/> begin<br/> select count(*) into rowsNo from member where member_id=columnId;<br/> end<br/> call proc_countNum(1,@no);<br/> select @no;<br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">方法：视图：<br/> create view v_countNum as select member_id,count(*) as countNum from member group by<br/> member_id<br/> select countNum from v_countNum where member_id=1</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo count(“abc”); </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">输出什么？</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答案:1</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">count — </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">计算数组中的单元数目或对象中的属性个数</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">int count ( <a href="http://blog.sina.com.cn/s/language.pseudo-types.html#language.types.mixed"><span style="color:#333333;text-underline:none">mixed</span></a>$var [, int $mode ] ), </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">如果 var 不是数组类型或者实现了 Countable 接口的对象，将返回1，有一个例外，如果 var 是 NULL 则结果是 0。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">对于对象，如果安装了 <a href="http://blog.sina.com.cn/s/ref.spl.html"><span style="color:#333333;text-underline:none">SPL</span></a>，可以通过实现 Countable 接口来调用 count()。该接口只有一个方法 count()，此方法返回 count() 函数的返回值。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">有一个一维数组，里面存储整形数据，请写一个函数，将他们按从大到小的顺序排列。要求执行效率高。并说明如何改善执行效率。（该函数必须自己实现，不能使用php函数）</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;?php<br/> function BubbleSort(&amp;$arr){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $cnt=count($arr);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $flag=1;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($i=0;$i&lt;$cnt;$i++){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($flag==0){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $flag=0;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for($j=0;$j&lt;$cnt-$i-1;$j++){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if($arr[$j]&gt;$arr[$j+1]){<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $tmp=$arr[$j];<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr[$j]=$arr[$j+1];<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arr[$j+1]=$tmp;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $flag=1;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }<br/> }<br/> $test=array(1,3,6,8,2,7);<br/> BubbleSort($test);<br/> var_dump($test);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">31</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">、.以下的代码会产生什么？为什么？<br/> $num =10;<br/> function multiply(){<br/> $num =$num *10;</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">}<br/> multiply();<br/> echo $num;</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">由于函式 multiply() 没有指定 $num 为全域变量（例如 global $num 或者 $_GLOBALS[&#39;num&#39;]），所以 $num 的值是 10。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面的类是否正确，如果正确请补全方法输入类属性$_a;错误请修改并输出属性$_a</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;?php</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Class A{</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; protected$a=1;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; publicfunction test(){</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; echo$this-&gt;a;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=new A;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a-&gt;test();</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请取出数组中的最大值？</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$a=array(1,9,3,5,6,8);</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$a=array(1,2,3,4,5,9);</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b=max($a);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo $b;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">or</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=array(1,9,3,5,6,8);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">rsort($a);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo array_shift($a);</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请问同时满足这样条件的数：被10除于9，被9除于8，被8除于7，在100—1000之间，有几个这样的数？（并写出算法）</span></span></strong>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">A</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不存在，B 1个 <span style="text-decoration:underline;">C2个</span>&nbsp;&nbsp; D 3个</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">分析过程：</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; P</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">除以10余9:P+1就被10整除</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; P</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">除以9余8:P+1就被9整除</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; P</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">除以8余7:P+1就被8整除</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">所以P=8，9，10的功倍数-1</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 8=2*2*2,9=3*3,10=2*5</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">则P+1一定是2*2*2*3*3*5的倍数（只能约掉一个2 ）</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">又100&lt;=P&lt;=1000</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; 101&lt;=P+1&lt;=1001</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">所以P+1=360,720</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">所以P=359,719</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出一个简单的静态数组？</span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Class A{</span>
</p>
<p style="margin-left:28px;text-align:left;text-indent:28px;line-height:15px;text-autospace: ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Static $a=array(&#39;11&#39;=&gt;&#39;1111&#39;);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Print_r(A::$a);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">从表login中选出name字段包含admin的前10条结果所有信息的sql语句</span></span></strong>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select *from login where name like &#39;%admin%&#39; limit 0,10;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出发贴数最多的十个人名字的SQL，利用下表：members(id,username,posts,pass,email)(2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; SELECT * FROM `members` ORDER BY posts DESC limit 0,10;</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">使用php写一段简单查询，查出所有姓名为“张三”的内容并打印出来 (2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span>　　<span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">表名User<br/> 　　Name Tel Content Date<br/> 　　张三 13333663366 大专毕业 2006-10-11<br/> 　　张三 13612312331 本科毕业 2006-10-15<br/> 　　张四 021-55665566 中专毕业 2006-10-15<br/> 　　请根据上面的题目完成代码：</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　$mysql_db=mysql_connect(&quot;local&quot;,&quot;root&quot;,&quot;pass&quot;);</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　　@mysql_select_db(&quot;DB&quot;,$mysql_db);</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; $result = mysql_query(&quot;SELECT * FROM `user` WHERE name=&#39;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">张三&#39;&quot;);</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp; while($rs = mysql_fetch_array($result)){</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $rs[&quot;tel&quot;].$rs[&quot;content&quot;].$rs[&quot;date&quot;];</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">PDO</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">写法:</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Try{</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$dsn = &quot;mysql:host=localhost;dbname=user&quot;;</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo = new PDO($dsn,&#39;root&#39;,&#39;123456&#39;);</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo-&gt;setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo-&gt;query(&#39;set names utf8&#39;);</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sql = &quot;SELECT * FROM user WHERE name=&#39;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">张三&#39;&quot;;</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$result = $pdo-&gt;query($sql);</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Foreach($result as $v){</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo $v[&#39;tel&#39;].$v[&#39;content&#39;].$v[&#39;date&#39;];</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}catch(PDOException $e){</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo $e-&gt;getCode().&#39;:&#39;.$e-&gt;getMessage();</span>
</p>
<p style="text-align:left;text-indent:24px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysqli</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">写法:</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$mysqli = new mysqli(&#39;localhost&#39;,&#39;root&#39;,&#39;123456&#39;,&#39;user&#39;);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">If(mysqli_connect_errno()){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Die(&#39;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">连接数据库失败,&#39;.mysqli_connect_error());</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$mysqli-&gt;set_charset(&#39;utf8&#39;);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$result = $mysqli-&gt;query(&quot;SELECT * FROM user WHERE name=&#39;</span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">张三&#39;&quot;);</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">If($result &amp;&amp; $result-&gt;affected_row()){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">While($row = $result-&gt;fetch_object()){</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo $row-&gt;tel.$row-&gt;content.$row-&gt;date;</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">如何使用下面的类,并解释下面什么意思?(3)<br/> </span></span></strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">　　class test{<br/> function Get_test($num){<br/> 　　 $num=md5(md5($num).&quot;En&quot;);<br/> 　　 return $num;<br/> 　　 }<br/> 　　}</span></span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:$testnum = &quot;123&quot;;<br/> $object = new test();<br/> $encrypt = $object-&gt;Get_test($testnum);<br/> echo $encrypt;<br/> 类test里面包含Get_test方法,实例化类调用方法多字符串加密</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出以下程序的输出结果 (1分)<br/> </span></span></strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　&nbsp;&nbsp;&nbsp; &lt;?php</span></span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b=201;<br/> </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">　　$c=40;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $a=$b&gt;$c?4:5;<br/> 　　echo $a;<br/> 　　?&gt;</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:4</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">检测一个变量是否有设置的函数是否?是否为空的函数是?(2分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; isset($str),empty($str);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">取得查询结果集总数的函数是?(1分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:mysql_num_rows($result);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$arr = array(&#39;james&#39;, &#39;tom&#39;, &#39;symfony&#39;); </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">请打印出第一个元素的值 (1分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:echo $array[0];</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请将41题的数组的值用&#39;,&#39;号分隔并合并成字串输出(1分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:for($i=0;$i</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$a = &#39;abcdef&#39;; </span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请取出$a的值并打印出第一个字母(1分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:echo $a{0} 或 echo substr($a,0,1)</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">PHP</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">可以和sql server/oracle等数据库连接吗?(1分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:当然可以</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出PHP5权限控制修饰符(3分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:public(公共),private(私用),protected(继承)</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出php5的构造函数和析构函数(2分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:__construct , __destruct</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">完成以下:<br/> (一)创建新闻发布系统，表名为message有如下字段 (3分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">　　id 文章id<br/> 　　title 文章标题<br/> 　　content 文章内容<br/> 　　category_id 文章分类id<br/> hits 点击量</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:CREATE TABLE &#39;message&#39;(<br/> &#39;id&#39; int(10) NOT NULL auto_increment,<br/> &#39;title&#39; varchar(200) default NULL,<br/> &#39;content&#39; text,<br/> &#39;category_id&#39; int(10) NOT NULL,<br/> &#39;hits&#39; int(20),<br/> PRIMARY KEY(&#39;id&#39;);<br/> )ENGINE=InnoDB DEFAULT CHARSET=utf8;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">(</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">二)同样上述新闻发布系统：表comment记录用户回复内容，字段如下 (4分)</span></span></strong>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span>　<span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">　comment_id 回复id<br/> 　　id 文章id，关联message表中的id<br/> 　　comment_content 回复内容<br/> 　　现通过查询数据库需要得到以下格式的文章标题列表,并按照回复数量排序，回复最高的排在最前面<br/> 　　文章id 文章标题 点击量 回复数量<br/> 　　用一个SQL语句完成上述查询，如果文章没有回复则回复数量显示为0</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:SELECT message.id id,message.title title,IF(message.`hits` IS NULL,0,message.`hits`) hits,<br/> IF(comment.`id` is NULL,0,count(*)) number FROM message LEFT JOIN<br/> comment ON message.id=comment.id GROUP BY message.`id`;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span>　　<strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">(</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">三)上述内容管理系统，表category保存分类信息，字段如下 (3分)</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span>　　<span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">category_id int(4) not null auto_increment;<br/> </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">　　categroy_name varchar(40) not null;<br/> 　　用户输入文章时，通过选择下拉菜单选定文章分类<br/> 　　写出如何实现这个下拉菜单</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">答:function categoryList(){<br/> $result=mysql_query(&quot;select category_id,categroy_name from category&quot;)<br/> or die(&quot;Invalid query: &quot; . mysql_error());<br/> print(&quot; ... &quot;);<br/> }</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个函数，算出两个文件的相对路径<br/> 　　如 $a = &#39;/a/b/c/d/e.php&#39;;<br/> 　　$b = &#39;/a/b/12/34/c.php&#39;;<br/> 　　计算出 $b 相对于 $a 的相对路径应该是 http://www.cnblogs.com/c/d将()添上</span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> function getRelativePath($a, $b) {</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $returnPath = array(dirname($b));</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arrA = explode(&#39;/&#39;, $a);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $arrB = explode(&#39;/&#39;, $returnPath[0]);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for ($n = 1, $len = count($arrB); $n &lt; $len; $n++){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ($arrA[$n] != $arrB[$n]) {</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; break;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if ($len - $n &gt; 0) {</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $returnPath = array_merge($returnPath, array_fill(1, $len - $n, &#39;..&#39;));</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $returnPath = array_merge($returnPath, array_slice($arrA, $n));</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return implode(&#39;/&#39;, $returnPath);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo getRelativePath($a, $b);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">填空题:<span style="color:#333333"><br/> </span>1.在PHP中，当前脚本的名称(不包括路径和查询字符串)记录在预定义变量__<span style="color:gray">$_SERVER[&#39;PHP_SELF&#39;]</span>__中;而链接到当前页面的URL记录在预定义变量__<span style="color:gray">$_SERVER[&#39;HTTP_REFERER&#39;]</span>__<br/> 中<br/> 2.执行程序段将输出__<span style="color:gray">0</span>__。</span>
</p>
<p style=";margin-bottom:0;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">4.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">数组函数 arsort 的作用是__<span style="color: gray">对数组进行逆向排序并保持索引关系</span>__;语句 error_reporting(2047)的作用是__<span style="color:gray">报告所有错误和警告</span>__。</span>
</p>
<p style=";margin-bottom:0;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">6.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">7.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">以Apache模块的方式安装PHP，在文件http.conf中首先要用语句____<span style="color:gray">动态装载PHP模块，然后再用语句</span>____使得Apache把所有扩展名为php的文件都作为PHP脚本处理。<br/> 10.一个函数的参数不能是对变量的引用，除非在php.ini中把__<span style="color:gray">allow_call_time_pass_reference boolean</span>__设为on.<br/> 11.SQL中LEFT JOIN的含义是__<span style="color:gray">自然左外链接</span>__。&nbsp;</span>
</p>
<p style=";margin-bottom:0;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">7.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px;vertical-align:baseline">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">编写一个在线留言本，实现用户的在线留言功能，留言信息存储到数据库？</span></span></strong>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">假设现在有数据库：test表：mess字段：id，name，message</span>
</p>
<p style="margin-left:0;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1、</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">html</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">页面，填写留言：</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;form&nbsp; method=&quot;post&quot; action=&quot;post.php&quot;&gt;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">留言者：&lt;input type=&quot;text&quot; name=&quot;name&quot; /&gt;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">留言内容：&lt;input type=&quot;text&quot; name=&quot;message&quot; /&gt;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;input type=&quot;submit&quot; value=&quot;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">提交&quot; /&gt;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&lt;/form&gt;</span>
</p>
<p style="margin-left:0;text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2、</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">post.php</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">页面，处理留言：</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$name = $_POST[&#39;name&#39;];</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$message = $_POST[&#39;message&#39;];</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Try{</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$dsn = &#39;&#39;mysql:host=localhost;dbname=test;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo = new PDO($dsn,&#39;root&#39;,&#39;112233&#39;);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo-&gt;setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$pdo-&gt;query(&#39;set names utf8&#39;);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sql = &quot;insert into test(name,message) values(&#39;$name&#39;,&#39;$message&#39;)&quot;;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$result = $pdo-&gt;exec($sql);</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">If($result){</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo ‘</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">留言成功’；</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}else{</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo &#39;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">留言失败&#39;;</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}catch(PDOException $e){</span>
</p>
<p style="text-indent:28px;line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo $e-&gt;getCode().&#39; : &#39;.$e-&gt;getMessage();</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style="line-height:15px;vertical-align:baseline">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">实现不使用第3个变量，交换$a、$b的值，$a、$b的初始值自己定。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=4;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $b=5;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=explode(‘,’,$a.’,’.$b);&nbsp;&nbsp;//</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">把用逗号把4,5分开。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b=$a[0];</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$a=$a[1];</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo&nbsp;$a,$b;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在数据库test中的一个表student，字段是name，class，score。分别代表姓名、所在班级，分数。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">1)&nbsp;</span></span><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">学出每个班级中的学生，按照成绩降序排序;</span></span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">select&nbsp;*&nbsp;from&nbsp;student&nbsp;order&nbsp;by&nbsp;score&nbsp;desc;</span>
</p>
<p style=";margin-bottom:0;text-indent:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">2)</span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">查出每个班的及格人数和不及格人数，格式为：class、及格人数、不及格人数；</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select&nbsp;A.class,A.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">及格人数,B.不及格人数&nbsp;from&nbsp;(select&nbsp;class,&nbsp;count(*)&nbsp;as&nbsp;’及格人数‘&nbsp;from&nbsp;student&nbsp;where&nbsp;score&gt;=60&nbsp;group&nbsp;by&nbsp;class)&nbsp;as&nbsp;A,(select&nbsp;&nbsp;class,count(*)&nbsp;as&nbsp;’不及格人数‘&nbsp;from&nbsp;student&nbsp;where&nbsp;score&lt;60&nbsp;group&nbsp;by&nbsp;class)&nbsp;as&nbsp;B&nbsp;where&nbsp;A.class=B.class;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">3)&nbsp;</span></span><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">用PHP写入连接数据库(“localhost”,”msuser”,”mspass”)、执行以上SQL、显示结果、判断错误、关闭数据库的过程；</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$conn=mysql_connect(‘localhost’,&#39;root’,’12345′);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysql_select_db(‘test’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$sql=”&quot;;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$result=Mysql_query($sql);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Mysql_close();</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">ftp://pub.foo.bar.com:2121/incoming/rls.sfv&nbsp;</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请给出这个URL各部分的意义&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、<a href target="_blank"><span style="color:#333333">ftp://&nbsp;</span></a>;使用的协议是：ftp</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Pub.foo.bar.com&nbsp;是域名</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、2121&nbsp;是使用的端口</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Incoming/rls.sfv&nbsp;是当前访问的文件。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下列不属于Javascrip&nbsp;DOM操作事件的是&nbsp;C</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">A.&nbsp;onclick</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">B.&nbsp;onkeydown</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">C.&nbsp;onbodyload</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">D.&nbsp;onmouseover</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">有两张数据表，表user(id,&nbsp;name)记录了用户的ID和昵称，表article(id,&nbsp;title,&nbsp;content,&nbsp;time)记录了用户发表的文章标题、内容和时间，写一个SQL语句打印出每个用户的昵称及其发表的文章总数。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Select&nbsp;user.name,A.id,A.</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">总数&nbsp;from&nbsp;user,(select&nbsp;id,count(*)&nbsp;as&nbsp;’总数‘&nbsp;from&nbsp;article&nbsp;group&nbsp;by&nbsp;id)&nbsp;as&nbsp;A&nbsp;where&nbsp;user.id=A.id;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下列PHP函数中不能直接在页面输出字符串的函数是&nbsp;B</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">A.&nbsp;echo</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">B.&nbsp;sprintf</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">C.&nbsp;printf</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">在PHP中，‘+’操作符的功能不包括&nbsp;A</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">A.&nbsp;</span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">字符串连接</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">B.&nbsp;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">数组数据合并</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">C.&nbsp;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">变量数据相加</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面哪个选项没有将john添加到users数组中？C</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(A)&nbsp;$users[]&nbsp;=&nbsp;’john’;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(B)&nbsp;array_push($users,&nbsp;’john’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(C)&nbsp;$users&nbsp;||=&nbsp;’john’;</span></span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">(D)&nbsp;array_unshift($users,&nbsp;’john’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请列出3种PHP数组循环操作的语法，并注明每种循环的优缺点&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Foreach()&nbsp;可以遍历关联数组和索引数组，操作简单。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、For()&nbsp;只能遍历索引数组。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Each&nbsp;list&nbsp;while&nbsp;以关联和索引两种方式遍历数组，操作复杂。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请列出3个PHP中的预定义全局变量&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、$_SESSION</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、$_COOKIE</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">3</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、$_SERVER</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">4</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、$_GET</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">5</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、$_POST</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">76.</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">从PHP4.2.0开始&nbsp;PHP默认配置将register_globals配置设定为off,请指出这个设定的作用和对PHP相关程序的影响。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Register_globals=off;</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">的时候，关闭了全局变量注册，访问POST方式提交值时用$_POST[];来访问，访问GET方式提交的值时用$_GET[];方式访问。</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写一个函数实现字符串翻转&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、Strrev()</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">2</span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、自己写：</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <a></a><a><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Function&nbsp;str($a){</span></a>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$len=strlen($a);</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b=”&quot;;</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">For($i=$len-1;$i&gt;=0;$i–){</span>
</p>
<p style="margin-top:0;margin-right:0;margin-bottom:0;margin-left:28px;margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$b.=$a[$i];</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;text-indent:28px;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Return&nbsp;$b;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请写出下列PHP代码的执行结果&nbsp;</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$var1&nbsp;=&nbsp;5;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$var2&nbsp;=&nbsp;10;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">function&nbsp;foo(&amp;$my_var){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">global&nbsp;$var1;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$var1&nbsp;+=&nbsp;2;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$var2&nbsp;=&nbsp;4;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$my_var&nbsp;+=&nbsp;3;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">return&nbsp;$var2;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$my_var&nbsp;=&nbsp;5;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo&nbsp;foo($my_var)&nbsp;.&nbsp;”\n”;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo&nbsp;$my_var&nbsp;.&nbsp;”\n”;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;8</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo&nbsp;$var1&nbsp;.&nbsp;”\n”;&nbsp;&nbsp;&nbsp;7</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo&nbsp;$var2&nbsp;.&nbsp;”\n”;&nbsp;&nbsp;&nbsp;10</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$bar&nbsp;=&nbsp;’foo’;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$my_var&nbsp;=&nbsp;10;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">echo&nbsp;$bar($my_var)&nbsp;.&nbsp;”\n”;&nbsp;&nbsp;&nbsp;&nbsp;4</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">不断在文件hello.txt头部写入一行“Hello&nbsp;World”字符串，要求代码完整</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$fp=fopen(‘hello.txt’,&#39;r’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$str=’hello!’.”\n”;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$str.=fread($fp,filesize(‘hello.txt’));</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">fclose($fp);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$fp1=fopen(‘hello.txt’,&#39;w’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">fwrite($fp1,$str);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">输出用户的IP地址，并且判断用户的IP地址是否在192.168.1.100&nbsp;—&nbsp;192.168.1.150之间</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo&nbsp;$ip=getenv(‘REMOTE_ADDR’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$ip=Str_replace(‘.’,”&quot;,$ip);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">If($ip&lt;1921681150&nbsp;&amp;&amp;&nbsp;$ip&gt;1921681100){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo&nbsp;’ip</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">在192.168.1.100—–192.168.1.150之间‘;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}Else{</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">Echo&nbsp;’ip</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">不在192.168.1.100—–192.168.1.150之间‘;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">请将2维数组按照name的长度进行重新排序，按照顺序将id赋值。</span></span></strong>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&lt;?php</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$Tarray&nbsp;=&nbsp;array(</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">array(‘id’&nbsp;=&gt;&nbsp;0,&nbsp;‘name’&nbsp;=&gt;&nbsp;‘123’),</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">array(‘id’&nbsp;=&gt;&nbsp;0,&nbsp;‘name’&nbsp;=&gt;&nbsp;‘1234’),</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">array(‘id’&nbsp;=&gt;&nbsp;0,&nbsp;‘name’&nbsp;=&gt;&nbsp;‘1235’),</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">array(‘id’&nbsp;=&gt;&nbsp;0,&nbsp;‘name’&nbsp;=&gt;&nbsp;‘12356’),</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">array(‘id’&nbsp;=&gt;&nbsp;0,&nbsp;‘name’&nbsp;=&gt;&nbsp;‘123abc’)</span>
</p>
<p style="margin-top:0;margin-bottom:0;margin-left: 0;margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">)</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">foreach($tarray&nbsp;as&nbsp;$key=&gt;$val){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$c[]=$val[&#39;name&#39;];</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">function&nbsp;aa($a,$b){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">if(strlen($a)==strlen($b))&nbsp;return&nbsp;0;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">return&nbsp;strlen($a)&gt;strlen($b)?-1:1;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">usort($c,’aa’);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$len=count($c);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">for($i=0;$i&lt;$len;$i++){</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$t[$i][&#39;id&#39;]=$i+1;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">$t[$i][&#39;name&#39;]=$c[$i];</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">}</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo&nbsp;’&lt;pre&gt;’;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">print_r($t);</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">echo&nbsp;’&lt;/pre&gt;’;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style=";margin-bottom:0;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">输出为Mozilla/4.0(compatible;MSIE5.01;Window NT 5.0)时，可能的输出语句是：B</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; A</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">．$_SERVER[&#39;HTTP_USER_AGENT_TYPE&#39;];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; B. $_SERVER[&#39;HTTP_USER_AGENT&#39;];</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; C. $_SERVER[&#39;USER_AGENT&#39;];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; D. $_SERVER[&#39;AGENT&#39;];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面功能PHP无法实现的是：D</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">&nbsp;A. </span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">服务器端脚本运行</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">命令行脚本运行</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">客户端图形界面（GUI）程序</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; <span style="text-decoration:underline;"><span style="color:#333333">D. </span></span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">浏览器端执行DOM操作</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面说法不正确的是：C</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">&nbsp;A. PHP</span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">有四种标量类型：布尔型(boolean),整型(integer),浮点型(float),字符串(string)</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">浮点型(float)与双精度型(double)是同一种类型</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; <span style="text-decoration:underline;">C. </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">符合类型包括:数组(array),对象(object),资源(resource)</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">伪类型：混合型(mixed),数字型(number),回调(callback)</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">执行下面的代码后，A</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="text-decoration:underline;">&nbsp;&nbsp; &lt;?php&nbsp;&nbsp; echo&nbsp; </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">和print不是系统函数（看手册）</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo function_exists(&#39;print&#39;);&nbsp;&nbsp; imagecreatetruecolor</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp; ?&gt;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp; </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">得到的输出是：</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">&nbsp;<span style="text-decoration:underline;">A. </span></span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">空</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. true</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. false</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; &nbsp;D. FALSE</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面不是PHP语法的组成部分的函数是：AD</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; <span style="color:#333333">A. array</span></span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. eval</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. each</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; &nbsp;<span style="text-decoration:underline;">D. list</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">执行下面的代码的结果是什么？A</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $bool = TRUE;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo gettype($bool);</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo is_string($bool);</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">&nbsp;A. boolean</span></span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. boolean0</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. booleanFALSE</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. booleanfalse</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出下面代码执行的结果：12 10 18</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $a = 12;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $b = 012;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $c = 0x12;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo$a,&quot;\n&quot;,$b,&quot;\n&quot;,$c;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码的执行结果是什么？C</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp; echo 1+2+&quot;3+4+5&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; A. 0</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; B. 3</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; <span style="text-decoration:underline;">C. 6</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; D. &quot;33+4+5&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码加入下面那个函数后返回TRUE:B</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; return ? == &#39;A&#39;;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="color:#333333">&nbsp; A. ord(65)</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; <span style="text-decoration:underline;">&nbsp;B. chr(65)</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. 65+&#39;&#39;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. &#39;&#39;+65</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码的输出正确的是：C</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $a =array(1=&gt;5,5=&gt;8,22,2=&gt;&#39;8&#39;,81);</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $a[7];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $a[6];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $a[3];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="color:#333333">&nbsp;A. </span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">空2281 B.空8122<span style="text-decoration:underline;">C.8122</span><span style="text-decoration:underline;">空</span>D.空空空</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码的输出结果：D</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $a[bar]=&#39;hello&#39;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $a[bar];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo $a[&#39;bar&#39;];</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="color:#333333">&nbsp;A. hello B. </span></span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">空空 C.报错<span style="text-decoration:underline;">D.hellohello</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">写出下面代码的结果：C </span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">左右相当于乘2，右移相当于除2</span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">二进制位移后</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo 1&gt;&gt;0;&nbsp; 0001 0001</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo 2&gt;&gt;1;&nbsp; 0010 0001</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo 3&lt;&lt;2;&nbsp; 0011 1100</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="color:#333333">&nbsp;A. 012 B. 106 <span style="text-decoration:underline;">C. 1112</span> D.123</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码的执行结果：D</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php&nbsp;&nbsp; </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">中间的i少个$</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp; for($i=0;i&lt;10;$i++){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; print $i;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp; A. 0123456789 B. 012345678910 C. </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">无输出 </span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">D. </span></span><span style="text-decoration:underline;"><span style="font-size: 12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">死循环</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面对于echo, print 的描述正确的是：C</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; A. echo, print </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">都可以打印多个参数</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. print </span><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">可以打印多个参数,echo 不可以</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;<span style="text-decoration:underline;">&nbsp; C. echo&nbsp; </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">可以打印多个参数,print不可以</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. echo, print </span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">都不可以打印多个参数</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">对于正面的代码</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="text-decoration:underline;">&nbsp;&lt;?php</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $fruits = array(&#39;strawberry&#39;=&gt;&#39;red&#39;,&#39;banana&#39;=&gt;&#39;yellow&#39;);</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; </span></span><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">能够正确得到结果&#39;yellow&#39;的代码是：ACD</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="text-decoration:underline;"><span style="color:#333333">&nbsp; A. echo &quot;A banana is{$fruits[&#39;banana&#39;]}&quot;;</span></span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. echo &quot;A banana is$fruits[&#39;banana&#39;]&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. echo &quot;A banana is{$fruits[banana]}&quot;;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. echo &quot;A banana is$fruits[banana]&quot;;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面代码执行完成后的结果是什么？1&nbsp; 2</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; &lt;?php</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; function change(){</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; static $i = 0;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $i++;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return $i;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; print change();&nbsp; //1</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; print change();&nbsp; //2</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; ?&gt;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">下面的include语句不正确的是？A</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;<span style="text-decoration:underline;">&nbsp;A. include &quot;mms://www.abc.com/a.php&quot;;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; B. include&quot;http://www.abc.com/a.php&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; C. include&quot;https://www.abc.com/a.php&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; D. include&quot;ftp://www.abc.com/home/a.php&quot;;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&lt;?php</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $foo = &#39;test&#39;;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $bar = &lt;&lt;&lt;&#39;EOT&#39;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $foobar</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">EOT;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo$bar;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ?&gt;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">上面的语句输出结果 (a): A</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="color:#333333">a. $foo bar;</span></span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; b. &#39;EOT&#39; $foo bar EOT;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; c. test bar;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; d. &#39;EOT&#39; test bar EOT;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">$a=3;$b=4;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; if($a||$b=5){&nbsp;&nbsp;&nbsp; ||</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">或和|的区别</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; echo &#39;todo&#39;;</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; }</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;&nbsp; <strong><span style="text-decoration:underline;">$b</span></strong></span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family: &#39;微软雅黑&#39;,&#39;sans-serif&#39;">的值是(a): A</span></span></strong>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp; <span style="text-decoration:underline;"><span style="color:#333333">&nbsp;a. 4;</span></span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">&nbsp;<span style="color:#333333">&nbsp; b. 5;</span></span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; c. 3;</span>
</p>
<p style="text-align:left;line-height:15px">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp; d. False</span>
</p>
<p style="text-align:left;line-height:15px">
    <strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:black"><a href="http://www.mianwww.com/html/2011/12/12535.html"><span style="color:black">如何提高php</span><span style="color:black">应用的性能</span></a> </span></span></strong>
</p>
<p style="text-align:left;text-indent:28px;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">1</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">、 如果能将类的方法定义成static，就尽量定义成static，它的速度会提升将近4倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2、$row[’id’] 的速度是$row[id]的7倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3、echo 比 print快，并且使用echo的多重参数(译注：指用逗号而不是句点)代替字符串连接，比如echo$str1,$str2。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4、在执行for循环之前确定最大循环数，不要每循环一次都计算最大值，最好运用foreach代替。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5、注销那些不用的变量尤其是大数组，以便释放内存。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6、尽量避免使用__get，__set，__autoload。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 7、require_once()代价昂贵。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 8、include文件时尽量使用绝对路径，因为它避免了PHP去include_path里查找文件的速度，解析操作系统路径所需的时间会更少。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 9、如果你想知道脚本开始执行(译注：即服务器端收到客户端请求)的时刻，使用$_SERVER[‘REQUEST_TIME’]要好于 time()。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 10、函数代替正则表达式完成相同功能。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 11、str_replace函数比preg_replace函数快，但strtr函数的效率是str_replace函数的四倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 12、如果一个字符串替换函数，可接受数组或字符作为参数，并且参数长度不太长，那么可以考虑额外写一段替换代码，使得每次传递参数是一个字符，而不是只写一行代码接受数组作为查询和替换的参数。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 13、使用选择分支语句(译注：即switch case)好于使用多个if，else if语句。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 14、用@屏蔽错误消息的做法非常低效，极其低效。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 15、打开apache的mod_deflate模块，可以提高网页的浏览速度。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 16、数据库连接当使用完毕时应关掉，不要用长连接。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 17、错误消息代价昂贵。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 18、在方法中递增局部变量，速度是最快的。几乎与在函数中调用局部变量的速度相当。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 19、递增一个全局变量要比递增一个局部变量慢2倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 20、递增一个对象属性(如：$this-&gt;prop++)要比递增一个局部变量慢3倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 21、递增一个未预定义的局部变量要比递增一个预定义的局部变量慢9至10倍。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 22、仅定义一个局部变量而没在函数中调用它，同样会减慢速度(其程度相当于递增一个局部变量)。PHP大概会检查看是否存在全局变量。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 23、方法调用看来与类中定义的方法的数量无关，因为我(在测试方法之前和之后都)添加了10个方法，但性能上没有变化。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 24、派生类中的方法运行起来要快于在基类中定义的同样的方法。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 25、调用带有一个参数的空函数，其花费的时间相当于执行7至8次的局部变量递增操作。类似的方法调用所花费的时间接近于15次的局部变量递增操作。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 26、Apache解析一个PHP脚本的时间要比解析一个静态HTML页面慢2至10倍。尽量多用静态HTML页面，少用脚本。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 27、除非脚本可以缓存，否则每次调用时都会重新编译一次。引入一套PHP缓存机制通常可以提升25%至100%的性能，以免除编译开销。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 28、尽量做缓存，可使用memcached。memcached是一款高性能的内存对象缓存系统，可用来加速动态Web应用程序，减轻数据库负载。对运算码 (OP code)的缓存很有用，使得脚本不必为每个请求做重新编译。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 29、当操作字符串并需要检验其长度是否满足某种要求时，你想当然地会使用strlen()函数。此函数执行起来相当快，因为它不做任何计算，只返回在zval 结构(C的内置数据结构，用于存储PHP变量)中存储的已知字符串长度。但是，由于strlen()是函数，多多少少会有些慢，因为函数调用会经过诸多步骤，如字母小写化(译注：指函数名小写化，PHP不区分函数名大小写)、哈希查找，会跟随被调用的函数一起执行。在某些情况下，你可以使用isset() 技巧加速执行你的代码。<br/> (举例如下)<br/> if (strlen($foo) &lt; 5) { echo “Foo is too short”$$ }<br/> (与下面的技巧做比较)<br/> if (!isset($foo{5})) { echo “Foo is too short”$$ }<br/> 调用isset()恰巧比strlen()快，因为与后者不同的是，isset()作为一种语言结构，意味着它的执行不需要函数查找和字母小写化。也就是说，实际上在检验字符串长度的顶层代码中你没有花太多开销。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 34、当执行变量$i的递增或递减时，$i++会比++$i慢一些。这种差异是PHP特有的，并不适用于其他语言，所以请不要修改你的C或 Java代码并指望它们能立即变快，没用的。++$i更快是因为它只需要3条指令(opcodes)，$i++则需要4条指令。后置递增实际上会产生一个临时变量，这个临时变量随后被递增。而前置递增直接在原值上递增。这是最优化处理的一种，正如Zend的PHP优化器所作的那样。牢记这个优化处理不失为一个好主意，因为并不是所有的指令优化器都会做同样的优化处理，并且存在大量没有装配指令优化器的互联网服务提供商(ISPs)和服务器。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 35、并不是事必面向对象(OOP)，面向对象往往开销很大，每个方法和对象调用都会消耗很多内存。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 36、并非要用类实现所有的数据结构，数组也很有用。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 37、不要把方法细分得过多，仔细想想你真正打算重用的是哪些代码?<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 38、当你需要时，你总能把代码分解成方法。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 39、尽量采用大量的PHP内置函数。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 40、如果在代码中存在大量耗时的函数，你可以考虑用C扩展的方式实现它们。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 41、评估检验(profile)你的代码。检验器会告诉你，代码的哪些部分消耗了多少时间。Xdebug调试器包含了检验程序，评估检验总体上可以显示出代码的瓶颈。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 42、mod_zip可作为Apache模块，用来即时压缩你的数据，并可让数据传输量降低80%。<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 43、在可以用file_get_contents替代file、fopen、feof、fgets等系列方法的情况下，尽量用 file_get_contents，因为他的效率高得多!但是要注意file_get_contents在打开一个URL文件时候的PHP版本问题;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 44、尽量的少进行文件操作，虽然PHP的文件操作效率也不低的;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 45、优化Select SQL语句，在可能的情况下尽量少的进行Insert、Update操作;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 46、尽可能的使用PHP内部函数(但是我却为了找个PHP里面不存在的函数，浪费了本可以写出一个自定义函数的时间，经验问题啊!);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 47、循环内部不要声明变量，尤其是大变量：对象(这好像不只是PHP里面要注意的问题吧?);<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 48、多维数组尽量不要循环嵌套赋值;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 49、在可以用PHP内部字符串操作函数的情况下，不要用正则表达式;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 50、foreach效率更高，尽量用foreach代替while和for循环;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 51、用单引号替代双引号引用字符串;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 52、“用i+=1代替i=i+1。符合c/c++的习惯，效率还高”;<br/> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 53、对global变量，应该用完就unset()掉。</span>
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333"><br/> </span><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">13</span></span></strong><strong><span style="text-decoration:underline;"><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;">、谈谈asp,php,jsp的优缺点(1分)<br/> </span></span></strong><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ASP</span><span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">全名Active Server Pages，是一个WEB服务器端的开发环境， 利用它可以产生和运<br/> 行动态的、交互的、高性能的WEB服务应用程序。ASP采用脚本语言VB Script（Java script<br/> ）作为自己的开发语言。<br/> 　　 PHP是一种跨平台的服务器端的嵌入式脚本语言. 它大量地借用C,Java和Perl语言的语法<br/> , 并耦合PHP自己的特性,使WEB开发者能够快速地写出动态生成页面.它支持目前绝大多数数<br/> 据库。还有一点，PHP是完全免费的，不用花钱，你可以从PHP官方站点(http://www.php.ne<br/> t)自由下载。而且你可以不受限制地获得源码，甚至可以从中加进你自己需要的特色。<br/> 　　 JSP 是Sun公司推出的新一代站点开发语言，他完全解决了目前ASP,PHP的一个通病－－<br/> 脚本级执行（据说PHP4 也已经在Zend 的支持下，实现编译运行）.Sun 公司借助自己在Jav<br/> a 上的不凡造诣，将Java 从Java 应用程序 和 Java Applet 之外，又有新的硕果，就是Js<br/> p－－Java Server Page。Jsp 可以在Serverlet和JavaBean的支持下，完成功能强大的站点<br/> 程序。<br/> 　　 三者都提供在 HTML 代码中混合某种程序代码、由语言引擎解释执行程序代码的能力。<br/> 但JSP代码被编译成 Servlet 并由 Java 虚拟机解释执行，这种编译操作仅在对 JSP 页面的<br/> 第一次请求时发生。在 ASP 、PHP、JSP 环境下， HTML 代码主要负责描述信息的显示样式<br/> ，而程序代码则用来描述处理逻辑。普通的 HTML 页面只依赖于 Web 服务器，而 ASP 、PH<br/> P、JSP 页面需要附加的语言引擎分析和执行程序代码。程序代码的执行结果被重新嵌入到<br/> HTML 代码中，然后一起发送给浏览器。 ASP 、PHP、 JSP三者都是面向 Web 服务器的技术<br/> ，客户端浏览器不需要任何附加的软件支持。</span>
</p>
<p>
    <strong>在quirks mode 和 strict mode中还有一个区别</strong>?
</p>
<p>
    在<strong>strict mode</strong> 中:
</p>
<p style="margin-left:112px;text-indent:28px">
    <strong>table的css属性font-size会继承父级元素的</strong> ，也就是说，table中的字体大小会继承父级元素字体的大小。
</p>
<p>
    在<strong>quirks mode</strong> 中:
</p>
<p style="margin-left:112px;text-indent:28px">
    <strong>table的css属性font-size不会继承父级元素的</strong> ，需要专门设置一下。也就是说，table中的字体大小不会继承父级元素字体的大小。
</p>
<p style="text-align:left;line-height:15px;text-autospace:ideograph-other">
    <span style="font-size:12px;font-family:&#39;微软雅黑&#39;,&#39;sans-serif&#39;;color:#333333">&nbsp;</span>
</p>
<p>
    <br/>
</p>
