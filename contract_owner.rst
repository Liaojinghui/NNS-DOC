**********
所有者合约
**********

所有者合约采用Appcall的形式调用顶级域名合约的owner\_SetXXX 接口

::

        [Appcall("dffbdd534a41dd4c56ba5ccba9dfaaf4f84e1362")]
        static extern object rootCall(string method, object[] arr);

顶级域名合约会检查调用栈，取出调用它的合约和顶级域名合约管理的所有者进行比对。

所以只有所有者合约可以实现管理

意义
=====

用户可以用所有者合约实现负责的合约所有权模式比如：

- 双人共有，双人签名操作。
- 多人共有，投票操作。

范例
=====

暂无
