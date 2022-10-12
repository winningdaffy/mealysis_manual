快速开始
===============

建立新试验项目
-------------------

(a) 点击 :numref:`tool_bar_tab` 中的 **File** 按钮，如 :numref:`tool_file` ：

.. figure:: /images/tool_file.png
    :width: 600px
    :align: center
    :name: tool_file 

    File按钮

(b) 如 :numref:`new_experiment` ，点击 **New** -> **New Experiment** 按钮，选择试验数据文件的保存目录，建议选择空目录，避免出现文件覆盖的问题。完成后在目录中会出现扩展名为 **exp** 的文件，这个文件包括了试验中所需的配置信息，再次试验时只需要重新打开试验文件就可以继续进行试验。

.. figure:: /images/new_experiment.png
    :align: center
    :name: new_experiment 

    新建试验项目

(c) 创建试验后可以在 **Experiment** 窗口看到试验包括的内容。
(d) 如 :numref:`img-add_device` ，点击 :numref:`tool_bar_tab` 中的 **Experiment** -> **Add Devices** 按钮，打开设备管理窗口。

.. figure:: /images/tool_add_device.png
    :width: 600px
    :align: center
    :name: img-add_device 

    点击添加设备按钮

(e) 在设备管理窗口中，从设备下拉列表中勾选需要添加的设备，然后点击添加按钮将设备添加到试验，如 :numref:`check_and_add_device` 所示，一次可以选择多个设备

.. figure:: /images/check_and_add_device.png
    :align: center
    :name: check_and_add_device 

    添加设备

(f) 在 :numref:`set_sn_ip` 所示位置修改设备的 **SN** 和 **IP地址** ，然后点击 **OK** 按钮确认

.. figure:: /images/set_sn_ip.png
    :align: center
    :name: set_sn_ip 

    设置SN和IP

(g) 回到主窗口后，软件会自动根据设备配置信息搜索设备，搜索到之后设备指示标志会变为绿色 :numref:`search_device` 。在状态栏中，最左侧的图标表示当前连接设备状态，状态含义参考 :numref:`device_state` 。点击此图标可以手动连接设备。

.. figure:: /images/search_device.png
    :width: 600px
    :align: center
    :name: search_device 

    设备连接状态

(h) 在状态栏中，最左侧的图标 :numref:`img_device_state` 表示当前连接设备状态，状态含义参考 :numref:`device_state` 。点击此图标可以手动连接设备。

.. figure:: /images/device_state.png
    :align: center
    :name: img_device_state 

    设备连接状态

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

开始试验
-------------------

(a) 在设备连接后，如 :numref:`img_start_measurement` 所示，点击 :numref:`tool_bar_tab` 中的 **Measurement** -> **Run** 按钮，开始试验。

.. figure:: /images/start_measurement.png
    :align: center
    :name: img_start_measurement

    开始试验

查看数据及修改参数
--------------------------

(a) 在设备连接后，如 :numref:`img_select_data` 所示，点击 :numref:`tool_bar_tab` 中的 **Measurement** -> **Select Data** 按钮，打开数据选择窗口。

.. figure:: /images/tool_select_data.png
    :align: center
    :name: img_select_data 

    选择数据

(b) 在打开的数据选择窗口 :numref:`img_data_selector` 选择数据

    - 点击数据名称可以切换选择状态，加粗为选择状态
    - 按 **Shift** 可以进行多选
    - 使用右键菜单选择 **Add to New** 将数据添加到选中控件中
    - 使用右键菜单选择 **Add to Exist** 将数据添加到现有控件中
    - 也可以使用工具条按钮数据、过滤数据
    - 数据选择窗口可以进行多次选择

.. figure:: /images/frm_data_selector.png
    :align: center
    :name: img_data_selector 

    数据选择窗口

(c) 在数据选择完成后，可以关闭数据选择窗口，对选中数据进行监视、修改等操作。如 :numref:`img_table_control` 所示

.. figure:: /images/table_control.png
    :align: center
    :name: img_table_control

    数据选择完成

(d) 如果有实时采集的数据可以打开数据选择窗口，选择数据曲线来查看实时数据

.. figure:: /images/frm_data_selector-select_ch.png
    :align: center
    :name: img_select_ch

    选择数据曲线


.. figure:: /images/measure-time_chart.png
    :align: center
    :name: img_measure-time_chart

    查看数据曲线

记录数据
--------------------------

当连接设备具有数据采集功能时，能够将采集的数据实时保存到文件中。
(a) 设置记录数据参数

点击 **记录** 按钮，打开记录数据设置工具条，工具条如 :numref:`img_measure-time_chart` 所示。点击 **模式切换** 开关将记录模式切换到 **时间** 或 **角度** 模式。如果是 **时间** 模式需要设置记录时长；如果是 **角度** 模式需要设置 **预触发循环数** 和 **记录循环数** 。 **预触发循环数** 表示在点击记录时刻前的循环数， **记录循环数** 表示保存到数据文件中的总循环数。
修改后的数据记录参数会保存到试验中，不需要每次设置。

.. figure:: /images/tool_record_01.png
    :align: center
    :name: img_tool_record_01

    显示数据记录参数

(b) 记录数据

切换到 **测试** 工具条，点击 **记录** 按钮，开始记录数据。同时在软件状态栏会实时显示记录状态，包括是否正在记录和记录的时间或循环数，如 :numref:`img_measure-time_chart` 所示。

.. figure:: /images/status_bar-record.png
    :align: center
    :name: img_status_bar_record

    数据记录状态


查看数据文件
--------------------------
(a) 停止测试

查看数据文件时需要首先停止测试

(b) 打开试验窗口

点击侧边栏的 **试验窗口** 按钮，如 :numref:`img_experiment_panel` 所示，打开试验窗口。

.. figure:: /images/experiment_panel.png
    :align: center
    :name: img_experiment_panel

    打开试验窗口

(c) 打开文件

双击需要打开的文件，文件名前的图标变为打开状态，如 :numref:`img_file_open_state` 所示。

.. figure:: /images/file_open_state.png
    :align: center
    :name: img_file_open_state

    打开文件


(d) 查看数据

点击 **新布局** 按钮新建一个显示布局，点击 **选择数据** 打开数据选择窗口，在左侧选择数据文件。如 :numref:`img_frm_data_selector_from_file` 所示。

    - 点击数据名称可以切换选择状态，加粗为选择状态
    - 按 **Shift** 可以进行多选
    - 使用右键菜单选择 **Add to New** 将数据添加到选中控件中
    - 使用右键菜单选择 **Add to Exist** 将数据添加到现有控件中
    - 也可以使用工具条按钮数据、过滤数据
    - 数据选择窗口可以进行多次选择

.. figure:: /images/frm_data_selector_from_file.png
    :align: center
    :name: img_frm_data_selector_from_file

    选择文件中的数据


.. figure:: /images/data_of_file.png
    :align: center
    :name: img_data_of_file

    文件中的数据


导出数据
--------------------------------

(a) 打开试验窗口
(b) 在文件上点击右键，选择 **Export to CSV** 将数据导出为csv文件，如 :numref:`img_export_to_csv` 所示。

.. figure:: /images/export_to_csv.png
    :align: center
    :name: img_export_to_csv

    文件中的数据
