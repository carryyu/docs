.. _cn_api_paddle_compat_to_text:

to_text
-------------------------------

.. py:function:: paddle.compat.to_text(obj, encoding='utf-8', inplace=False)

飞桨中的所有字符串都需要用文本字符串表示。
此函数将对象转换为不带任何编码的文本字符串。特别是，如果对象类型是列表或集合容器，我们将迭代对象中的所有项并将其转换为文本字符串。

在 Python3 中：

    使用特定编码将 bytes 类型对象解码为 str 类型。

在 Python2 中：

    使用特定编码将 str type 对象解码为 unicode 类型。

参数
::::::::::

    - **obj** (unicode|str|bytes|list|set) - 要解码的对象。
    - **encoding** (str) - 解码字符串的编码格式。
    - **inplace** (bool) - 是否改变原始对象或创建一个新对象。

返回
::::::::::

    obj 解码后的结果。

代码示例
:::::::::

COPY-FROM: paddle.compat.to_text
