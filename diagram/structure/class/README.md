## Class Diagram

**类之间的关系**

- Dependency (依赖)
- Association (关联)
- Aggregation (聚合)
- Composition (组合)
- Realization (实现)
- Generalization (继承)

**类之间关系的简称**

- has-a
- is-a
- contains-a

**类图的表示方法**

- `+` 表示 public 绿色圆形
- `#` 表示 protected 或 friendly 黄色棱形
- `-` 表示 private 红色正方形
- `~` 表示 default 也就是 package 权限 蓝色三角
- `_` 表示 static 下划线
- *italic* 表示抽象 斜体
- 方法 (method) 实心，变量 (field) 空心


**类之间关系的实现描述**

- 依赖
  - A 类使用到了 B 类一部分属性或方法。不会主动改变 B 类内的内容；
  - 类 A 把类 B 的实例作为方法里的参数使用；
  - 类 A 的某个方法里使用了类 B 的实例作为局部变量；
  - 类 A 调用了类B的静态方法；
- 关联 A 类需要 B 类作为它的属性，以进行一定的读操作。
- 聚合 A 类在一定情形下属于 B 类内，即 A 类可以独立于 B 类存在。
- 组合 A 类属于 B 类，即 A 类不可以独立存在。A 析构时 B 被销毁。
- 泛化 A 类拥有 B 类全部属性，并且可以额外拥有一些 B 类没有的特征。
- 实现 A 类实现 B 类的纯虚函数。
