# package archive/tar

> Package tar implements access tar archive. It aims to cover most of the variations, including those produced by BSD and GNU tars.
***
> tar 包实现对tar归档文件的读取和写入。它的目标包含大部分的tar包之间的差异，包括BSD和GNU的tar文件。

在阅读这个包的源码之前，先互相一下我们对时间的几种常用场景：
    1. 获取当前时间  
    2. 当前时间的一段时间之前或之后
    3. 周期性的时间间隔

##### 获取当前时间
Go中对应的API如下：
```
    func Now() time.Time
```
对应的Time结构如下：
```
    type Time struct{
        
    }
```
