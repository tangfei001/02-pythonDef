**20-内部函数lambda匿名函数的讲解**

格式:date=lambda x,y:x+y

	date(3,4)

实例一:

login =lambda username,password:print("登录成功") if username == "admin" and password ==123456 else print("打印失败")

print(login("admin",123456))

实例二:\

date = lambda **kwargs:dict(sorted(kwargs.items(),key=lambuda item:item[0]))

print(date(name="admin",age="18"))
-------------------------------------------

lambda x: xxxxxx   xxxx:要实现的功能