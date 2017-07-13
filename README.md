## **定义字符集**

[a-e]表示a到e这些字符中的某一个字符

[a-z]26个字母之一

[aeiou]表示aeiou这5个字符其中的某一个字符

[a-zA-Z]表示大写、小写字母中的某一个字符

[a-zA-Z0-9_-]表示大写、小写字母、数字、_、-中的某一个字符

[0-9]表示0到9之间任意一个数字

[5-9]表示5到9之间的任意一个数字

## **特别字符**

$ : 匹配输入字符串的结尾位置

^ (托字符) : 表示字符串的开始位置(托字符)

( ): 标记一个子表达式的开始和结束位置

\* : 其前面那个单元出现0次或以上（任意次数）

\+ : 其前面那个单元出现1次或以上

? : 其前面那个单元出现0次或1次

\. : 匹配除换行符 \n之外的任何单字符 

\ : 这个符号是用来转义的

| : 指明两项之间的一个选择

****

## **组合字符**

\d :表示数字[0-9]\D :表示非数字\[^0-9]

\w :表示字母、数字、下划线其中一个[a-zA-Z0-9_]

\W :非字母、数字、下划线

\s :表示空格

\S :表示非空格

\b :表示单词边界

\B :表示非单词边界

## **限定字符**

{m} : 其前一单元严格出现m次

{m,} : 其前一单元出现至少m次，至多不限制

{m,n} : 其前一单元出现至少m，至多n次

[^lsjd]: 不是中括号中的任意一个字符\[^a-f]: 不是中括号中中杠的两端字符范围var reg = /^apple/; 匹配内容开始有apple字样var reg = /\[^a-h]/; 不给匹配a-h之间的字母，可以匹配其他字符

## **重复使用模式单元**


**正向预查**具体内容(?=pattern) 正向匹配具体内容(?!pattern) 正向不匹配
**反向预查(php支持)**(?<=pattern)具体内容 反向匹配(?<!pattern)具体内容 反向不匹配