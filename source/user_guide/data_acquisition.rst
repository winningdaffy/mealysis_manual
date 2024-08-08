数据采集
================

连接硬件
-------------

1. 连接硬件模块到计算机
2. 设置计算机IP地址
3. 搜索硬件模块

 - 打开软件后，软件会自动搜索试验中配置的硬件模块
 - 网络连接变化时，软件会自动搜索试验中配置的硬件模块
 - 点击状态栏中的 **设备连接状态按钮** 按钮，能够手动搜索试验中配置的硬件模块

4. 状态栏的设备连接状态指示当前设备连接情况，如 :numref:`device_state` 所示

.. table:: 设备连接状态
    :align: center
    :name: device_state 

    =============   ============
    颜色            状态
    =============   ============
    红色            所有设备未连接
    橙色            部分设备已连接
    绿色            所有设备已连接
    =============   ============



开始测试
-------------

1. 点击工具栏中的 **开始测试** 按钮，开始测试
2. 如果测试正常，则状态栏中的 **数据上传状态** 图标会变成绿色，表示数据实时从硬件模块中传输到软件系统

.. figure:: /images/data_transfer_state.png
    :width: 400px
    :alt: data transfer state
    :align: center
    :name: img_data_transfer_state

    数据传输状态


查看数据
-------------

1. 点击工具栏中的 **选择数据** 按钮，打开数据选择窗口，如 :numref:`img_data_select_wnd` 所示。数据选择窗口的工具栏按钮定义如 :numref:`img_data_select_wnd_toolbar` 所示。

.. figure:: /images/data_select_wnd.png
    :width: 600px
    :alt: data_select_wnd
    :align: center
    :name: img_data_select_wnd

    数据选择窗口
    

.. figure:: /images/data_select_wnd_toolbar.png
    :width: 600px
    :alt: data_select_wnd tool bar
    :align: center
    :name: img_data_select_wnd_toolbar

    数据选择窗口工具栏


2. 单击数据列表中的数据名称，当数据名称变为 **加粗** 时表示数据选中，选中状态下单击为取消选中
3. 按住 **Shift** 能够进行多选
4. 选择数据后，点击右键，打开菜单选择 **Add to Exist** 或 **Add to New** 中的控件，控件类型如 :numref:`img_data_select_control` 所示 

.. figure:: /images/data_select_control.png
    :width: 400px
    :alt: data_select_wnd cotnrol
    :align: center
    :name: img_data_select_control

    添加数据到控件
    

控件
-------------

软件可以使用多种控件查看各种数据，控件类型包括：

- Table，表格
- CA Chart，曲线图
- Trend Chart，趋势图
- Bar Chart，柱状图
  
表格
^^^^^^^^^^^^^

表格控件用来显示数值数据，当用表格控件显示曲线数据时，控件只显示曲线的第一个数值。
表格控件能够显示只读数据和可修改数据，当显示不同类型数据时，控件能够自动识别数据类型，并以合适的方式显示。

- 只读数据

.. figure:: /images/table_control_readonly.png
    :width: 300px
    :alt: table control readonly
    :align: center
    :name: img_table_control_readonly

    显示只读数据

- 可修改，多选项数据

.. figure:: /images/table_control_enum.png
    :width: 300px
    :alt: table control enum 
    :align: center
    :name: img_table_control_enum

    显示可修改多选项数据

- 可修改，数值数据

.. figure:: /images/table_control_value.png
    :width: 300px
    :alt: table control value
    :align: center
    :name: img_table_control_value

    显示可修改数值数据

操作表格数据
:::::::::::::::::

表格中的数据能够上下移动和删除，首先选择要操作的数据，然后点击鼠标右键弹出菜单，选择以下操作：

- Move Up，上移
- Move Down，下移
- Delete，删除
  
.. figure:: /images/table_control_popup.png
    :width: 300px
    :alt: table control popup
    :align: center
    :name: img_table_control_popup

    数据操作

曲线图
^^^^^^^^^^^^^

曲线图控件用来显示曲线数据，能够显示基于角度的曲线和基于时间的曲线，控件能够自动判断曲线坐标类型并显示横坐标。

.. figure:: /images/ca_chart.png
    :width: 500px
    :alt: ca chart control
    :align: center
    :name: img_ca_chart

    曲线图

曲线图控件工具条有以下功能按钮。

.. figure:: /images/chart_toolbar.png
    :width: 300px
    :alt: chart tool bar
    :align: center
    :name: img_chart_toolbar

    曲线图

光标
:::::::::::::::::

1. 点击 **添加光标** 按钮
2. 点击 **显示数据列表** 按钮，打开数据列表，在数据列表中会显示所有添加光标的数值

坐标轴合并
:::::::::::::::::

1. 点击 **显示数据列表** 按钮，打开数据列表
2. 在数据列表中按住 **Ctrl** 键，点击数据名称选择多个数据
3. 点击 **合并纵坐标轴** 按钮，可以实现坐标轴合并
4. 点击 **取消合并纵坐标轴** 按钮，可以取消坐标轴合并

坐标轴堆叠
:::::::::::::::::

1. 点击 **显示数据列表** 按钮，打开数据列表
2. 在数据列表中按住 **Ctrl** 键，点击数据名称选择多个数据
3. 点击 **堆叠纵坐标轴** 按钮，可以实现坐标轴合并
4. 点击 **取消堆叠纵坐标轴** 按钮，可以取消坐标轴合并
   

趋势图
^^^^^^^^^^^^^

趋势图控件用来显示数值数据，当用趋势图控件显示曲线数据时，控件每次会将曲线数据的第一个数值添加到趋势图中。

.. figure:: /images/trend_chart.png
    :width: 500px
    :alt: trend chart control
    :align: center
    :name: img_trend_chart

    趋势图
    
趋势图的工具栏功能参考 :numref:`img_chart_toolbar`。

柱状图
^^^^^^^^^^^^^

柱状图控件用来显示数值数据，当用柱状图控件显示曲线数据时，控件每次会将曲线数据的第一个数值添加到柱状图中。

.. figure:: /images/bar_chart.png
    :width: 200px
    :alt: bar chart control
    :align: center
    :name: img_bar_chart

    趋势图
    

布局
------------

在添加一个或多个控件后，软件能够将布局保存为布局文件，以便在下一次测试时直接使用，不需要重新添加控件。
试验文件下可以添加多个布局文件，以满足在不同的测试中对数据显示的不同需求。

新建布局
^^^^^^^^^^^^^

1. 点击工具栏中的 **新建布局** 按钮
2. 新建布局会清除当前的布局和所有控件


保存布局
^^^^^^^^^^^^^

1. 点击工具栏中的 **保存布局** 按钮
2. 在打开的对话框选择布局保存位置，然后按 **确定** 按钮
3. 保存后的布局文件会自动添加到试验中，并且在下一次开打试验时自动加载
4. 布局文件的扩展名是 **.mly**

.. figure:: /images/save_layout.png
    :width: 200px
    :alt: save layout
    :align: center
    :name: img_save_layout

    保存的布局