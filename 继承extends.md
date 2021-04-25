继承extends

语法：子类名extends 父类名

父类

```
public class Uncle {
    private String name;
    private int age;

    public void faHongbao(){
        System.out.println("发红包");

    }
}
```

子类一

```
public class UncleOne {
    //独有的方法
    public void choyan() {
        System.out.println("大舅喜欢吸烟");

    }
}
```

子类二

```
public class UncleTwo {
    //独有的方法
    public void hejiu(){
        System.out.println("二舅喜欢喝酒");
    }
    //复写（覆写）Override 父类中的方法
    public void faHongbao(){
        System.out.println("家道中落，不发红包，改为祝福");
    }
}
```

优点

1提高了代码的利用率

2提高了代码的扩展性

覆写

```
 //复写（覆写）Override 父类中的方法
    public void faHongbao(){
        System.out.println("家道中落，不发红包，改为祝福");
    }
```

多层继承（层次继承）

```
//多层继承
public class UncleTwoSon {
    public void faHongbao() {
        System.out.println("逆袭了，发红包");
    }
}

```

警告：不支持多重继承

```
public class Temp extends UncleOne,UncleTwo{
}
```

final 最终的

被final的修饰的内容不能再被更改

final 修饰的变量不能被修改 基本数据类型 如果修饰的是引用数据类型，引用的地址不能发生变化，但是引用位置得知可以发生修改

final 修饰的方法不能被重写

final 修饰的类不能被继承