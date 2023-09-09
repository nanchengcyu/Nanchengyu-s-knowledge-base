# Java基础
## Java基本构成
1）一个 Java 程序可以认为是一系列对象的集合，而这些对象通过调用彼此的方法来协同工作。下面简要介绍下类、对象、方法和实例变量的概念。

- **对象**：对象是类的一个实例，有状态和行为。例如，一条狗是一个对象，它的状态有：颜色、名字、品种；行为有：摇尾巴、叫、吃等。
- **类**：类是一个模板，它描述一类对象的行为和状态。
- **方法**：方法就是行为，一个类可以有很多方法。逻辑运算、数据修改以及所有动作都是在方法中完成的。
- **实例变量**：每个对象都有独特的实例变量，对象的状态由这些实例变量的值决定。

2）![1690789264164.jpg](https://cdn.nlark.com/yuque/0/2023/jpeg/38420467/1690789269828-1b411680-4994-48ee-bedf-b55213e16437.jpeg#averageHue=%23f0efef&clientId=uce8d3ae6-9553-4&from=paste&height=260&id=ufd483335&originHeight=292&originWidth=757&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=81499&status=done&style=none&taskId=u46a4c7f0-7288-45b8-bf5c-210295bcb87&title=&width=672.8888888888889)

## Java类与对象区分
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690790773832-bc9336a9-ff0d-4886-b3ee-b9e01c2870fc.png#averageHue=%23d7d3c3&clientId=uce8d3ae6-9553-4&from=paste&height=557&id=u3fbb9050&originHeight=627&originWidth=857&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=377997&status=done&style=none&taskId=uecf47475-f2b3-4e6e-8993-07d8ba6d8ef&title=&width=761.7777777777778)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690790902633-117ea255-b373-42eb-a0ed-bde65d82e903.png#averageHue=%23f8f4f1&clientId=u1634f63d-31e3-4&from=paste&height=558&id=u6ca4819f&originHeight=628&originWidth=986&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=82439&status=done&style=none&taskId=u9f45562b-d1c0-4e94-9fea-cf888fdaef1&title=&width=876.4444444444445)
解释：
类、对象、状态、行为
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690791104409-67a10530-223e-4d2e-bc48-e751ca5e0984.png#averageHue=%23f5f2ee&clientId=u1634f63d-31e3-4&from=paste&height=553&id=u9265ea5a&originHeight=622&originWidth=1138&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=252211&status=done&style=none&taskId=udb221454-ea35-41df-8720-5fd04efba86&title=&width=1011.5555555555555)
![上面是属性（状态），下面是方法（行为）](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690791172788-5f6ce00a-0f37-4c49-b442-57d29ced5b99.png#averageHue=%23f8f8f8&clientId=u1634f63d-31e3-4&from=paste&height=440&id=uc0d5361d&originHeight=495&originWidth=1146&originalType=binary&ratio=1.125&rotation=0&showTitle=true&size=33847&status=done&style=none&taskId=u45426648-e824-48d0-a91f-4b6d9ed227e&title=%E4%B8%8A%E9%9D%A2%E6%98%AF%E5%B1%9E%E6%80%A7%EF%BC%88%E7%8A%B6%E6%80%81%EF%BC%89%EF%BC%8C%E4%B8%8B%E9%9D%A2%E6%98%AF%E6%96%B9%E6%B3%95%EF%BC%88%E8%A1%8C%E4%B8%BA%EF%BC%89&width=1018.6666666666666 "上面是属性（状态），下面是方法（行为）")
## 构造方法与方法区别
构造方法的名称必须与类同名，一个类可以有多个构造方法。
方法不需要。
![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690791550796-a376bb8d-a22c-4ed7-bead-aabe1d58286d.png#averageHue=%23636c7a&clientId=u1634f63d-31e3-4&from=paste&height=2412&id=u40babdf2&originHeight=2714&originWidth=820&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=616346&status=done&style=none&taskId=ub2ab2dfa-0da9-4965-9d5c-97ea2acd909&title=&width=728.8888888888889)
## 方法对象实例运用展示

- **实例化**：使用关键字 new 来创建一个对象。
- **初始化**：使用 new 创建对象时，会调用构造方法初始化对象。

![image.png](https://cdn.nlark.com/yuque/0/2023/png/38420467/1690792256070-4494fe86-e186-452e-8109-be67033e7f9c.png#averageHue=%23f8f7f6&clientId=u1634f63d-31e3-4&from=paste&height=704&id=ud97f1fbe&originHeight=880&originWidth=1123&originalType=binary&ratio=1.125&rotation=0&showTitle=false&size=75201&status=done&style=none&taskId=ufb87b7bf-a188-46e6-aaca-2246142283c&title=&width=898.4)
