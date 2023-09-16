# python-AI-12-
python+AI笔记(12)
#元组和列表的最大区别是元组是不可修改的
#但元组里面嵌套一个list列表，这个列表是可以修改的
t9=(1,2,["bala","cala"])
print(f"t9的内容是:{t9}")
t9[2][0]="bala"
t9[2][1]="cala"
print(f"t9的内容是:{t9}")

# 一阶-六章-字符串的定义和操作
my_str="bala and cala"
value=my_str[2]  #取l
value2=my_srt[-11]  #取l
print(f"从字符串{my_str}取下标为2的元素,值是:{value},取下标为-11的元素，值是:{value2}")
#字符串和元组一样，是一个不可修改的数据容器
my_str[2]="L"  #输出错误，字符串是不支持修改的

value=my_str.index("and")
print(value)

#字符串的替换
new_my_str=my_str.replace("ba","程序")
print(new_my_str)

#split方法
my_str="hello python bala cala"
my_str_list=my_str.split(" ")
print(f"将字符串{my_str}进行split切分后得到:{my_str_list},类型是:{type(my_str_list)})

#strip方法
my_str="  bala and cala  "
new_my_str=my_str.strip()  #不穿入参数，就是取出首位空格
print(f"字符串{my_str}被strip后，结果:{new_my_str}")  #字符串原本有空格，strip之后就没有空格了

my_str="12bala and cala21"
new_my_str=my_str.strip("12")
print(f"字符串{my_str}被strip('12')后，结果:{new_my_str}")  #strip输出后将12和21都消除掉了

my_str="bala and cala"
count=my_str.count("la")
print(f"字符串{my_str}中la出现的次数是:{count}")

num=len(my_str)
print(f"字符串{my_str}的长度是:{num}")
