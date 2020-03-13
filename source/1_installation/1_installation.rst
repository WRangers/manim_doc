安装
====

本节主要参考 `Manim Github`_ 的README.

.. _Manim Github: https://github.com/3b1b/manim

Manim的安装有两种方式,第一种是安装发布的manimlib,第二种是克隆Github上的repo,在本地直接与repo中的manimlib的文件挂钩进行编译.

个人推荐第二种安装方式,因为发布的manimlib比较老了,有些功能没有更新;其次方便自己二次开发,并与自己fork的repo同步;最后是安装比较简单.这里只介绍第二种安装方式,基于Window系统,其他平台本人不熟悉,故不予以介绍,请参考Github上的README.

.. warning::
    如果你选择直接安装manimlib的话,需要把电脑的编码改成UTF-8(自行百度一下),否则可能会出现一片红的报错,但是这会对一些软件造成影响!

安装Python
########### 

官网_ 直接下载安装即可.个人建议安装 Anaconda_ ,方便一些!

.. _官网: https://www.python.org/downloads/

.. important::
    安装Python的时候要把添加到环境变量的选项勾选上.如果安装Anaconda,也要添加到环境变量(一般默认添加).



.. _Anaconda: https://www.anaconda.com/distribution/


安装相关的依赖
##############

.. tip::
    使用pip进行安装相关的包时,可以更换为国内的镜像源(自行百度一下)!
    

安装FFmpeg
------------
FFmpeg是多媒体处理库,manim的视频、图片、音乐插入与生成都依赖与它.安装请参考 文章_.

.. _文章: https://www.wikihow.com/Install-FFmpeg-on-Windows

.. important::
    也要记得把FFmpeg添加到环境变量中.

安装Cairo
----------

这个包是manim的基本图形包,直接通过pip安装会出问题,建议直接手动安装.在 `这里 <https://www.lfd.uci.edu/~gohlke/pythonlibs/#pycairo/>`_ 下载对应你的python和操作系统位数版本的Cairo.然后在 ``cmd`` 中输入

::

    pip install <Cairo的路径>(比如 C:/path/to/wheel/pycairo‑1.18.0‑cp37‑cp37m‑win32.whl)

.. important::
    如果你安装的是Anaconda,需要先启动Anaconda的环境,在命令行中输入 ``conda activate <环境名称>`` 如果省略 ``环境名称`` 则默认启动 ``root`` 环境.后续的命令行操作也都如此.

安装LaTex
------------
如果你没有使用LaTex的话,可以在网上查找相关的资料快速上手.Manim中的文字和数学公式都是通过Latex编译,然后生成SVG图片插入的.推荐下载 `MiKTeX <https://miktex.org/download>`_ ,包管理比较方便.

.. important::
    同样要把相关的路径添加到环境变量,但一般默认会添加.如果编译出现问题再检查一下.

安装Sox
---------
Sox是音频处理包.可以直接通过 ``pip install sox`` 安装.


克隆repo并安装其他依赖
#########

在电脑上选个好地方,打开 ``Git Bash`` ,输入

:: 
    
    git clone https://github.com/3b1b/manim.git

如果你有二次开发的需求,可以先fork再clone.如果你不了解Git的使用,可以参考廖雪峰的 教程_.

.. _教程: https://www.liaoxuefeng.com/wiki/896043488029600

安装其他Python依赖
-----------------

打开 ``cmd`` 命令行,进入到manim repo的本地主目录中,输入

::

    pip install -r requirements.txt

``requirement.txt`` 文件内容如下

::

    argparse==1.4.0
    colour==0.1.5
    numpy==1.16.4
    Pillow==5.2.0
    progressbar==2.5
    scipy==1.3.0
    tqdm==4.24.0
    opencv-python==3.4.2.17
    pycairo==1.17.1; sys_platform == 'linux'
    pycairo>=1.18.1; sys_platform == 'win32'
    pydub==0.23.0
    pyreadline==2.1; sys_platform == 'win32'

如果你本地已经安装了其中的一些包,但版本高于上面所列的版本号,如果不想降低版本的话,可以把上面的 ``==`` 都改为 ``>=`` ,但本人不晓得会不会出现什么问题.你也可以用Anaconda创建一个新的虚拟环境后在安装.

测试
######

在 ``cmd`` 中,进入manim的repo本地主目录,输入:

::

    python manim.py example_scenes.py SquareToCircle -pl

``python``  代表启动python, ``manim.py`` 是编译脚本, ``example_scenes.py`` 是包含你的动画代码的文件, ``SquareToCircle`` 是你要编译的动画类, ``-pl`` 是编译选项,后面会有详细介绍.第一和第二个是必不可少的.

如果最后出现动画了,那恭喜你,你已经完成了安装的一大半!为什么不是成功安装呢?请看FAQ.

你也可以选择Live Sreaming模式,但我觉得挺鸡肋的.

::

    > python -m manim --livestream
    Writing to media/videos/scene/scene/1080p30/LiveStreamTemp.mp4

    Manim is now running in streaming mode. Stream animations by passing
    them to manim.play(), e.g.
    >>> c = Circle()
    >>> manim.play(ShowCreation(c))

    >>>

----

如果你安装的是manimlib库,应该输入

::

    manim my_project.py MyScene

``manim`` 是直接启动manim, ``my_project.py`` 就是包含你的动画代码的文件, ``MyScene`` 是你要编译的动画类.可以附加编译选项,这里没有加.

再次不推荐你安装manimlib!