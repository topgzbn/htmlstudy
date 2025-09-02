# 1.语义化标签
```html
  <h2>有语义强调与重要性标签</h2>

  加粗： <strong>加粗文字</strong>

  倾斜: <em>倾斜文字</em>

  下划线： <ins>下划线</ins>

  删除线： <del>删除线</del>


  <h2>无语义强调与重要性标签</h2>

  加粗： <b>加粗文字</b>

  倾斜： <i>倾斜文字</i>

  下划线： <u>下划线</u>

  删除线: <s>删除线</s>

  

  <h2>注释标签</h2>

  <!-- 这段文字是看不见的 -->
```
总结：有语义强调与重要性标签常用
# 2.图像标签
```html
  <h2>图像标签的基本使用：</h2>

  <img src="pig.png" alt="猪爸爸">

  

  <h2>图像标签修改宽度和高度：</h2>

  <img src="pig.png" alt="猪爸爸" width="300">

  <!-- 一般情况下，我们宽度和高度修改其中一个就可以了，剩下的等比例缩放 -->

  <img src="pig.png" alt="猪爸爸" width="300" height="300">

  <h2>图像标签添加title 图像标题：</h2>

  <img src="pig.png" alt="猪爸爸" width="300" title="猪爸爸">

  

  <h2> 插入图片不同的格式：</h2>

  <img src="img/1.jpg" alt="">

  <img src="img/2.webp" alt="">

  <img src="img/4.avif" alt="">

  <img src="img/5.gif" alt="">

  <img src="img/login.png" alt="">
```
# 3.音视频标签
```html
<h2>视频标签</h2>

  <!-- 在h5中如果属性的 键 和值是相同的，则可以省略值 -->

  <!-- <video src="./media/test.mp4" width="400" controls="controls"></video> -->

  <!-- 想要自动播放 autoplay，需要先静音 muted ， 循环播放loop -->

  <!-- <video src="./media/test.mp4" width="400" controls autoplay muted loop poster="./media/yu7.jpg"></video> -->

  <!-- <video src="./media/test.mp4" width="400" controls muted loop poster="./media/yu7.jpg"></video> -->

  

  <!-- 兼容性写法 -->

  <video width="400" controls muted loop poster="./media/yu7.jpg">

    <source src="./media/test.mp4" type="video/mp4">

    <p> 您的浏览器不支持视频播放 </p>

  </video>

  
  

  <h2>音频标签</h2>

  <!-- 音频标签浏览器不让自动播放 后续可以用js实现 -->

  <audio src="./media/test.mp3" controls muted autoplay></audio>

  <!-- 兼容性写法 -->

  <audio controls>

    <source src="./media/test.mp3" type="audio/mp3">

    <p> 您的浏览器不支持音频播放 </p>

  </audio>
```

