数据记录
================

选择记录数据
------------------

在某些情况下，采集的数据很多，需要记录的数据是其中的一部分，为了避免磁盘空间占用，可以选择部分数据记录。

1. 点击功能栏上的 **记录数据选择** 按钮，打开记录数据选择视图

.. figure:: /images/record_data_select_wnd.png
    :width: 400px
    :alt: record data select window
    :align: center
    :name: img_record_data_select_wnd

    记录数据选择视图

2. 勾选或取消勾选复选框，可以添加或删除统计结果
3. 单击选择数据，数据名称变为 **粗体** 表示选中。可以用 **Shift** 或 **Ctrl** 进行批量多选。
4. 如果需要批量添加统计结果，单击需要添加统计的 **列标题** ，对应的复选框会变为选中状态，表示选择完成。如 :numref:`img_record_data_add` 所示，选择CH2、CH3后，单击 **Mean列标题** ，则增加了CH2和CH3的 **Mean** 计算结果。如果需要取消的话则再次单击Mean列标题。

.. figure:: /images/record_data_add.png
    :width: 400px
    :alt: record data add
    :align: center
    :name: img_record_data_add

    添加待记录数据
    
5. 点击 **保存** 按钮保存配置


触发设置
------------------

软件可以设置多个触发器，触发器控制开始或停止记录数据。

触发器类型
^^^^^^^^^^^^^^^

触发器分为多个种类，包括以下类型：

.. figure:: /images/trigger_type_list.png
    :width: 300px
    :alt: trigger type list
    :align: center
    :name: img_trigger_type_list

    触发器类型

- External

    + Manual，手动触发，当点击工具栏 **记录** 按钮时触发

- Data

    + Simple Edge，比较阈值触发
    + Filterd Edge，带滞回的比较阈值触发
    + Window，在窗口范围内触发
    + Pulse Window，超出阈值大于或小于指定时间触发
    + Window and Pulse Width，进入或退出窗口范围的时间大于或小于指定时间触发
    + Slope，数据的陡峭程度触发
      
- Time

    + Absolute Time, 在指定时间触发
    + Relative Time，相对上一次触发的相对时间触发

- Cycle

    + Cycle，指定循环数触发
      
- FFT

    + FFT Amplitude，FFT幅值触发


添加触发器
^^^^^^^^^^^^^^^^

1. 点击功能栏上的 **触发设置** 按钮，打开触发设置视图

.. figure:: /images/trigger_setting.png
    :width: 600px
    :alt: trigger setting
    :align: center
    :name: img_trigger_setting

    触发器设置视图
    
- 触发器分为两类

    + 开始，触发开始记录数据
    + 停止，触发停止记录数据

- 每一类下如果有多个触发器，则触发器关系为 **或**，就是当任意一个触发器被触发时都会执行对应的记录动作

2. 选择 **开始** 类别，点击工具条中的 **添加触发器** 按钮，在弹出的触发器类型中选择要添加的触发器，然后点击 **确定** 按钮
3. 选择刚添加的触发器，在 **触发器参数** 视图修改触发器参数
4. 点击工具条中的 **保存** 按钮保存设置

删除触发器
^^^^^^^^^^^^^^^^

1. 选择要删除的触发器
2. 点击工具条中的 **删除触发器** 按钮
3. 点击工具条中的 **保存** 按钮保存设置
   
清除所有触发器
^^^^^^^^^^^^^^^^

1. 点击工具条中的 **清除所有触发器** 按钮
2. 两类触发器中的 **Manual** 不会被清除，保证任何情况下都能够使用工具栏按钮控制记录功能
3. 点击工具条中的 **保存** 按钮保存设置
   

记录数据
--------------------

1. 设置触发器
2. 当 **Start** 类别中任意触发器被触发时开始记录数据
3. 当开始记录后，状态栏中的 **记录数据状态** 会变为红色
4. 当 **Stop** 类别中任意触发器被触发时停止记录数据
5. 记录完成后，数据文件会自动添加到试验中

