#Standard Markdown

##Strong and Emphasize
```
*emphasize*   **strong**
_emphasize_   __strong__
```
##Links and Email
Inline:
```
An [example](http://url.com/ "Title")
```
Reference-style labels (titles are optional):
```

An [example][id]. Then, anywhere
else in the doc, define the link:

  [id]: http://example.com/  "Title"
```
Email:
```
An email <example@example.com> link.
```

##Images
Inline (titles are optional):
```
![alt text](/path/img.jpg "Title")
```
Reference-style:
```
![alt text][id]

[id]: /url/to/img.jpg "Title"
```
##Headers
```
Setext-style:

Header 1
========

Header 2
--------
```
atx-style (closing #’s are optional):
```
# Header 1 #

## Header 2 ##

###### Header 6
```
##Lists
Ordered, without paragraphs:
```
1.  Foo
2.  Bar
```
Unordered, with paragraphs:
```
*   A list item.

    With multiple paragraphs.

*   Bar
```
You can nest them:
```
*   Abacus
    * answer
*   Bubbles
    1.  bunk
    2.  bupkis
        * BELITTLER
    3. burper
*   Cunning
```
##Blockquotes
```
> Email-style angle brackets
> are used for blockquotes.

> > And, they can be nested.

> #### Headers in blockquotes
> 
> * You can quote a list.
> * Etc.
```
##Inline Code
```
`<code>` spans are delimited
by backticks.

You can include literal backticks
like `` `this` ``.
```
##Block Code
Indent every line of a code block by at least 4 spaces or 1 tab.
```
This is a normal paragraph.

    This is a preformatted
    code block.
```
##Horizontal Rules
Three or more dashes or asterisks:
```
---

* * *

- - - -
```
##Hard Line Breaks
End a line with two or more spaces:
```
Roses are red,   
Violets are blue.```

##Git的功能特性
###从一般开发者的角度来看
1. 1、从服务器上克隆完整的Git仓库（包括代码和版本信息）到单机上。
2. 2、在自己的机器上根据不同的开发目的，创建分支，修改代码。
3. 3、在单机上自己创建的分支上提交代码。
4. 4、在单机上合并分支。
5. 5、把服务器上最新版的代码fetch下来，然后跟自己的主分支合并。
6. 6、生成补丁（patch），把补丁发送给主开发者。
7. 7、看主开发者的反馈，如果主开发者发现两个一般开发者之间有冲突（他们之间可以合作解决的冲突），就会要求他们先解决冲突，然后再由其中一个人提交。如果主开发者可以自己解决，或者没有冲突，就通过。
8. 8、一般开发者之间解决冲突的方法，开发者之间可以使用pull 命令解决冲突，解决完冲突之后再向主开发者提交补丁。
###从项目管理者的角度看
1. 1、查看邮件或者通过其它方式查看一般开发者的提交状态。
2. 2、打上补丁，解决冲突（可以自己解决，也可以要求开发者之间解决以后再重新提交，如果是开源项目，还要决定哪些补丁有用，哪些不用）。
3. 3、向公共服务器提交结果，然后通知所有开发人员。

##感激
    感谢以下的项目,排名不分先后
* [git](https://github.com)

##代码格式

```javascript
  var ihubo = {
    nickName  : "123",
    site : "http://123.me"
  }
```