# 4.链接标签
```html
    1. 内部链接 <br>

    <a href="#2"> 2. 外部链接</a> <br>

    <a href="#3">3. 空链接</a> <br>

    2. 下载链接 <br>

    3. 邮件链接 <br>

  

  <h2>1. 内部链接</h2>


  <p>超链接使我们能够将我们的文档链接到任何其他文档（或其他资源），也可以链接到文档的指定部分，我们可以在一个简单的网址上提供应用程序。几乎任何网络内容都可以转换为链接，点击（或激活）超链接将使网络浏览器转到另一个网址（URL）。

  </p>

  例如：

  <a href="./11-音视频标签.html">音视频</a>

  如果有需要作为链接的图片，使用 a元素来包裹要引用图片的 img 元素。下面的示例使用相对路径来引用本地存储的 SVG 图像文件。

  

  <h2 id="2">2. 外部链接</h2>

  

  例如：

  <a href="https://www.deepseek.com/" title="deepseek" target="_blank">deepseek</a>

  你可能要添加到你的链接的另一个属性是 title。这旨在包含关于链接的补充信息，例如页面包含什么样的信息或需要注意的事情。

  

  <h2 id="3">3. 空连接 </h2>

  

  <p>在 HTML 中，空连接（Empty Link）通常指的是没有指定 href 属性或 href 属性值为空的 a标签。

    空连接的 href 属性值为空字符串（""）或 # 字符。</p>

  例如：

  <a href="">点击跳转到顶部</a>

  <p>空链接点击默认会跳到当前页面的顶部。</p>

  <p>空连接的作用是为了提供一个占位符，用于在页面的特定位置创建一个目标，以便其他链接或脚本可以跳转到该位置。这在页面布局中非常有用，尤其是当你需要在页面的不同部分之间创建导航链接时。</p>

  

  <h2>4. 下载链接 </h2>

  

  <a href="./download.zip">下载软件</a>

  <p>下载链接是一种特殊类型的链接，用于将文件从服务器下载到用户的计算机上。当用户点击下载链接时，它会触发浏览器的下载功能，将文件保存到用户的本地存储中，而不是直接在浏览器中显示文件内容。</p>

  <p>下载链接通常用于提供软件、文档、图片或视频等可下载资源，以便用户可以离线使用或分享给他人。</p>

  

  <h2>5. 邮件链接 </h2>

  

  <p>当点击一个链接或按钮时，可能会开启新的邮件的发送而不是连接到一个资源或页面。这种场景可以使用 <a> 元素和 mailto: URL 协议实现。</p>

  

  <p> 其最基本和最常用的使用形式为一个指明收件人电子邮件地址的 mailto: 链接。例如：</p>

  <a href="mailto:123@qq.com">联系我们</a>
```
# 5.网页结构标签以及div和span标签
```html
  <h2>网页结构标签</h2>

  <header>网页头部标签</header>

  <nav>导航栏标签</nav>

  <main>

    <aside>侧边栏标签</aside>

    <article>主要内容区域标签</article>

  </main>

  <footer>页面底部标签</footer>

  <section>区块标签</section>

  

  <h2>div和span标签 </h2>

  <div>我是div标签是块级元素</div>

  <div>我是div标签是块级元素</div>

  <span>我是span标签是行内元素</span>

  <span>我是span标签是行内元素</span>
```
# 6.列表标签
```html
  <h2>一.无序列表</h2>

  <ul>

   <li>看视频</li>

    <li>写代码</li>

  </ul>

  

  <h2>二.有序列表（了解即可）</h2>

  <ol>

    <li>看视频</li>

    <li>写代码</li>

  </ol>

  

  <h2>三.描述列表（自定义列表）</h2>

  <dl>

    <dt>水果</dt>

    <dd>苹果</dd>

    <dd>西瓜</dd>

    <dd>桃子</dd>

  </dl>
```
总结：常用ul无序列表
# 7.表格标签
## 7.1基本用法
```html
  <h2>表格标签基本语法</h2>

    <table border="1">

    <tr>

      <th>姓名</th>

      <th>年龄</th>

      <th>性别</th>

      <th>爱好</th>

      <th>居住地</th>

    </tr>

    <tr>

      <td>张三</td>

      <td>18</td>

      <td>男</td>

      <td>足球</td>

      <td>北京</td>

    </tr>

    <tr>

      <td>李四</td>

      <td>20</td>

      <td>女</td>

      <td>篮球</td>

      <td rowspan="2">深圳</td>

    </tr>

    <tr>

      <td>王五</td>

      <td>22</td>

      <td>男</td>

      <td>篮球</td>

  

    </tr>

    <tr>

      <td>合计</td>

      <td colspan="4"></td>

    </tr>

  </table>
```
总结：rowspan：行合并；colspan列合并
## 7.2表格结构标签
```html
  <table border="1">

    <thead>

      <tr>

        <th>姓名</th>

        <th>年龄</th>

        <th>成绩</th>

      </tr>

    </thead>

    <tbody>

      <tr>

        <td>张三</td>

        <td>18</td>

        <td>100</td>

      </tr>

      <tr>

        <td>李四</td>

        <td>20</td>

        <td>90</td>

      </tr>

      <tr>

        <td>王五</td>

        <td>22</td>

        <td>80</td>

      </tr>

    </tbody>

  </table>
```
# 8.表单标签
```html
  <form action="">

    <!-- 1. 单行文本框和密码框 -->

    <ul>

      <li>

        <label>

          账号： <input type="text" placeholder="请输入账号" name="username" accesskey="s" autocomplete="off">

        </label>

      </li>

      <li>

        密码： <input type="password" placeholder="请输入密码" name="pwd" maxlength="6">

      </li>

      <!-- 2. 单选框 复选框和文件域 -->

      <li>

        性别：

        <!-- label 方式一   for  id 关联 -->

        <input type="radio" name="gender" value="0" checked id="nv">

        <label for="nv">女</label>

        <input type="radio" name="gender" value="1" id="nan">

        <label for="nan">男</label>

      </li>

      <li>

        爱好：

        <!-- label 方式二 -->

        <label>

          <input type="checkbox" name="hobby" value="0" checked> 足球

        </label>

        <label>

          <input type="checkbox" name="hobby" value="1"> 篮球

        </label>

        <label>

          <input type="checkbox" name="hobby" value="2"> 双色球

        </label>

  

      </li>

      <li>

        头像：

        <input type="file" name="file" multiple accept=".exe,.jpg">

      </li>

      <!-- 文本域 下拉列表和button按钮 -->

      <li>

        <label>

          留言：

          <textarea name="msg" cols="30" rows="10" placeholder="请输入留言"></textarea>

        </label>

      </li>

      <li>

        城市：

        <select name="city" id="">

          <option value="北京">北京</option>

          <option value="上海" selected>上海</option>

          <option value="广州">广州</option>

        </select>

      </li>

      <li>

        <button disabled>注册</button>

      </li>

    </ul>

  

  </form>
```
# 9.特殊字符
```html
   特殊字符：

  <div>

    &nbsp; 空格

    &lt; 小于号

    &gt; 大于号

    &copy; 版权符号

    &reg; 注册商标

    &yen; 人民币符号

    &cent; 分

    &pound; 英镑符号

    &euro; 欧元符号

    &amp; 与符号

    &quot; 双引号

  </div>
```
