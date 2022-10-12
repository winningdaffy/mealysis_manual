软件功能
=============

新建试验
--------------

点击 :numref:`tool_bar_tab` 中的 **文件** 按钮，如 :numref:`img-new_experiment-no_select` 所示：

.. figure:: /images/new_experiment-no_select.png
    :width: 600px
    :align: center
    :name: img-new_experiment-no_select

    新建试验

在 **新建** 页面有多个按钮能够新建不同类型的试验项目，包括 **新建试验** 、 **新建脚本** 、 **新建xxx试验** 等按钮及模板

    -  **新建试验** 按钮能够建立空试验，后续再添加试验使用的设备
    -  **新建脚本** 按钮能够建立空的python脚本，结合软件提供的API接口实现数据计算、自动控制等多种功能
    - 其他的按钮为针对各种设备的模板，能够再创建试验后自动添加设备、计算脚本、显示模板到试验中，然后可以直接开始测试

新建试验模板由python代码构成，可以自己构建所需的模板。

打开试验
--------------

点击 :numref:`tool_bar_tab` 中的 **文件->打开** 按钮，如 :numref:`file_open` 所示：

.. figure:: /images/open_experiment.png
    :width: 600px
    :align: center
    :name: file_open 

    打开试验

打开试验包括两部分： **最近的文件** 和 **计算机文件** 。通过 **最近的文件** 能够快速打开最近打开过的试验；通过 **计算机文件** 能够浏览计算机中的试验并打开。

软件选项
--------------

点击 :numref:`tool_bar_tab` 中的 **文件->选项** 按钮。在 **软件选项** 中包括了软件所有的全局设置，包括以下几个部分：

- **设备驱动插件**，如 :numref:`app_option` 所示。列出了所有支持的设备驱动，可以根据需要勾选，如果不勾选则软件不会加载相应的设备驱动；如果某个设备驱动为灰色并且不可勾选，则表示驱动版本过低，需要升级

.. figure:: /images/app_option.png
    :width: 600px
    :align: center
    :name: app_option 

    设备驱动插件


- **分析算法插件**，如 :numref:`option_analysis_plugin` 所示。列出了软件所有支持分析算法

.. figure:: /images/option_analysis_plugin.png
    :width: 600px
    :align: center
    :name: option_analysis_plugin 

    分析算法插件


- **搜索路径**，如 :numref:`option_search_path` 所示。配置文件及脚本的搜索路径，默认为试验项目路径和应用程序路径

.. figure:: /images/option_search_path.png
    :width: 600px
    :align: center
    :name: option_search_path 

    搜索路径


- **全局变量**，如 :numref:`option_global_variable` 所示。可以定义全局变量，在软件中使用

.. figure:: /images/option_global_variable.png
    :width: 600px
    :align: center
    :name: option_global_variable 

    全局变量


脚本设置
-------------------

软件中测试时运行的脚本分为两种类型，一种类型是每次数据采集完成运行脚本；一种类型是周期运行脚本。






测试
-------------------



显示设置
-------------------


数据选择
-------------------


记录数据
-------------------


