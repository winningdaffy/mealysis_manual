
主界面介绍
-------------


打开软件，显示如 :numref:`img_main_form` 所示主界面。


.. figure:: /images/main_form.png
    :width: 600px
    :alt: app main form
    :align: center
    :name: img_main_form

    主窗口

主界面包括以下几个部分：

1. **菜单栏**：包含文件、编辑、视图、帮助等菜单。
#. **工具栏**：提供常用工具的快捷按钮，如开始采集、停止采集、导出数据等。
#. **功能栏**：切换数据视图区的显示页面等。
#. **数据视图区**：实时显示采集到的数据。
#. **状态栏**：显示当前状态信息，如连接状态、采样频率等。
   
菜单栏功能
~~~~~~~~~~~~~~~~~~

- **文件**：打开试验文件、软件全局配置
- **测试**：测试控制，新建、保存布局，修改硬件配置，选择数据，新建和保存计算模型
- **记录**：设置记录文件名规则
- **试验**：修改试验包括的文件
- **布局**：修改页面和控件
- **脚本**：打开和调试脚本
- **工具**：自定义工具


工具栏功能
~~~~~~~~~~~~~~~~~~

- **测试** 工具栏定义如 :numref:`img_toolbar_measurement` 所示：

.. figure:: /images/toolbar_measurement.png
    :width: 600px
    :alt: Measurement tool bar
    :align: center
    :name: img_toolbar_measurement 

    测试工具栏
    

- **记录** 工具栏定义如 :numref:`img_toolbar_record` 所示：

.. figure:: /images/toolbar_record.png
    :width: 200px
    :alt: Record tool bar
    :align: center
    :name: img_toolbar_record

    记录工具栏

    
- **试验** 工具栏定义如 :numref:`img_toolbar_experiment` 所示：

.. figure:: /images/toolbar_experiment.png
    :width: 250px
    :alt: Experiment tool bar
    :align: center
    :name: img_toolbar_experiment

    试验工具栏


功能栏功能
~~~~~~~~~~~~~~~~~~

功能栏各个按钮的功能如 :numref:`img_side_bar` 所示:

.. figure:: /images/side_bar.png
    :width: 280px
    :alt: Side bar
    :align: center
    :name: img_side_bar

    功能栏按钮


数据视图区功能
~~~~~~~~~~~~~~~~~~

数据视图区显示各个设置界面和数据，数据视图的切换由功能栏按钮实现。

- 数据显示
- 通道设置
- 统计计算设置
- 计算模型设置
- 记录数据选择
- 触发设置
- 导出数据
- CAN通信设置
- PUMA通信设置
  

  


.. 工具栏各个页面功能如 :numref:`tool_bar_tab` 所示。

.. .. table:: 工具栏页面
..     :align: center
..     :name: tool_bar_tab

..     =============   ============
..     工具栏           功能
..     =============   ============
..     File            新建、打开试验，新建脚本
..     Measurement     测量数据
..     Record          记录数据相关设置
..     Experiment      试验相关配置
..     Layout          测试面板、控件配置
..     Script          脚本运行、调试
..     Tools           自定义工具
..     =============   ============



状态栏功能
~~~~~~~~~~~~~~~~~~

状态栏各个按钮的功能如 :numref:`img_status_bar` 所示:

.. figure:: /images/status_bar.png
    :width: 600px
    :alt: Status bar
    :align: center
    :name: img_status_bar

    状态栏
    
- 设备连接状态

    - 红色：未连接
    - 橙色：部分设备已连接
    - 绿色：全部设备已连接

- 数据上传状态

    - 灰色：无数据上传
    - 绿色：有数据上传
      
- 记录数据状态

    - 灰色：未进行记录
    - 红色：记录中
      
- 网络连接状态：显示当前所有网络的连接状态

