---
marp: true
theme: PKUSimple
paginate: true
---
<!-- 
_class: title 
_paginate: false
-->
# 在这里输入标题总共这么多字这里是第二行标题 H1
## 在这里输入副标题  h2
### 作者 H3
#### 日期 H4

---
<!-- 
_class: content
_paginate: false 
-->
# 目录 H1
## Content H2
### **01** 基本样式 H3
### **02** 列表
### **03** 代码
### **04** 表格
### **05** 公式
### **06** 图片
### **07** 分栏

---
<!--
_class: chapter
-->
# 01 基本样式

---
<!-- _header: 使用header来添加标题-->
# H1 标题一
## H2 标题二
### h3 标题三
#### h4 标题四
##### h5 标题五
###### h6 标题六
Normal
**Bold**

> 引用文字

<!-- _footer: 使用footer来添加参考文献 -->

---
<!-- _header: 列表-->

- 无序列表
- 无序列表
  - 无序列表
- 无序列表

1. 有序列表
2. 有序列表
   1. 有序列表
3. 有序列表
   

---
<!-- _header: 代码-->
# 代码块
## Python
```python
import torch
print(torch.cuda.is_available())
```

## C++
```C++
#include <iostream>
using namespace std;
int main() {
    cout << "Hello world" << endl;
}
```

# 行间代码
这个是行间代码`this is code`

---
<!--_header: 表格-->

|  表头   | 表头  | 表头 |
|  ----  | ----  |--- |
| 单元格  | 单元格 |单元格|
| 单元格  | 单元格 |单元格|

---
<!--_header: 公式-->
# 行内公式
行内公式 $123$
# 行间公式

$$

D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases} 

$$

---
<!-- _header: 图片-->
>**命令换行时图片换行**

![img h:130px](images/PKUlogo_long.png) ![img w:200px](images/kenkyu_woman_seikou.png)
![img w:200px](images/kenkyu_woman_seikou.png)

---
<!--
_header: 分栏 
_class: split
 -->
# 等分
<div class=columns>
<div>

## Column 1

Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas eveniet, corporis commodi vitae accusamus obcaecati dolor corrupti eaque id numquam officia velit sapiente incidunt dolores provident laboriosam praesentium nobis culpa.

</div>

<div>

## Column 2

Tempore ad exercitationem necessitatibus nulla, optio distinctio illo non similique? Laborum dolor odio, ipsam incidunt corrupti quia nemo quo exercitationem adipisci quidem nesciunt deserunt repellendus inventore deleniti reprehenderit at earum.

</div>
</div>

---
<!--
_header: 分栏 
_class: split
 -->
# 不等分
<div class=columns style="grid-template-columns: 30% 70%">
  <div>
    <img src="./images/sample_thss_img.png" width=100% >
  </div>
  <div>

  ## Column 2
  调整 `grid-teplate-columns` 参数来调整栏的数目和宽度
  **注意** 
  在`<div>`中只能使用`<img>`这样的 HTML tag 来进行图片插入
  不接受类似`![img](image path)`的语法
  但是接受 `#` 语法

  </div>
</div>

---
![bg right contain](./images/sample_thss_img.png)
# 分栏2
当然也可以直接使用bg的方式来对图片进行分栏
在这样的情况下可能无法使用header
