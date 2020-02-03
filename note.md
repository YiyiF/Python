# 第8章

## if语句
单条件判断：
'''python
if expression:
  expr_true_suite
 '''
多条件判断：

if not warn and (system_load>=10):
  print ("WARNING: losing resourses")
  warn += 1
  
 可以单行写一个仅包含一行代码的复合语句：
 if make_hard_copy:send_data_to_printer()
 
 ## else语句
 if expression:
  expr_true_suite
 else:
  expr_false_suite
  
 example：
 
  if passwd == user.passwd:
    ret_str = "password accepted"
    id = user.id
    valid = True
   else:
    ret_str = "invalid password entered....try again!"
    valid = False
    
   ## elif语句
   if expression1:
    expr1_true_suite
   elif expression2:
    expr2_true_suite
   elif expressionN:
    exprN_true_suite
   else:
    none_of_the_above_suite
    
   ## 条件表达式（三元操作符）
   X if C else Y
   
   ## while语句
   while expression:
    suite_to_repeat
    
   ## for语句
   for iter_var in iterable:
    suite_to_repeat
   
   ## pass语句
   def foo_func():
    pass            #可以用来先定结构，而不干扰其他代码
      
      
      
      
      
      
    
