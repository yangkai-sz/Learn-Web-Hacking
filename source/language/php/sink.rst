Sink
=================================

执行系统命令
---------------------------------
- pcntl_exec
- exec
- passthru
- popen
- shell_exec
- system
- proc_open

Magic函数
---------------------------------
- ``__construct()`` 构建对象的时被调用
- ``__destruct()`` 销毁对象或脚本结束时被调用
- ``__call()`` 调用不可访问或不存在的方法时被调用
- ``__callStatic()`` 调用不可访问或不存在的静态方法时被调用
- ``__get()`` 读取不可访问或不存在属性时被调用
- ``__set()`` 给不可访问或不存在属性赋值时被调用
- ``__isset()`` 对不可访问或不存在的属性调用 ``isset`` 或 ``empty()`` 时被调用
- ``__unset()`` 对不可访问或不存在的属性进行 ``unset`` 时被调用
- ``__sleep()`` 对象序列化时被调用
- ``__wakeup()`` 对象反序列化时被调用
- ``__toString()`` 当一个类被转换成字符串时被调用
- ``__invoke()`` 对象被以函数方式调用时被调用
- ``__set_state()`` 调用 ``var_export()`` 导出类时被调用
- ``__clone()`` 进行对象clone时被调用
- ``__debugInfo()`` 调用 ``var_dump()`` 打印对象时被调用

文件相关敏感函数
---------------------------------
- ``move_uploaded_file``
- ``file_put_contents`` / ``file_get_contents``
- ``unlink``
- ``fopen`` / ``fgets``

SSRF
---------------------------------
- ``file_get_contents()``
- ``fsockopen()``
- ``curl_exec()``
- ``fopen()``
- ``readfile()``
