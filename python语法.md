https://markdown.com.cn/basic-syntax/
## 类 Class
Python的类名必须是由一个或多个有意义的单词连缀而成的，每个单词首字母大写，其他字母全部小写，单词与单词之间不要使用任何分隔符。<br>
```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    xs = 0
    print("Hello my name is " + self.name)

p1 = Person("Bill", 63)
p1.myfunc()
```
Python的类定义由类头（指 ```class``` 关键字和类名部分）和统一缩进的类体构成，在类体中最主要的两个成员就是类变量和方法。<br>
类中各成员之间的定义顺序没有任何影响，各成员之间可以相互调用。<br>
**类变量**属于类本身，用于定义该类本身所包含的状态数据<br>
定义在```def```函数之外，比如```hair = 0```<br>
**实例变量**则属于该类的对象，用于定义对象所包含的状态数据<br>
定义在```def```函数里面，比如上面的```xs = 0```<br>
**方法**则用于定义该类的对象的行为或功能实现，第一个参数为```self```<br>
```__init__```为构造方法，用于构造该类的对象。<br>

## Assert
```python
assert expression
# equal to
if not expression:
    raise AssertionError
```
当expression不成立时，触发异常。
