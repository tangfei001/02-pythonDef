**21-内部函数map的讲解**
#简化前
list1=[1,2,3,4]

def f1():
	list2=[]
	for i in list1:
		i+=100
		list2.append(i)
	print(list2)

f1()

#简化后
list3 =[1,2,3,4,5]

print(list(map(lambda a:a+100,list3))) #map的第一个参数是函数,第二个参数是可迭代的请求参数
--------------------------------------------------------------------------------------

map(x,y)
x== lambda a:1+100
y==list3

map(lambda a:a+100,list3)
print(list(map(lambda a:a+100,list3)))