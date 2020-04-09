.. manim_doc documentation master file, created by
   sphinx-quickstart on Tue Mar 10 11:29:10 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Manim's documentation!
=====================================

.. image:: ../README.assets/logo_cut.png

About
======

`Manim`_ 是Grant Sanderson (3Blue1Brown) 开发的Python库,旨在制作数学动画. Sanderson最早开发该库用于自己在可汗学院教授微积分等数学课程时使用,现在Manim仍是一个在发展中的项目!如果你看过3Blue1Brown频道的数学视频,一定领略到了Manim的强大,虽然还有很多不完善的地方,但瑕不掩瑜!

本中文文档是本人业余所为,所以不能保证更新的进度.如果你想要提前了解更多,可以参考 `Theorem of Beethoven`_ 编写的 `英文文档`_ (但也不完善).另外我推荐你在YouTube频道上订阅Theorem of Beethoven频道,其专门制作Manim教程,比较系统;Bilibili上有搬运教程,但由于版权问题,我就不在这里给出链接.本文档有很多地方也都是参考Theorem of Beethoven的视频资料和文档.

Theorem of Beethoven的 `Github <https://github.com/Elteoremadebeethoven/AnimationsWithManim>`_ 上有很多有趣的projects,可供大家参考!

关于Manim,Bilibili和YouTube上都有很多有趣的资源可供参考与学习,但都比较杂,没有形成社区生态.故本文档参考资料比较杂烩,会在相关之处一一列明,如果侵权了您的权益,请与我联系!

Happy maniming!

.. _Manim: https://github.com/3b1b/manim
.. _Theorem of Beethoven: https://www.youtube.com/channel/UCxiWCEdx7aY88bSEUgLOC6A/videos
.. _英文文档: https://manim-tb-manual.000webhostapp.com/

.. toctree::
   :maxdepth: 2
   :caption: Installation

   1_installation/win.rst
   1_installation/linux.rst
   1_installation/macos.rst

.. toctree::
   :maxdepth: 2
   :caption: FAQ and Others

   faq_others/faq.rst
   faq_others/vscode.rst

.. toctree::
   :maxdepth: 4
   :caption: Tutorial

   2_getst/hw.rst
   2_getst/compile.rst

.. toctree::
   :maxdepth: 4
   :caption: Reference

   3_reference/structure/file.rst
   3_reference/structure/constants.rst

   3_reference/mobject/mobject.rst
   3_reference/mobject/vmobject.rst
   3_reference/mobject/pmobject.rst
   3_reference/mobject/svg_mobject.rst
   3_reference/mobject/image_mobject.rst
   3_reference/mobject/tex_mobject.rst
   3_reference/mobject/text_mobject.rst


.. toctree::
   :maxdepth: 4
   :caption: Advanced Usage
   :numbered:


.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`
