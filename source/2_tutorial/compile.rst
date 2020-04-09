编译选项
############

用法
-----------

对于安装manimlib的情况:

::

    manim [-h] [-p] [-w] [-s] [-l] [-m] [--high_quality] [-g] [-i] [-f]             
    [-t] [-q] [-a] [-o FILE_NAME] [-n START_AT_ANIMATION_NUMBER]             
    [-r RESOLUTION] [-c COLOR] [--sound] [--leave_progress_bars]
             [--media_dir MEDIA_DIR]
             [--video_dir VIDEO_DIR | --video_output_dir VIDEO_OUTPUT_DIR]
             [--tex_dir TEX_DIR] [--livestream] [--to-twitch]
             [--with-key TWITCH_KEY]
             [file] [scene_names [scene_names ...]]

对于克隆repo直接挂钩编译则只需把上面的 ``manim`` 改为 ``python manim.py`` 就可以了.

选项详解
------------

文件参数
==============

:file: 代码路径

:scene_names: 需要编译的代码类


可选参数
===========

-h, --help              显示帮助信息
-p, --preview           编译完成后自动播放
-w, --write_to_movie    将场景作为媒体文件渲染为电影文件
-s, --save_last_frame   输出最后一帧
-l, --low_quality       低分辨率渲染
-m, --medium_quality    中分辨率渲染
--high_quality          高分辨率渲染
-g, --save_pngs         保存每一帧为png图片
-i, --save_as_gif       保存为gif图片
-f, --show_file_in_finder
                        渲染完成后,打开文件所在文件夹
-t, --transparent       在透明通道渲染
-q, --quiet             #TODO
-a, --write_all         编译文件中的所有动画类
-o FILE_NAME, --file_name FILE_NAME
                        重新命名动画类名称
-n START_AT_ANIMATION_NUMBER, --start_at_animation_number START_AT_ANIMATION_NUMBER
                        不从第一个动画开始渲染,如果输入两个参数,例如"3,6",就只渲染第3到第6个动画
-r RESOLUTION, --resolution RESOLUTION
                        重设分辨率,输入形式为 ``高度,宽度``
-c COLOR, --color COLOR
                        设置背景颜色
--sound                 编译成/失败提示音
--leave_progress_bars
                        隐藏终端中的编译条
--media_dir MEDIA_DIR
                        设置存放媒体文件的目录
--video_dir VIDEO_DIR
                        设置存放输出视频的目录
--video_output_dir VIDEO_OUTPUT_DIR
                        设置输出视频的目录
--tex_dir TEX_DIR       设置存放 ``.tex`` 文件的目录
--livestream            进入livestream模式
--to-twitch             #TODO
--with-key TWITCH_KEY
                        #TODO