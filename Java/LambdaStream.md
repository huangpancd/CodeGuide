# Lambda、Stream

## Lambda

## 函数式接口

### 自定义函数式接口

```java
@FunctionalInterface
interface SayHello
{
    void sayMessage(String message);
}

public class GreetingService {
    public static void main(String[] args) {
        SayHello sayHello = message -> {
            System.out.println("Say Hello " + message);
        };
        sayHello.sayMessage("Ni hao");
    }
}
```

### 内置函数式接口

To do



## Stream（日常开发中经常会用到）

stream是从Java8开始引入的。用来“做什么而非怎么做”的方式处理集合。

stream提供了一种更直观的操作容器的方式。之前操作容器往往需要显式的使用循环。而使用stream之后，对容器的处理更加直观了。

stream方法实现在Collection接口中。

### 常用的操作

### 创建流





| 操作名                                            | 操作介绍                    |
| ------------------------------------------------- | --------------------------- |
| Stream<T> filter(Predicate<? super T> predicate); | 产生一个满足当前条件P的元素 |
| count                                             | 产生当前流中元素的个数      |
|                                                   |                             |



### 并行操作

在产生流的过程中可以使用parallelStream()产生并行流




