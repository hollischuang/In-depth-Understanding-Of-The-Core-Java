# 《深入理解Java核心技术（基础篇》勘误

亲爱的读者们，欢迎大家对本书内容进行勘误，如您在本书中发现需要修改的地方，请通过提交Issue的方式告知我们，谢谢

# 以下勘误问题存在于<印次：2022年7月第4次印刷>版本中。



# 以下勘误问题存在于<印次：2022年6月第2次印刷>版本中。

## 第四章

## 第五章

### 51页


代码除需要修改

```
public void pass(User user){
  user = new User();
  user.setName("hollischuang");
  System.out.println("print in pass , user is " + user);

}


```

改为：

```
public void pass(User user){
  user = new User();
  user.setName("hollischuang");
  user.setGender("Male");
  System.out.println("print in pass , user is " + user);

}

```

即，新增`user.setGender("Male");`


### 51页

图5-2中，最下面的灰色方框中，两个橙色方框的位置需要上下调换一下。

## 第八章

### 114

倒数第四段，“所以，s3与s4的关系应该和s与s2的关系一样不相等才对”修改为”所以，s3与s4的关系应该和s1与s2的关系一样不相等才对“.

## 第九章

整章调整为：https://github.com/hollischuang/In-depth-Understanding-Of-The-Core-Java/blob/main/when_finally_execute 

## 第十章

### 141页

`String[] strings = String[] strings = {xxx}`中，String[] strings = 重复了，改为` String[] strings = {xxx}`

### 159页

最后一段代码中 list.stream().skip(strart).limit(end) 中的strart 改为 start 

### 173页

第三段文字中"remove方法源码如下。" 这句话多余，删除。

在第四段文字前增加一句描述："通过查看前面我们贴出来的remove方法的源码我们可以发现，当index>elementCount时"，更方便理解。

### 184页

第二段代码第二行，int aHandredMillion = 10000000 改为 int aHandredMillion = 100000000；

### 197页

第二行， Stack Overflor 改为 Stack Overflow

## 第十二章

### 259页

"如果要序列化的类有父类.....那么父类也应该集成..."这里的"集成"改为"继承"

### 275页

标题里面单词拼错了，应该为：Apache-Commons-Collections

### 296页

第一行，”这种形式定义不二类型的属性“，错别字“不二”应为”布尔“

### 299页

298和199页中，文字里面的json 双引号格式不统一，有的是中文引号，有的是英文引号。把299的{”success“:true}改为{"success":true}

## 第十三章

### 306页

第一句文字，“所以，定先定义的枚举” 改为 “所以，先定义的枚举” 。

## 第十六章

### 348页

第二行，”即使该注解没有使用@Retention“ 改为 ”即使该注解没有使用@Inherited“

## 第17章

### 374页

第三段，”问题来了，Child接口实现了Parent接口“，改为"Child类实现了Parent接口"

## 第20章

### 415页

第一行"任意多个下画线"改为”任意多个下划线“


# 以下勘误问题存在于<印次：2022年5月第1次印刷>版本中。

## 第二章

### 19页

当编写一个可实例化的类时，如果没有专门编写构造函数，那么多数......Interge -> null 

和下一段有重复，需要删除本段。

### 21页

而对于线程c和d，  改为 "而对于变量c和d"

## 第六章

### 58页

https://github.com/hollischuang/In-depth-Understanding-Of-The-Core-Java/issues/2

## 第七章

### 67页

“原因就是和Integer中的缓存机制有关....如果数字在128至127之间，” 这里的128应该为-128。

## 第八章

### 81页

代码段中第三行注释“使用replace将a替换成H”，应该改为"使用replaceAll将a替换成H"

### 86页

1、”查看StringUtils.join的源代码....它也是通过StringBuilde实现...  “这里的StringBuilde应该替换为StringBuilder

2、代码段中的`&gt;` 改为 ">"


### 110页

可以看到，在Class文件的.... Holl、s888这六个常量。其中"s888"为笔误，应该是"is888"

### 111页

"在《深入理解Java虚拟》中"，改为"在《深入理解Java虚拟机》中"

### 116 

但s2.intern()会从池中取出已有的引用，这就和s2相等了，这里应该是和s1相等了

## 第九章

### 124页

"以上介绍了异常的声明....6.4节将介绍一些...."  这里的6.4改为9.4

### 140页

以上代码的输出结果为3，这里应该改为'以上代码的输出结果为2'


## 第十章

### 142页

图10-1 ，interface和class的颜色标反了


### 147页

Map遍历中通过key找value遍历，key和value类型都应为string，即 Integer value = map.get(key) 中的Integer需要改为String


### 152页

表格中Vector的缺点"不适合查找"修改为"不适合插入、删除"

### 156页

代码段中System.out.println("subList.set(3,666)得到List : ") 改为 System.out.println("subList.set(1,666)得到List : ")

### 233页

"相比于非阻塞队列.....而非阻塞队列虽然安全性不如非阻塞队列..."  修改为 "相比于非阻塞队列.....而非阻塞队列虽然安全性不如阻塞队列..." 

https://github.com/hollischuang/In-depth-Understanding-Of-The-Core-Java/issues/1

## 第13章

### 311页

4枚举可解决反序列化会破坏单例模式的问题
……
第二段：在 13.4 节中介绍过，……
应该是：在 13.5 节……

## 第18章

### 388页

最后一段代码的注释中 Data 应该改为 Date

### 399页

顶部第3点

……
……
……，而1.1、1.2、1.3 才属于2020年，1.4 周日是下一周的开始，所以第一周应该只有1.1、1.2、1.3这三天

应是：

……，而1.1、1.2、1.3、1.4 才属于2020年，1.5 周日是下一周的开始，所以第一周应该只有1.1、1.2、1.3、1.4这四天

https://github.com/hollischuang/In-depth-Understanding-Of-The-Core-Java/issues/5

