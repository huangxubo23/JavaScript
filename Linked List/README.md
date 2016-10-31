## 链表

### 数组的缺点
数组不总是组织数据的最佳数据结构，原因如下。在很多编程语言中，数组的长度是固定的，所以当数组已被数据填满时，再要加入新的元素就会非常困难。
在数组中，添加和删除元素也很麻烦，因为需要将数组中的其他元素向前或向后平移，以反映数组刚刚进行了添加或删除操作。
然而，JavaScript 的数组并不存在上述问题，因为使用 split() 方法不需要再访问数组中的其他元素了

JavaScript中数组的主要问题是，它们被实现成了对象，与其他语言（比如 C++ 和 Java）的数组相比，效率很低。
如果你发现数组在实际使用时很慢，就可以考虑使用链表来替代它。除了对数据的随机访问，链表几乎可以用在任何可以使用一维数组的情况中。
如果需要随机访问，数组仍然是更好的选择。

### 定义链表
`链表（Linked List）`是由一组节点组成的集合。每个节点都使用一个对象的引用指向它的后继。指向另一个节点的引用叫做链。
数组元素靠它们的位置进行引用，链表元素则是靠相互之间的关系进行引用。


遍历链表，就是跟着链接，从链表的首元素一直走到尾元素（但这不包含链表的头节点，头节点常常用来作为链表的接入点）。
然而要标识出链表的起始节点却有点麻烦，许多链表的实现都在链表最前面有一个特殊节点，叫做头节点。链表的尾元素指向一个 null 节点。