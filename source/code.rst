代码
=====

前缀
~~~~~~

公共
-----

``qloc`` 或 ``QLOC`` ，意为 ``Quectel Location``

接口层
------

``qloci`` 或 ``QLOCI`` ，意为 ``Quectel Location Interface``

核心层
------

``qlocc`` 或 ``QLOCC`` ，意为 ``Quectel Location Core``

移植层
------

``qlocp`` 或 ``QLOCP`` ，意为 ``Quectel Location Port``

注释
~~~~~~

必须使用英文进行注释，防止不同编码格式打开时造成乱码。

文件注释
--------

.. code-block:: c
   :linenos:

    /**
    * @file [file name]
    * 
    * @brief [brief comment]
    * 
    * @copyright Copyright (c) 2021 Quectel Wierless Solution,Co.,Ltd. All Rights Reserved.
    * 
    * ============================== EDIT HISTORY FOR MODULE ==============================
    * This section contains comments describing the changes made to the module.
    * Notice that the latest change comment should be at the bottom.
    * WHEN         WHO                 WHAT,WHERE,WHY
    * ----------   -----------------   ----------------------------------------------------
    * YYYY-MM-DD   [your name]         [note]
    */

示例

.. code-block:: c
   :linenos:

    /**
    * @file qloc_common.h
    * 
    * @brief Quectel Location Common Header File.
    * 
    * @copyright Copyright (c) 2021 Quectel Wierless Solution,Co.,Ltd. All Rights Reserved.
    * 
    * ============================== EDIT HISTORY FOR MODULE ==============================
    * This section contains comments describing the changes made to the module.
    * Notice that the latest change comment should be at the bottom.
    * WHEN         WHO                 WHAT,WHERE,WHY
    * ----------   -----------------   ----------------------------------------------------
    * 2021-09-07   Remy SHI            First commit.
    * 2021-10-22   Remy SHI            Add control id.
    */

函数注释
--------

.. code-block:: c
   :linenos:

    /**
    * @brief [brief comment]
    * @param [type] [name] : [meaning]
    * @return  [type] : [meaning]
    */

示例

.. code-block:: c
   :linenos:

    /**
    * @brief interface layer control function.
    * @param qloc_int32_t id : control id.
    * @param void *args : control argument.
    * @return  qloc_err_t : error code.
    */

行注释
------

- 原则一：推荐使用 ``/* */`` 多行注释的方式，以便代码可以在 C89/C90/ANSI C标准下编译。
- 原则二：注释适当。

日志
~~~~~

- 原则一：必须使用框架统一的日志接口。
- 原则二：应当正确选择日志等级。
