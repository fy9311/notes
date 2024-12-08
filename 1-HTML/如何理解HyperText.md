#html
### MarkUp(标记)

Markup（标记）的核心思想是用特定的标记来描述文本的结构和样式，而不是直接展示内容本身。
例如：
```html
// 没标记的纯文本
小明的个人简历

个人信息
姓名：小明
年龄：25岁
邮箱：xiaoming@example.com

工作经历
2020-2022 ABC公司
负责前端开发工作

教育背景
2016-2020 某大学计算机系

// 加入标记后
<article class="resume">
    <h1>小明的个人简历</h1>
    <section class="personal-info">
        <h2>个人信息</h2>
        <ul>
            <li><strong>姓名：</strong>小明</li>
            <li><strong>年龄：</strong>25岁</li>
            <li><strong>邮箱：</strong><a href="mailto:xiaoming@example.com">xiaoming@example.com</a></li>
        </ul>
    </section>
    <section class="work-experience">
        <h2>工作经历</h2>
        <div class="job">
            <time>2020-2022</time>
            <h3>ABC公司</h3>
            <p>负责前端开发工作</p>
        </div>
    </section>
    <section class="education">
        <h2>教育背景</h2>
        <div class="edu-item">
            <time>2016-2020</time>
            <p>某大学计算机系</p>
        </div>
    </section>
</article>
```

### 标记的作用：
1. 结构化文档
	1. 通过section划分模块
	2. 通过h1 h2来表明标题层级
2. 定义内容类型
	1. ul表示列表
	2. time表示时间
	3. a表示链接
3. 添加额外信息，语义增强
	 
### 带来的好处：

- 对机器友好
	- 搜索引擎更容易理解内容
	- 屏幕阅读器能更好地解读内容
	- 爬虫更容易提取信息

- 对开发友好
	- 容易添加样式
	- 便于 JavaScript 操作
	- 方便维护和修改

- 对用户友好
	- 可以点击邮箱链接
	- 可以设置不同的显示样式
	- 支持响应式布局
