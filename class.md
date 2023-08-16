# 类和对象

## 定义类

```python
class Bill():
    def study(self,coursename):
        print(f'Bill is studying{coursename}')

    def play(self):
        print(f'Bill is play')

```

## 初始化类

```python
class person():
    def __init__(self,name,age):
        self.name = name
        self.age =age

    def study(self,coursename):
        print(f'{self.name} is studying{coursename}')

    def play(self):
        print(f'{self.name} is play')
```

* __init__ 方法用于初始化
  * 内部定义的属性，属于类的属性。
  
## 打印对象

```python
class person():
    def __init__(self,name,age):
        self.name = name
        self.age =age

    def study(self,coursename):
        print(f'{self.name} is studying{coursename}')

    def play(self):
        print(f'{self.name} is play')
    
    def __repr__(self):
        return f'{self.name}:{self.age}'

```

* 定义了__repr__方法
* self传入的是这个类的属性

