# 第8章

## if语句
单条件判断：
```python
if expression:
  expr_true_suite
```
多条件判断：
```python
if not warn and (system_load>=10):
  print ("WARNING: losing resourses")
  warn += 1
```
 可以单行写一个仅包含一行代码的复合语句：
 ```python
 if make_hard_copy:send_data_to_printer()
 ```
 ## else语句
 ```python
 if expression:
  expr_true_suite
 else:
  expr_false_suite
 ```
 example：
 ```python
  if passwd == user.passwd:
    ret_str = "password accepted"
    id = user.id
    valid = True
   else:
    ret_str = "invalid password entered....try again!"
    valid = False
  ```
   ## elif语句
   ```python
   if expression1:
    expr1_true_suite
   elif expression2:
    expr2_true_suite
   elif expressionN:
    exprN_true_suite
   else:
    none_of_the_above_suite
   ``` 
   ## 条件表达式（三元操作符）
   ```python
   X if C else Y
   ```
   ## while语句
   ```python
   while expression:
    suite_to_repeat
   ```
   ## for语句
   ```python
   for iter_var in iterable:
    suite_to_repeat
   ```
   ## pass语句
   ```python
   def foo_func():
    pass            #可以用来先定结构，而不干扰其他代码
   ```   
      
   ## range()
   ```python
   range(start, end, step=1)
   range(end)   # 默认start=0，step=1
   range(star, end) #默认start=0
   ```
   ## 序列相关的内建函数
   ```python
   sorted()   #返回一个有序序列
   reversed()   #反转一个序列
   enumerate()    #返回迭代器
   zip()    #压缩两个列表为对应元组
   zip(*zipped)   #解压，返回为二维矩阵形式
   ```
   
   example：
   ```python
seq = [11, 12, 13, 1, 4, 34, 45, 56, 6, 67, 78, 3]
seq2 = [0, 1]
seq3 = [2, 3]

sorted_seq = sorted(seq)
print(sorted_seq)

reversed_seq = reversed(seq)
print(list(reversed_seq))

enumerate_seq = enumerate(seq)
print(list(enumerate_seq))

zipped_seq = zip(seq2, seq3)
print(list(zipped_seq))

unzip_seq = zip(*zipped_seq)
print(list(unzip_seq))
   ```
   
   ## break和continue
   break：结束当前循环然后跳到下一条语句
   continue：终止当前循环，并忽略剩余的语句，然后回到循环的顶端，开始下一次循环。
   
   ## 迭代器和iter（）函数
   ### 迭代
   可迭代的类型：字符串、列表、元组、字典、集合——可被for循环：内部实现了__iter__方法
   ```python
from collections.abc import Iterable

l = [1, 2, 3, 4]
t = (1, 2, 3, 4)
d = {1: 2, 3: 4}
s = {1, 2, 3, 4}

print(isinstance(l, Iterable))
print(isinstance(t, Iterable))
print(isinstance(d, Iterable))
print(isinstance(s, Iterable))
   ```
   
      
    
