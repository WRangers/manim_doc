基本参数
===========

本节主要参考 `Constants <https://manim-tb-manual.000webhostapp.com/tree/constants.html>`_.

路径
-----------

当你第一次运行动画编译的时候,终端会出现这样的提示::

    Media will be stored in media/. You can change this behavior by writing a different directory to media_dir.txt.

这是因为动画文件会被存放在在 ``media`` 路径中,在你终端运行的主目录下,会出现新的文件

::

    .
    ├── manim.py
    ├── stage_scenes.py 
    ├── media                  # <- 新目录
    └── manimlib
        └── media_dir.txt      # <- 新文件
        └── scene 
            └── media_dir.txt  # <- 新文件

如果你不更改媒体路径的话,后面不会再出现这个提示.可以通过更改 ``media_dir.txt`` 来更改媒体保存路径,这会导致  ``manimlib/constants.py`` 第 ``14`` 行的改变.


.. literalinclude:: /manimlib/constants.py
    :lines: 4-53
    :lineno-start: 4
    :emphasize-lines: 11

更多细节请参考 `FAQ 2.7 <如何改变视频输出地址>`_.


Text设置
----------

``Text`` 类的设置.

.. literalinclude:: /manimlib/constants.py
    :lines: 55-72
    :lineno-start: 55

LaTex编译设置
--------------

.. literalinclude:: /manimlib/constants.py
    :lines: 74-85
    :lineno-start: 74

帮助与报错信息
--------------

.. literalinclude:: /manimlib/constants.py
    :lines: 87-115
    :lineno-start: 87

分辨率
----------

.. literalinclude:: /manimlib/constants.py
    :lines: 117-140
    :lineno-start: 117

画面尺寸
----------------

.. literalinclude:: /manimlib/constants.py
    :lines: 142-154
    :lineno-start: 142

间距
-----

.. literalinclude:: /manimlib/constants.py
    :lines: 156-162
    :lineno-start: 156

时间
-------

.. literalinclude:: /manimlib/constants.py
    :lines: 165-167
    :lineno-start: 165

向量
-------

.. literalinclude:: /manimlib/constants.py
    :lines: 170-190
    :lineno-start: 170

角度
------

.. literalinclude:: /manimlib/constants.py
    :lines: 192-194
    :lineno-start: 192

颜色
-------------

.. raw:: html

    <a href="https://manim-tb-manual.000webhostapp.com/_static/colors/colors.html"> 颜色盘展示 </a>

.. note::
    
    默认 ``COLOR = COLOR_C``

.. literalinclude:: /manimlib/constants.py
    :lines: 198-262
    :lineno-start: 198

..