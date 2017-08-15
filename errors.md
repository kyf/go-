# package errors

> Package errors implements functions of manipulate errors.

在说这个包之前先说一下Go的接口机制：只要实现了接口所有定义方法的结构体默认就认为实现了该接口，无需显式声明。
本质上Go中的error是一个包含Error的方法，原型定义如下：
```
    type error interface{
        Error() string
    }
```

结下来看一下errors包中的API：
```
    func New(string) error
```
只有这一个，而这个的作用就是把string包装成error类型
