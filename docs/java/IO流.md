## I/O流





### 抽象基类

* InputStream
* OutputStream
* Reader
* Writer

### 节点流（文件流）

* FileInputStream
* FileOutputStream
* FileReader
* FileWriter



### 处理流

#### 缓冲流

* BufferedInputStream
* BufferedOutputStream
* BufferedReader
* BufferedWriter

**缓冲流原理**

以输出流为例：BufferedOutputStream,BufferedWriter

使用Array数组作为缓冲区

当写入的数据长度比缓冲区总长度大时（写入的数据不可能够放了），直接将写入的数据和缓冲区数据全部写出

当写入的数据长度比缓冲区空白区长度大时，先写出缓冲区的内容，清空缓冲区，然后将数据复制到缓冲区



所以缓冲流真正写出到底层的操作是由“缓冲区放不下数据了”触发的



#### 转换流

InputStreamReader,OutputStreamWriter

InputStreamReader:将读数据的字节流转换为字符流

OutputStreamWriter：将写数据的字符流转换为字节流

#### 标准输入、输出流

用于指明输入流的来源和输出流的流向

```java
InputStream：标准输入流
PrintStream：标准输出流

System.out.println() :该方法是向设定的标准输出流写出数据

默认的标准输入流是键盘，标准输出流是显示器

通过System.setIn(),System.setOut()可以设置输入，输出流
比如：
        File file = new File("./class18/src/test.txt");
        PrintStream outputStream = new PrintStream(file);
        System.setOut(outputStream);

        System.out.println("this is a test!!!");


        outputStream.close();

这样的输出流向是输出到文件

```

#### 数据流

DataInputStream,DataOutputStream

为了方便地操作Java语言的基本数据类型和String的数据，可以使用数据流

```java
readBoolean(),readByte(),readChar(),readFloat()等
```

#### 对象流

ObjectInputStream，ObjectOutputStream

用于存储和读取基本数据类型或对象的处理流



##### 序列化



##### 反序列化



**不能序列化static和transient修饰的成员变量**



**serialVersionUID**

主要是解决数据传输的不一致问题，java会对传输过来的UID和本地的UID（在导入的包的类里面）进行比较，如果不一致会抛出异常