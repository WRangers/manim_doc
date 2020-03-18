Manimlib架构
=============

::
  
    .
    ├── manim.py
    ├── stage_scenes.py 
    ├── manimlib
    │   ├── animation
    │   │   ├── animation.py
    │   │   ├── composition.py
    │   │   ├── creation.py
    │   │   ├── fading.py
    │   │   ├── growing.py
    │   │   ├── indication.py
    │   │   ├── movement.py
    │   │   ├── numbers.py
    │   │   ├── rotation.py
    │   │   ├── specialized.py
    │   │   ├── transform.py
    │   │   └── update.py
    │   ├── camera
    │   │   ├── camera.py
    │   │   ├── mapping_camera.py
    │   │   ├── moving_camera.py
    │   │   ├── multi_camera.py
    │   │   └── three_d_camera.py
    │   ├── config.py
    │   ├── constants.py
    │   ├── container
    │   │   └── container.py
    │   ├── ctex_template.tex
    │   ├── extract_scene.py
    │   ├── files
    │   │   ├── Bubbles_speech.svg
    │   │   ├── Bubbles_thought.svg
    │   │   └── PiCreatures_plain.svg
    │   ├── for_3b1b_videos
    │   │   ├── common_scenes.py
    │   │   ├── pi_class.py
    │   │   ├── pi_creature_animations.py
    │   │   ├── pi_creature.py
    │   │   └── pi_creature_scene.py
    │   ├── mobject
    │   │   ├── changing.py
    │   │   ├── coordinate_systems.py
    │   │   ├── frame.py
    │   │   ├── functions.py
    │   │   ├── geometry.py
    │   │   ├── matrix.py
    │   │   ├── mobject.py
    │   │   ├── mobject_update_utils.py
    │   │   ├── number_line.py
    │   │   ├── numbers.py
    │   │   ├── probability.py
    │   │   ├── shape_matchers.py
    │   │   ├── svg
    │   │   │   ├── brace.py
    │   │   │   ├── drawings.py
    │   │   │   ├── svg_mobject.py
    │   │   │   └── tex_mobject.py
    │   │   │   └── text_mobject.py
    │   │   ├── three_dimensions.py
    │   │   ├── three_d_shading_utils.py
    │   │   ├── three_d_utils.py
    │   │   ├── types
    │   │   │   ├── image_mobject.py
    │   │   │   ├── point_cloud_mobject.py
    │   │   │   └── vectorized_mobject.py
    │   │   ├── value_tracker.py
    │   │   └── vector_field.py
    │   ├── once_useful_constructs
    │   │   ├── arithmetic.py
    │   │   ├── combinatorics.py
    │   │   ├── complex_transformation_scene.py
    │   │   ├── counting.py
    │   │   ├── fractals.py
    │   │   ├── graph_theory.py
    │   │   ├── light.py
    │   │   ├── matrix_multiplication.py
    │   │   ├── NOTE.md
    │   │   └── region.py
    │   ├── scene
    │   │   ├── graph_scene.py
    │   │   ├── moving_camera_scene.py
    │   │   ├── reconfigurable_scene.py
    │   │   ├── sample_space_scene.py
    │   │   ├── scene_file_writer.py
    │   │   ├── scene_from_video.py
    │   │   ├── scene.py
    │   │   ├── three_d_scene.py
    │   │   ├── vector_space_scene.py
    │   │   └── zoomed_scene.py
    │   ├── stream_starter.py
    │   ├── tex_template.tex
    │   └── utils
    │       ├── bezier.py
    │       ├── color.py
    │       ├── config_ops.py
    │       ├── file_ops.py
    │       ├── images.py
    │       ├── iterables.py
    │       ├── paths.py
    │       ├── rate_functions.py
    │       ├── simple_functions.py
    │       ├── sounds.py
    │       ├── space_ops.py
    │       ├── strings.py
    │       └── tex_file_writing.py
    ├── README.md          
    ├── requirements.txt   
    ├── Dockerfile         
    ├── example_scenes.py  
    └── LICENSE            

基于Theorem of Beethoven编写的 `Doc <https://manim-tb-manual.000webhostapp.com/tree/manim_packages.html>`_ 进行修改.

:manim.py: 编译启动文件.

:stage_scenes.py: # TODO

:example_scenes.py: 示例文件.

:manimlib.config.py: 设定编译指令,如输出的分辨率、输出格式、帧率、路径、背景颜色等命令.

:manimlib.stream_starter: Livestream模式的启动设置.

:manimlib.extract_scene.py: 场景解析文件,在编译过程中会使用到.

:manimlib.imports.py: 模块导入文件.如果你自主开发了一些功能,添加在库中,为了方便调用,你可以在这里文件里面添加相应的模块.

:manimlib.media_dir.txt: 媒体文件路径.正常情况下,媒体文件都会储存在你的终端运行的主目录下的 ``/media`` 中,你可以自定义修改.

:manimlib.tex_template.tex: 默认LaTex模板.

:manimlib.ctex_template.tex: 使用中文时的LaTex模板.

:manimlib.constants.py: 基本参数,将在基本参数中介绍.


