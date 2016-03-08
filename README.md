# some-questions
知识片段

#### 1.不要在dealloc init 中使用accessor
[为什么不要在init和dealloc函数中使用accessor](http://blog.smilexiaofeng.com/blog/2015/08/11/why-do-not-use-accessor-in-init-and-dealloc/)

[不要在init和dealloc函数中使用accessor](http://blog.devtang.com/2011/08/10/do-not-use-accessor-in-init-and-dealloc-method/)

> 在init和dealloc中使用accessor是存在风险的。即使现在代码没有问题，难保将来维护或扩展时会出现问题。只有将苹果所说的Don’t Use Accessor Methods in Initializer Methods and dealloc当作一条编程规范，才能从根本上规避这个问题。规矩立好了，代码欠的债就少，将来的生活就会更加美好。

> 在 init 和 dealloc 中，对象的存在与否还不确定，所以给对象发消息可能不会成功。
